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


## Mirror descentをKLで抑える

参考：[Uncoupled and Convergent Learning in Two-Player Zero-Sum Markov Games with Bandit Feedback](https://arxiv.org/abs/2303.02738)のLemma 11．

$X \subseteq \Delta(A)$を凸集合として，$g$を$\mathbb{R}^{|A|}$上の非負のベクトルとします．
$x'=\operatorname{argmin}_{\bar{x} \in X}\langle\bar{x}, g\rangle+\frac{1}{\eta} \mathrm{KL}(\bar{x}, x)$
であれば，任意の$x^\star \in X$について，

$$
\left\langle x-x^{\star}, g\right\rangle \leq \frac{\mathrm{KL}\left(x^{\star}, x\right)-\mathrm{KL}\left(x^{\star}, x^{\prime}\right)}{\eta}+\eta \sum_{a \in A} x_a\left(g_a\right)^2 .
$$

が成立します．


## エントロピー正則化付きをKLで抑える

参考：[A Policy Gradient Primal-Dual Algorithm for Constrained MDPs with Uniform PAC Guarantees](https://arxiv.org/abs/2401.17780)のLemma 8．

$\ell \in \mathbb{R}_{+}^A, x \in \Delta(\mathbf{A}), 1 \geq \eta>0$, $1 \geq \tau \geq 0$, について，

$$
x^{\prime}=\underset{\tilde{x} \in \Delta(\mathbf{A})}{\arg \min }\left\{\sum_{a \in \mathcal{A}} \tilde{x}_a\left(\ell_a+\tau \ln x_a\right)+\frac{1}{\eta} \mathrm{KL}[\tilde{x}, x]\right\}
$$

とします．このとき，任意の$u \in \Delta(A)$について

$$
\sum_{a \in \mathbf{A}}\left(x_a-u_a\right)\left(\ell_a+\tau \ln x_a\right) \leq \frac{\mathrm{KL}[u, x]-\mathrm{KL}\left[u, x^{\prime}\right]}{\eta}+\eta \sum_a x_a \ell_a^2+\eta \tau^2 A^{\eta \tau}\left(\frac{2}{1-\eta \tau}-1+\ln A\right)^2
$$

が成立します．


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
