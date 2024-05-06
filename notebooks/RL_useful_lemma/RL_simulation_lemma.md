## Simulation Lemma系の便利な補題

### 正則化なし

#### Extended Value Difference

参考：
* [Exploration-Exploitation in Constrained MDPs](https://arxiv.org/abs/2003.02189)の補題34など

表記：
* 方策：$\pi, \pi'$
* MDP：$\mathcal{M}=(\mathcal{S}, \mathcal{A}, \{p_h\}_{h=1}^H, \{r_h\}_{h=1}^H)$と$\mathcal{M}'=(\mathcal{S}, \mathcal{A}, \{p_h'\}_{h=1}^H, \{r_h'\}_{h=1}^H)$
* $\widehat{Q}_h^\pi(s, a; r, p)$を$\mathcal{M}$でのQ関数の近似
* $\widehat{V}_h^\pi(s; r, p)=\left\langle \widehat{Q}_h^\pi(s, \cdot; r, p), \pi_h(\cdot \mid s)\right\rangle$

のとき，

$$
\begin{aligned}
\widehat{V}_h^\pi(s; r, p)
-
{V}_h^{\pi'}(s; r', p')
=
&\sum^{H}_{h=1}\mathbb{E}\left[
\left\langle \widehat{Q}_h^\pi(s_h, \cdot; r, p), \pi_h'(\cdot \mid s_h) - \pi_h(\cdot \mid s_h)\right\rangle
\mid s_1, \pi', p'
\right]
+ \\
&\sum^{H}_{h=1}\mathbb{E}\left[
\widehat{Q}_h^\pi(s_h, a_h; r, p) - r_h'(s_h, a_h) - p_h'(\cdot \mid s_h, a_h)\widehat{V}_{h+1}^\pi(\cdot; r, p) \mid s_1, \pi', p'
\right]
\end{aligned}
$$


### エントロピー正則化

#### Soft performance difference lemma

参考：
* [On the Global Convergence Rates of Softmax Policy Gradient Methods](https://arxiv.org/abs/2005.06392)のLemma 25など

表記：
* ソフト価値：$\tilde{V}^\pi(\rho):=V^\pi(\rho)+\tau \cdot \mathbb{H}(\rho, \pi)$
* エントロピー価値：$\mathbb{H}(\rho, \pi):=\underset{\substack{s_0 \sim \rho, a_t \sim \pi\left(\cdot \mid s_t\right) \\ s_{t+1} \sim \mathcal{P}\left(\cdot \mid s_t, a_t\right)}}{\mathbb{E}}\left[\sum_{t=0}^{\infty}-\gamma^t \log \pi\left(a_t \mid s_t\right)\right]$
* Occupancy measure：$d_{s_0}^\pi(s):=(1-\gamma) \sum_{t=0}^{\infty} \gamma^t \operatorname{Pr}\left(s_t=s \mid s_0, \pi, \mathcal{P}\right)$

---

任意の方策$\pi$と$\pi'$について，
$$
\tilde{V}^{\pi^{\prime}}(\rho)-\tilde{V}^\pi(\rho)=\frac{1}{1-\gamma} \sum_s d_\rho^\pi(s) \cdot\left[\sum_a\left(\pi^{\prime}(a \mid s)-\pi(a \mid s)\right) \cdot\left[\tilde{Q}^{\pi^{\prime}}(s, a)-\tau \log \pi^{\prime}(a \mid s)\right]+\tau \cdot D_{\mathrm{KL}}\left(\pi(\cdot \mid s) \| \pi^{\prime}(\cdot \mid s)\right)\right] .
$$
が成立します．

**証明**

$$
\begin{aligned}
\tilde{V}^{\pi^{\prime}}(s)-\tilde{V}^\pi(s)&=\sum_a \pi^{\prime}(a \mid s) \cdot\left[\tilde{Q}^{\pi^{\prime}}(s, a)-\tau \log \pi^{\prime}(a \mid s)\right]-\sum_a \pi(a \mid s) \cdot\left[\tilde{Q}^\pi(s, a)-\tau \log \pi(a \mid s)\right]\\
&=\sum_a\left(\pi^{\prime}(a \mid s)-\pi(a \mid s)\right) \cdot\left[\tilde{Q}^{\pi^{\prime}}(s, a)-\tau \log \pi^{\prime}(a \mid s)\right]+\sum_a \pi(a \mid s) \cdot\left[\tilde{Q}^{\pi^{\prime}}(s, a)-\tau \log \pi^{\prime}(a \mid s)-\tilde{Q}^\pi(s, a)+\tau \log \pi(a \mid s)\right]\\
&=\sum_a\left(\pi^{\prime}(a \mid s)-\pi(a \mid s)\right) \cdot\left[\tilde{Q}^{\pi^{\prime}}(s, a)-\tau \log \pi^{\prime}(a \mid s)\right]+\tau D_{\mathrm{KL}}\left(\pi(\cdot \mid s) \| \pi^{\prime}(\cdot \mid s)\right)+\gamma \sum_a \pi(a \mid s) \sum_{s^{\prime}} \mathcal{P}\left(s^{\prime} \mid s, a\right) \cdot\left[\tilde{V}^{\pi^{\prime}}\left(s^{\prime}\right)-\tilde{V}^\pi\left(s^{\prime}\right)\right]
\end{aligned}
$$
２行目は$\pm\sum_{a} \pi(a \mid s)\left[\tilde{Q}^{\pi^{\prime}}(s, a)-\tau \log \pi^{\prime}(a \mid s)\right]$してます．


ここで，最後の項に$\tilde{V}^{\pi^{\prime}}(s')-\tilde{V}^\pi(s')$が登場したことに注意しましょう．後は再帰的に展開すれば，これは報酬が

$$
\sum_a\left(\pi^{\prime}(a \mid s)-\pi(a \mid s)\right) \cdot\left[\tilde{Q}^{\pi^{\prime}}(s, a)-\tau \log \pi^{\prime}(a \mid s)\right]+\tau D_{\mathrm{KL}}\left(\pi(\cdot \mid s) \| \pi^{\prime}(\cdot \mid s)\right)
$$

である場合に$\pi$で動き回った価値関数とみなせます．よって，Occupancy measureを使って

$$
=\frac{1}{1-\gamma} \sum_{s^{\prime}} d_s^\pi\left(s^{\prime}\right) \cdot\left[\sum_{a^{\prime}}\left(\pi^{\prime}\left(a^{\prime} \mid s^{\prime}\right)-\pi\left(a^{\prime} \mid s^{\prime}\right)\right) \cdot\left[\tilde{Q}^{\pi^{\prime}}\left(s^{\prime}, a^{\prime}\right)-\tau \log \pi^{\prime}\left(a^{\prime} \mid s^{\prime}\right)\right]+\tau \cdot D_{\mathrm{KL}}\left(\pi\left(\cdot \mid s^{\prime}\right) \| \pi^{\prime}\left(\cdot \mid s^{\prime}\right)\right)\right]
$$
が成り立ちます．

---

ひっくり返した版も示しておきます．
任意の方策$\pi$と$\pi'$について，
$$
\tilde{V}^{\pi^{\prime}}(\rho)-\tilde{V}^\pi(\rho)=\frac{1}{1-\gamma} \sum_s d_\rho^{\pi'}(s) \cdot\left[\sum_a\left(\pi^{\prime}(a \mid s)-\pi(a \mid s)\right) \cdot\left[\tilde{Q}^{\pi}(s, a)-\tau \log \pi(a \mid s)\right]-\tau \cdot D_{\mathrm{KL}}\left(\pi'(\cdot \mid s) \| \pi(\cdot \mid s)\right)\right] .
$$
が成立します．

**証明**

$$
\begin{aligned}
\tilde{V}^{\pi^{\prime}}(s)-\tilde{V}^\pi(s)&=\sum_a \pi^{\prime}(a \mid s) \cdot\left[\tilde{Q}^{\pi^{\prime}}(s, a)-\tau \log \pi^{\prime}(a \mid s)\right]-\sum_a \pi(a \mid s) \cdot\left[\tilde{Q}^\pi(s, a)-\tau \log \pi(a \mid s)\right]
\end{aligned}
$$
右辺で$\pm\sum_{a} \pi'(a \mid s)\left[\tilde{Q}^{\pi}(s, a)-\tau \log \pi(a \mid s)\right]$すると，

$$
\begin{aligned}
&=\sum_a\left(\pi^\prime(a \mid s)-\pi(a \mid s)\right) \cdot\left[\tilde{Q}^{\pi}(s, a)-\tau \log \pi(a \mid s)\right]+\sum_a \pi'(a \mid s) \cdot\left[\tilde{Q}^{\pi^{\prime}}(s, a)-\tau \log \pi^{\prime}(a \mid s)-\tilde{Q}^\pi(s, a)+\tau \log \pi(a \mid s)\right]\\
&=\sum_a\left(\pi^{\prime}(a \mid s)-\pi(a \mid s)\right) \cdot\left[\tilde{Q}^{\pi}(s, a)-\tau \log \pi(a \mid s)\right]-\tau D_{\mathrm{KL}}\left(\pi'(\cdot \mid s) \| \pi(\cdot \mid s)\right)+\gamma \sum_a \pi'(a \mid s) \sum_{s^{\prime}} \mathcal{P}\left(s^{\prime} \mid s, a\right) \cdot\left[\tilde{V}^{\pi^{\prime}}\left(s^{\prime}\right)-\tilde{V}^\pi\left(s^{\prime}\right)\right]\\
&=\frac{1}{1-\gamma} \sum_{s^{\prime}} d_s^{\pi'}\left(s^{\prime}\right) \cdot\left[\sum_{a^{\prime}}\left(\pi^{\prime}\left(a^{\prime} \mid s^{\prime}\right)-\pi\left(a^{\prime} \mid s^{\prime}\right)\right) \cdot\left[\tilde{Q}^{\pi}\left(s^{\prime}, a^{\prime}\right)-\tau \log \pi\left(a^{\prime} \mid s^{\prime}\right)\right]-\tau \cdot D_{\mathrm{KL}}\left(\pi'\left(\cdot \mid s^{\prime}\right) \| \pi\left(\cdot \mid s^{\prime}\right)\right)\right]
\end{aligned}
$$




#### Soft sub-optimality

参考（表記も上と同じ）：
* [On the Global Convergence Rates of Softmax Policy Gradient Methods](https://arxiv.org/abs/2005.06392)のLemma 25など

まず，最適価値関数は次を満たします
* 証明は[Bridging the Gap Between Value and Policy Based Reinforcement Learning](https://proceedings.neurips.cc/paper_files/paper/2017/hash/facf9f743b083008a894eee7baa16469-Abstract.html)のTheorem 1

$$
\begin{aligned}
& \pi_\tau^*(a \mid s)=\exp \left\{\left(\tilde{Q}^{\pi_\tau^*}(s, a)-\tilde{V}^{\pi_\tau^*}(s)\right) / \tau\right\} \\
& \tilde{V}^{\pi_\tau^*}(s)=\tau \log \sum_a \exp \left\{\tilde{Q}^{\pi_\tau^*}(s, a) / \tau\right\} .
\end{aligned}
$$

---

任意の方策$\pi$について，次が成立します：

$$
\tilde{V}^{\pi_\tau^*}(\rho)-\tilde{V}^\pi(\rho)=\frac{1}{1-\gamma} \sum_s\left[d_\rho^\pi(s) \cdot \tau \cdot D_{\mathrm{KL}}\left(\pi(\cdot \mid s) \| \pi_\tau^*(\cdot \mid s)\right)\right]
$$

**証明**

定義より，まず次が成立します：
$$
\tau \log \pi_\tau^*(a \mid s)=\tilde{Q}^{\pi_\tau^*}(s, a)-\tilde{V}^{\pi_\tau^*}(s) .
$$

続いて，上でやったsoft performance difference lemmaより，

$$
\begin{aligned}
\tilde{V}^{\pi_\tau^*}(s)-\tilde{V}^\pi(s)&=\frac{1}{1-\gamma} \sum_{s^{\prime}} d_s^\pi\left(s^{\prime}\right) \cdot\left[\sum_{a^{\prime}}\left(\pi_\tau^*\left(a^{\prime} \mid s^{\prime}\right)-\pi\left(a^{\prime} \mid s^{\prime}\right)\right) \cdot\left[\tilde{Q}^{\pi_\tau^*}\left(s^{\prime}, a^{\prime}\right)-\tau \log \pi_\tau^*\left(a^{\prime} \mid s^{\prime}\right)\right]+\tau \cdot D_{\mathrm{KL}}\left(\pi\left(\cdot \mid s^{\prime}\right) \| \pi_\tau^*\left(\cdot \mid s^{\prime}\right)\right)\right]\\
& =\frac{1}{1-\gamma} \sum_{s^{\prime}} d_s^\pi\left(s^{\prime}\right) \cdot\left[\sum_{a^{\prime}}\left(\pi_\tau^*\left(a^{\prime} \mid s^{\prime}\right)-\pi\left(a^{\prime} \mid s^{\prime}\right)\right) \cdot \tilde{V}^{\pi_\tau^*}\left(s^{\prime}\right)+\tau \cdot D_{\mathrm{KL}}\left(\pi\left(\cdot \mid s^{\prime}\right) \| \pi_\tau^*\left(\cdot \mid s^{\prime}\right)\right)\right] \\
& =\frac{1}{1-\gamma} \sum_{s^{\prime}} d_s^\pi\left(s^{\prime}\right) \cdot\left[(1-1) \cdot \tilde{V}^{\pi_\tau^*}\left(s^{\prime}\right)+\tau \cdot D_{\mathrm{KL}}\left(\pi\left(\cdot \mid s^{\prime}\right) \| \pi_\tau^*\left(\cdot \mid s^{\prime}\right)\right)\right] \\
& =\frac{1}{1-\gamma} \sum_{s^{\prime}}\left[d_s^\pi\left(s^{\prime}\right) \cdot \tau \cdot D_{\mathrm{KL}}\left(\pi\left(\cdot \mid s^{\prime}\right) \| \pi_\tau^*\left(\cdot \mid s^{\prime}\right)\right)\right] .
\end{aligned}
$$

---

ひっくり返した版はPerformance difference以上のことは言えないかもです．
上でやったsoft performance difference lemmaより，

$$
\begin{aligned}
0 \leq& \tilde{V}^{\pi^{\star}_\tau}(\rho)-\tilde{V}^\pi(\rho)\\
=&\frac{1}{1-\gamma} \sum_s d_\rho^{\pi^\star_\tau}(s) \cdot\left[\sum_a\left(\pi^{\star}_\tau(a \mid s)-\pi(a \mid s)\right) \cdot\left[\tilde{Q}^{\pi}(s, a)-\tau \log \pi(a \mid s)\right]-\tau \cdot D_{\mathrm{KL}}\left(\pi^\star_\tau(\cdot \mid s) \| \pi(\cdot \mid s)\right)\right]\\
\leq &\frac{1}{1-\gamma} \sum_s d_\rho^{\pi^\star_\tau}(s) \cdot\left[\sum_a\left(\pi^{\star}_\tau(a \mid s)-\pi(a \mid s)\right) \cdot\left[\tilde{Q}^{\pi}(s, a)-\tau \log \pi(a \mid s)\right]\right]\\
\end{aligned}
$$

です．ここで$\pi$が
$$
\tau \log \pi(a \mid s)=\tilde{Q}^{\pi}(s, a)-\tilde{V}^{\pi}(s)
$$
を満たすと，

$$
0 \leq 
\tilde{V}^{\pi^{\star}_\tau}(\rho)-\tilde{V}^\pi(\rho)\leq 0
$$
になるので，これは　$\pi$が最適方策であることを示します．


### Natural policy gradientでのsub-optimality gap

$\pi_t$から$\pi_{t+1}$への更新を次で実現する場合について考えましょう．

$$
\begin{aligned}
\pi^{(t+1)}(a \mid s)&=\frac{1}{Z^{(t)}(s)}\left(\pi^{(t)}(a \mid s)\right)^{1-\frac{\eta \tau}{1-\gamma}} \exp \left(\frac{\eta Q_\tau^{\pi^{(t)}}(s, a)}{1-\gamma}\right)\\
&=\underset{\pi(\cdot \mid s) \in \dot{\Delta}(A)}{\operatorname{argmax}}\left\{\sum_a \pi(a \mid s) Q_{\tau}^{\pi^{(t)}}(s, a)-\frac{1}{\eta} \mathrm{KL}\left(\pi(\cdot \mid s), \pi_t(\cdot \mid s)\right)
- \tau\log \pi(a \mid s)
\right\}
\end{aligned}
$$

これは[mirror descentのバウンド]()