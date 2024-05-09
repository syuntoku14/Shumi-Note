# Mirror Descent

オンラインのMirror descentでは次の問題をときます：

$$
x_{k+1} \in \arg \min _{x \in C} t_K\left\langle g_k, x-x_k\right\rangle+B_\omega\left(x, x_k\right)
$$

ここで$t_K$はステップサイズで，$B_\omega$はBregman divergenceです．
特に$C$を単位単体としてKL divergenceを選択すれば，

$$
x_{k+1} \in \arg \min _{x \in C}\left\{t_K\left\langle\nabla f_k\left(x_k\right), x-x_k\right\rangle+d_{K L}\left(x \| x_k\right)\right\}
$$

と同じです．

## オンラインMirror descentの基本の不等式

参考：
* [Exploration Exploitation in Constrained MDPs](https://arxiv.org/abs/2003.02189)のLemma 39


準備：
* $g_{k, i} \geq 0$が$k=1, \dots, K$と$i=1, \dots, d$で成立．これが勾配に相当．
* $C=\Delta_d$
* 初期化は一様に$x_1=[1 / d, \ldots, 1 / d]$とする
* 学習率$t_K$

このとき，任意の$u \in \Delta_d$について，

$$
\sum_{k=1}^K\left\langle g_t, x_k-u\right\rangle \leq \frac{\log d}{t_K}+\frac{t_K}{2} \sum_{k=1}^K \sum_{i=1}^d x_{k, i} g_{k, i}^2
$$

が成立する．

## オンラインのMirror descentをするときに便利

参考：
* [Exploration Exploitation in Constrained MDPs](https://arxiv.org/abs/2003.02189)

準備：
* $t_K > 0$
* $\pi_h^1(\cdot \mid s)$：任意の$h$と$s$について一様分布．
* $Q_h^k(s, a) \in[0, M]$が任意の$k$と$h$で成立

このとき，

$$
\pi_h^{k+1}(\cdot \mid s) \in \arg \min _{\pi \in \Delta_A} t_K\left\langle Q_h^k(s, \cdot), \pi-x_h^k(\cdot \mid s)\right\rangle+d_{K L}\left(\pi \| \pi_h^k(\cdot \mid s)\right) .
$$

に従ってMirror descentを実行すると，任意の$k \in [K], h\in[H], s \in \mathcal{S}$について，任意の$\pi$について次が成立する．

$$
\sum_{k=1}^K\left\langle Q_h^k(\cdot \mid s), \pi_h^k(\cdot \mid s)-\pi_h(\cdot \mid s)\right\rangle \leq \frac{\log A}{t_K}+\frac{t_K M^2 K}{2}
$$

**証明**

**補題：オンラインMirror descentの基本の不等式**を，$g_k=Q^k_h(s, \cdot)$と$x_k=\pi^k_h(s, \cdot)$として適用すれば成立する．

## Three-Point Descent Lemma

参考：
* [On the Convergence Rates of Policy Gradient Methods](https://www.jmlr.org/papers/volume23/22-0056/22-0056.pdf)のLemma 6など
* [Bandit Algorithms](https://tor-lattimore.com/downloads/book/book.pdf#page=336.11)の333ページあたりにもあるよ


表記：
* $\mathcal{C} \subset \mathbf{R}^n$を閉じた凸集合
* $\phi: \mathcal{C} \to \mathbb{R}$を[プロパー](https://en.wikipedia.org/wiki/Proper_convex_function)で[closed](https://en.wikipedia.org/wiki/Closed_convex_function)な凸関数とします．
  * プロパー：少なくとも１つの$x$で$f(x) < + \infty$かつすべての$x$で$f(x) > -\infty$ならOKです．例えば$\mathcal{C}$が確率単体であり，$x \in \mathcal{C}$ について$f(x)=\langle x, Q\rangle$はプロパーですね（RLでよく出てきます）．
  * closed：各$\alpha$に対して，$\{x \in \operatorname{dom} f \mid f(x) \leq \alpha\}$が閉集合ならOKです．まあ$\operatorname{dom} f$を確率単体として撮っておけば大丈夫かも？あとは$\cup$みたいな形の関数では成立してます．
* $h$をルジャンドル形式かつ$\operatorname{rint dom} (h) \cap \mathcal{C} \neq \emptyset$な関数とします．$D_h(\cdot, \cdot)$を$h$についてのBregman divergenceとします．KL divergenceなどなら多分OK．

ここで，適当な$x \in \operatorname{rint dom} h$について，

$$
x^{+}=\operatorname{argmin}_{u \in C}\left\{\phi(u)+D_h(u, x)\right\} .
$$

とします．すると，次の２つが成立します：
* $x^{+} \in \operatorname{rint dom} h \cap C$
* 任意の$u \in \mathcal{C}$について，
  
$$
\phi\left(x^{+}\right) - \phi(u) \leq D_h(u, x)-D_h\left(u, x^{+}\right) - D_h\left(x^{+}, x\right) 
$$

## Mirror descentをKLで抑える（雑バウンド）

参考：
* [Bandit Algorithms](https://tor-lattimore.com/downloads/book/book.pdf#page=336.11)のProposition 28.6

$X \subseteq \Delta(A)$を凸集合として，$g$を$\mathbb{R}^{|A|}$上の非負のベクトルとします．
$x'=\operatorname{argmin}_{\bar{x} \in X}\langle\bar{x}, g\rangle+\frac{1}{\eta} \mathrm{KL}(\bar{x}, x)$
であれば，任意の$x^\star \in X$について，

$$
\left\langle x-x^{\star}, g\right\rangle \leq \frac{\mathrm{KL}\left(x^{\star}, x\right)-\mathrm{KL}\left(x^{\star}, x^{\prime}\right)}{\eta}+\frac{\eta}{2} \max_a \left(g_a\right)^2 .
$$

が成立します．

**証明**

上のThree point descent lemmaから

$$
\begin{aligned}
\eta \left\langle x-x^{\star}, g\right\rangle &\leq {\mathrm{KL}\left(x^{\star}, x\right)-\mathrm{KL}\left(x^{\star}, x^{\prime}\right)}+ 
\eta\left\langle x-x', g\right\rangle -\mathrm{KL}\left(x', x\right)\\
&\leq
{\mathrm{KL}\left(x^{\star}, x\right)-\mathrm{KL}\left(x^{\star}, x^{\prime}\right)}
+ 
\| x-x'\|_1 \|\eta g\|_\infty 
-\frac{1}{2}\|x - x'\|_1^2
\end{aligned}
$$
２行目はPinskerの不等式を使ってます．ここでYoungの不等式を使うと，２つの非負の実数について

$$
ab \leq \frac{1}{2} a^2 + \frac{1}{2} b^2
$$

なので，
$$
\| x-x'\|_1 \|\eta g\|_\infty -\frac{1}{2}\|x - x'\|_1^2 \leq \frac{\eta^2}{2}
\|g\|_\infty^2
$$


## Mirror descentをKLで抑える（マシなバウンド）

上と同じ条件で，
$$
\left\langle x-x^{\star}, g\right\rangle \leq \frac{\mathrm{KL}\left(x^{\star}, x\right)-\mathrm{KL}\left(x^{\star}, x^{\prime}\right)}{\eta}+{\eta} \sum_a x(a) \left(g(a)\right)^2 .
$$
が成立します．


**証明**

$$
\begin{aligned}
\left\langle x-x^{\star}, g\right\rangle &\leq \frac{\mathrm{KL}\left(x^{\star}, x\right)-\mathrm{KL}\left(x^{\star}, x^{\prime}\right)}{\eta}+ 
\left\langle x-x', g\right\rangle -\frac{1}{\eta}\mathrm{KL}\left(x', x\right)\\
\end{aligned}
$$
を上から抑えていきます．

まず，
$$\phi (x, y) 
= \sum_a x(a) \left(\ln x(a) - \ln y(a)\right)  - x(a) + y(a)$$
なる関数を考えましょう．
これは$x, y \in \Delta(A)$である限り$\mathrm{KL}(x, y) = \phi(x, a)$です．

上からバウンドしたい式の２項目と３項目に注目しましょう．
$\Delta(A)$ではなく$\mathbb{R}^A$上の最大値を考えると，
$$
\begin{aligned}
&\left\langle x-x', g\right\rangle -\frac{1}{\eta}\mathrm{KL}\left(x', x\right)\\
=&\left\langle x, g\right\rangle + \left\langle x', -g\right\rangle  -\frac{1}{\eta}\phi\left(x', x\right)\\
\leq&\left\langle x, g\right\rangle + \max_{y\in \mathbb{R}^A}\left\langle y, -g\right\rangle  -\frac{1}{\eta}\phi\left(y, x\right)\\
% =&\left\langle x, g\right\rangle + \left\langle y', -g\right\rangle  -\frac{1}{\eta}\phi\left(y', x\right)\\
\end{aligned}
$$
が成り立ちます．
<!-- 

まず，[Leverage the Average](https://arxiv.org/pdf/2003.14089)より，
$$x'=\argmax _{y \in \Delta(A)} \langle y, -g\rangle-\frac{1}{\eta} \mathrm{KL}(y \| x)=\frac{x}{Z} \exp (-\eta g)
$$
ですが，$\Delta(A)$ではなく$\mathbb{R}^A$上の最大値を考えてみましょう． -->
ここで，
$$f(y)=-\sum_{a} y(a) g(a) -\frac{1}{\eta} \sum_{a} y(a) (\ln y(a) - \ln x(a) - 1)$$
とすると，これは明らかに上に凸な関数であり，最大値が唯一存在します．
$$\frac{d f(y)}{d y_a}= -g(a) +\frac{1}{\eta} \ln x(a) - \frac{1}{\eta} \ln y(a)$$
なので，これが$0$になる場合を考えれば，
$$y'=\argmax _{y \in \mathbb{R}^A} \langle y, -g\rangle-\frac{1}{\eta} \mathrm{KL}(y \| x)=x \exp (-\eta g) $$
になり，$Z$が外せます．

ここで
$
\ln y' =  \ln x - \eta g
$
なので，
$
-g = \frac{1}{\eta}\ln y' - \frac{1}{\eta}\ln x 
$
であるから，
$$
\begin{aligned}
\langle y', -g\rangle &= 
\sum_a y'(a) \left(\frac{1}{\eta}\ln y'(a) - \frac{1}{\eta}\ln x(a) \right)
=\frac{1}{\eta}\mathrm{KL}\left(y', x\right)\\
\langle x, g\rangle &= 
\sum_a x(a) \left(-\frac{1}{\eta}\ln y'(a) + \frac{1}{\eta}\ln x(a)\right)
=\frac{1}{\eta}\mathrm{KL}\left(x, y'\right)
\end{aligned}
$$
です．よって，
$$
\begin{aligned}
&\left\langle x-x', g\right\rangle -\frac{1}{\eta}\mathrm{KL}\left(x', x\right)\\
\leq&\left\langle x, g\right\rangle +\left\langle y', -g\right\rangle  -\frac{1}{\eta}\phi\left(y', x\right)\\
\leq&
\frac{1}{\eta} \mathrm{KL}(x, y') + \frac{1}{\eta} \mathrm{KL}(y', x) 
-\frac{1}{\eta}\mathrm{KL}\left(y', x\right)
- \sum_a - y'(a) + x(a)
\\
\leq &\frac{1}{\eta}\mathrm{KL}\left(x, y'\right)
+ \sum_a - x(a) + y'(a) = 
\frac{1}{\eta}\phi(x, y')
\end{aligned}
$$
が成り立ちます．さらに，$y'=x \exp (-\eta g)$を思い出すと，
$$
\begin{aligned}
\frac{1}{\eta}\phi(x, y')
&= 
\frac{1}{\eta} \sum_a x(a) \left(\ln x(a) - \ln y'(a)\right)  - x(a) + y'(a)\\
&= \frac{1}{\eta} \sum_a x(a) \left(\eta g(a)  - 1 + \exp(-\eta g(a))\right)\\
&\leq \frac{1}{\eta} \sum_a x(a) \left(\eta g(a)\right)^2
= \eta \sum_a x(a) \left(g(a)\right)^2
\end{aligned}
$$
が成り立ちます．最後の部分では$x \geq -1$について，$e^{-x}-1+x \leq x^2$なる不等式を使いました．


<!-- 
ここで，[Leverage the Average](https://arxiv.org/pdf/2003.14089)より，$\max _{\pi \in \Delta_{\mathcal{A}}^S}(\langle\pi, q\rangle-\lambda \mathrm{KL}(\pi \| \mu))=\lambda \ln \left\langle 1, \exp \frac{q+\lambda \ln \mu}{\lambda}\right\rangle$なので，
$$
\max_y \left\langle y, -g\right\rangle 
-\frac{1}{\eta}\mathrm{KL}\left(y, x\right)
= 
\frac{1}{\eta} \ln \sum_{a} x(a) \exp\left(-\eta g(a)\right)
\geq 
-\sum_{a} x(a) g(a)
$$
です．最後のはJensenの不等式です（$\ln$は上に凸な関数なので）． -->

## エントロピー正則化付きをKLで抑える

参考：[A Policy Gradient Primal-Dual Algorithm for Constrained MDPs with Uniform PAC Guarantees](https://arxiv.org/abs/2401.17780)のLemma 8．

上のやつを利用するとバウンドできます．

$\ell \in \mathbb{R}_{+}^A, x \in \Delta(\mathbf{A}), 1 \geq \eta>0$, $1 \geq \tau \geq 0$, について，

$$
x^{\prime}=\underset{\tilde{x} \in \Delta(\mathbf{A})}{\arg \min }\left\{\sum_{a \in \mathcal{A}} \tilde{x}_a\left(\ell_a+\tau \ln x_a\right)+\frac{1}{\eta} \mathrm{KL}[\tilde{x}, x]\right\}
$$

とします．このとき，任意の$u \in \Delta(A)$について

$$
\sum_{a \in \mathbf{A}}\left(x_a-u_a\right)\left(\ell_a+\tau \ln x_a\right) \leq \frac{\mathrm{KL}[u, x]-\mathrm{KL}\left[u, x^{\prime}\right]}{\eta}+\eta \sum_a x_a \ell_a^2+\eta \tau^2 A^{\eta \tau}\left(\frac{2}{1-\eta \tau}-1+\ln A\right)^2
$$

が成立します．

