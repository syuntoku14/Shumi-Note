## 制約付きMDP系の便利な補題

### 制約付き凸最適化

参考：
* [Exploration-Exploitation in Constrained MDPs](https://arxiv.org/abs/2003.02189)のAppendix G

準備：

次の制約付き最適化を考えましょう．

$$
f_{\mathrm{opt}}=\min _{\mathbf{x} \in X}\{f(\mathbf{x}): \mathbf{g}(\mathbf{x}) \leq \mathbf{0}, \mathbf{A} \mathbf{x}+\mathbf{b}=\mathbf{0}\}
$$

ここで，$\mathbf{g}(\mathbf{x}):=\left(g_1(\mathbf{x}), . ., g_I(\mathbf{x})\right)^T$と$f, g_1, . ., g_m: \mathbb{E} \rightarrow(-\infty, \infty)$は凸な実数関数です．また，$\mathbf{A} \in \mathbb{R}^{p \times n}, \mathbf{b} \in \mathbb{R}^p$とします．

これに対して，感度関数を

$$
v(\mathbf{u}, \mathbf{t})=\min _{\mathbf{x} \in X}\{f(\mathbf{x}): \mathbf{g}(\mathbf{x}) \leq \mathbf{u}, \mathbf{A} \mathbf{x}+\mathbf{b}=\mathbf{t}\}
$$

とします．
また，双対関数を

$$
q(\lambda, \mu)=\min _{x \in X}\left\{L(\mathbf{x}, \lambda, \mu)=f(\mathbf{x})+\lambda^T \mathbf{g}(\mathbf{x})+\mu^T(\mathbf{A} \mathbf{x}+\mathbf{b})\right\}
$$

として（$\lambda \in \mathbb{R}_{+}^m, \mu \in \mathbb{R}^p$です．），双対問題を

$$
q_{\mathrm{opt}}=\max _{\lambda \in \mathbb{R}_{+}^m, \mu \in \mathbb{R}^p}\{q(\lambda, \mu):(\lambda, \mu) \in \operatorname{dom}(-q)\}
$$

とします．ここで，$\operatorname{dom}(-q)=\left\{(\lambda, \mu) \in \mathbb{R}_{+}^m, \mu \in \mathbb{R}^p: q(\lambda, \mu)>-\infty\right\}$です．

---

仮定：

最適値は有限であり，$g(\overline{\mathbf{x}})<0$および$\mathbf{A} \widehat{\mathbf{x}}+\mathbf{b}=0$であるような$\bar{x}$と$\widehat{\mathbf{x}} \in \operatorname{ri}(X)$が存在するとします．
ここで，$\operatorname{ri}(X)$は$X$の相対的内部です．

---

**定理**

$(\lambda^*, \mu^*)$は次を満たし，またそのときに限り最適解です．

$$
-\left(\lambda^*, \mu^*\right) \in \partial v(\mathbf{0}, \mathbf{0})
$$

---

**定理**

$2\left\|\lambda^*\right\|_1 \leq \rho$とします．
$\widetilde{\mathbf{x}}$ は$\mathbf{A} \widetilde{\mathbf{x}}+\mathbf{b}=0$
および
$$
f(\widetilde{\mathbf{x}})-f_{o p t}+\rho\left\|[g(\widetilde{\mathbf{x}})]_{+}\right\|_{\infty} \leq \delta,
$$
とします．このとき，

$$
\left\|[g(\widetilde{\mathbf{x}})]_{+}\right\|_{\infty} \leq \frac{\delta}{\rho}
$$

が成立します．

### 制約付きMDP

表記（[Last-Iterate Convergent Policy Gradient Primal-Dual Methods for Constrained MDPs](https://arxiv.org/abs/2306.11700)参照）：

* 制約付きMDP：$\underset{\pi \in \Pi}{\operatorname{maximize}} V_r^\pi(\rho) \quad \text { subject to } V_u^\pi(\rho) \geq b$：
* $g:=u-(1-\gamma) b$とする
* $L(\pi, \lambda):=V_r^\pi(\rho)+\lambda V_g^\pi(\rho)$
* ラグランジュ形式：$\underset{\pi \in \Pi}{\operatorname{maximize}} \underset{\lambda \in[0, \infty]}{\operatorname{minimize}} V_{r+\lambda g}^\pi(\rho)$
    * 鞍点$(\pi', \lambda')$：$V_{r+\lambda^{\prime} g}^\pi(\rho) \leq V_{r+\lambda^{\prime} g}^{\pi^{\prime}}(\rho) \leq V_{r+\lambda g}^{\pi^{\prime}}(\rho)$
* 主問題：$V_P^\pi(\rho):=\inf _{\lambda \in[0, \infty]} V_{r+\lambda g}^\pi(\rho)$
* 双対問題：$V_D^\lambda(\rho):=\max _{\pi \in \Pi} V_{r+\lambda g}^\pi(\rho)$

---

**補題：強双対性**

参考：
* [Safe Policies for Reinforcement Learning via Primal-Dual Methods](https://arxiv.org/abs/1911.09101)のTheorem 3

$$
V_P^{\pi^{\star}}(\rho)=V_D^{\lambda^{\star}}(\rho)
$$

---

**補題：未定乗数の範囲**

参考：
* [Natural Policy Gradient Primal-Dual Method for Constrained Markov Decision Processes](https://proceedings.neurips.cc/paper/2020/hash/5f7695debd8cde8db5abcb9f161b49ea-Abstract.html)のLemma 1

次のFeasibilityが成立するとする：$\bar{\pi} \in \Pi$ and $\xi>0$ such that $V_g^{\bar{\pi}}(\rho) \geq \xi$．
このとき，

$$
\lambda^{\star} \in\left[0,\left(V_r^{\bar{\pi}}-V_r^{\pi^{\star}}\right) / \xi\right]
$$

---