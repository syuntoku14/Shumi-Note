# Shumi-Note

## 制作方針

* 勉強のアウトプット用にまとめているJupyter notebookです。[notebooks](notebooks/)以下に色々まとまっています。
* 全てのnotebookは独立させています。管理もしやすいので嬉しいですね。
* その日の気分でクオリティが左右されます
* 「なぜその内容を学ぶと嬉しいのか？」がなるべく分かるように書いています。教育用途でも使えたらいいなって気持ち。


---

## インストール

poetryを使ってください。

```bash
git clone git@github.com:syuntoku14/Shumi-Note.git && cd Shumi-Note
poetry install
```
---

## 日付順のNotebook一覧

* 内容のチョイスは僕の趣味です。
( 内容は勉強中にまとめているので必ずしも正しいとは限りません。誤りは見つけ次第直します。
* 内容が怪しいやつ（Notationの不備など）はTODOがついてます。
* 実装ではしばしば高速化のためにjaxを使用してます。だいたいnumpyと一緒ですが、高速に実験できるので便利です。 (これからRLの研究をする人はjaxも身につけることをおすすめします。)
* NDA的にここに出せないやつは****になってます。（出せるようになったらここにも現れるかも）

1. (2023/1/18) Linear MDPについての説明と実験: [notebooks/linearMDP.ipynb](notebooks/linearMDP.ipynb)
2. (2023/1/21) 測度論的確率論の導入（TODO）: [notebooks/measure_theoretic_probability.ipynb](notebooks/measure_theoretic_probability.ipynb)
3. (2023/1/26) 確率過程の説明（TODO）: [notebooks/probability_process.ipynb](notebooks/probability_process.ipynb)
4. (2023/1/28) ルベーグ積分の説明: [notebooks/lebesgue_integral.ipynb](notebooks/lebesgue_integral.ipynb)
5. (2023/1/28) 上極限、下極限の説明: [notebooks/liminf_limsup.ipynb](notebooks/liminf_limsup.ipynb)
6. (2023/1/29) 極値分布の説明: [notebooks/extreme_value_distribution.ipynb](notebooks/extreme_value_distribution.ipynb)
7. (2023/1/29) 特性関数の説明: [notebooks/characteristic_function.ipynb](notebooks/characteristic_function.ipynb)
8. (2023/1/29) 確率積分の説明（TODO）: [notebooks/stochastic_integration.ipynb](notebooks/stochastic_integration.ipynb)
9. (2023/1/29) バンディットアルゴリズムの基本: [notebooks/bandit_algorithms.ipynb](notebooks/bandit_algorithms.ipynb)
10. (2023/1/30) テイラーの定理: [notebooks/taylor_theorem.ipynb](notebooks/taylor_theorem.ipynb)
11. (2023/1/31) 伊藤積分の説明 & 確率微分方程式の数値シミュレーション（TODO）: [notebooks/stochastic_integration.ipynb](notebooks/stochastic_integration.ipynb)
12. (2023/2/1) Girsanovの定理: [notebooks/stochastic_integration.ipynb](notebooks/stochastic_integration.ipynb)
13. (2023/2/4) ガウス過程回帰: [notebooks/gp_regression.ipynb](notebooks/gp_regression.ipynb)
14. (2023/2/5) 敵対的バンディット（TODO）: [notebooks/bandit_algorithms.ipynb](notebooks/bandit_algorithms.ipynb)
15. (2023/2/5) マルチステップ強化学習 (On-policy推定編): [notebooks/multi_step_RL.ipynb](notebooks/multi_step_RL.ipynb)
16. (2023/2/6) マルチステップ強化学習 (Off-policy推定編): [notebooks/multi_step_RL.ipynb](notebooks/multi_step_RL.ipynb)
17. (2023/2/6) マルチステップ強化学習 (マルチステップ制御編): [notebooks/multi_step_RL.ipynb](notebooks/multi_step_RL.ipynb)
18. (2023/2/7) MDPについて (Garnet MDP): [notebooks/Markov_Decision_Process.ipynb](notebooks/Markov_Decision_Process.ipynb)
19. (2023/2/8) 文脈付きバンディット (TODO): [notebooks/contextual_bandit.ipynb](notebooks/contextual_bandit.ipynb)
21. (2023/2/9) 線形バンディット: [notebooks/contextual_bandit.ipynb](notebooks/contextual_bandit.ipynb)
22. (2023/2/10) 適合価値反復法: [notebooks/fitted_Q_iteration.ipynb](notebooks/fitted_Q_iteration.ipynb)
23. (2023/2/12) Generalized RL (適合Q学習などの一般化): [notebooks/generalied_RL.ipynb](notebooks/generalized_RL.ipynb)
24. (2023/2/13) Generalized RL (確率的な作用素で一般化): [notebooks/generalied_RL.ipynb](notebooks/generalized_RL.ipynb)
25. (2023/2/14~17) マルチステップRLのスライド: [notebooks/Multi_step_RL.pdf](notebooks/Multi_step_RL.pdf)
26. (2023/2/17) 方策勾配法 (途中): [notebooks/policy_gradient.ipynb](notebooks/policy_gradient.ipynb)
27. (2023/2/19) 方策勾配法 (マルチステップRL): [notebooks/policy_gradient.ipynb](notebooks/policy_gradient.ipynb)
28. (2023/2/20~21) Transformer: [notebooks/transformer.ipynb](notebooks/transformer.ipynb)
29. (2023/2/22) Reward Free RL: [notebooks/reward_free_RL.ipynb](notebooks/reward_free_RL.ipynb)
30. (2023/2/23) 教育用強化学習修行Notebook (行列形式の動的計画法編): [notebooks/exercise_RL.ipynb](notebooks/exercise_RL.ipynb)
31. (2023/2/23) Reward Free RL (RF-EXPRESS): [notebooks/reward_free_RL.ipynb](notebooks/reward_free_RL.ipynb)
32. (2023/2/24) **** : ****.ipynb
33. (2023/2/24) Self-Normalized Bound for Vector Valued Martingales (途中): [notebooks/improved_linear_bandit.ipynb](notebooks/improved_linear_bandit.ipynb) 
34. (2023/2/25) YadokoriとDaniのバンディットアルゴリズムの比較: [notebooks/improved_linear_bandit.ipynb](notebooks/improved_linear_bandit.ipynb) 
35. (2023/2/26) 探索の理論 (UCB編): [notebooks/UCB_regret_proof.ipynb](notebooks/UCB_regret_proof.ipynb) 
<!-- 35. (2023/2/25) マルチタスクバンディット: [notebooks/improved_linear_bandit.ipynb](notebooks/improved_linear_bandit.ipynb)  -->

---

## 分野別のNotebook一覧

### 確率論入門

* (2023/1/21) 測度論的確率論の導入: [notebooks/measure_theoretic_probability.ipynb](notebooks/measure_theoretic_probability.ipynb)
* (2023/1/26) 確率過程の説明: [notebooks/probability_process.ipynb](notebooks/probability_process.ipynb)
* (2023/1/28) ルベーグ積分の説明: [notebooks/lebesgue_integral.ipynb](notebooks/lebesgue_integral.ipynb)
* (2023/1/28) 上極限、下極限の説明: [notebooks/liminf_limsup.ipynb](notebooks/liminf_limsup.ipynb)
* (2023/1/29) 極値分布の説明: [notebooks/extreme_value_distribution.ipynb](notebooks/extreme_value_distribution.ipynb)
* (2023/1/29) 特性関数の説明: [notebooks/characteristic_function.ipynb](notebooks/characteristic_function.ipynb)
* (2023/1/29) 確率積分の説明（TODO）: [notebooks/stochastic_integration.ipynb](notebooks/stochastic_integration.ipynb)
* (2023/1/31) 伊藤積分の説明 & 確率微分方程式の数値シミュレーション: [notebooks/stochastic_integration.ipynb](notebooks/stochastic_integration.ipynb)
* (2023/2/1) Girsanovの定理: [notebooks/stochastic_integration.ipynb](notebooks/stochastic_integration.ipynb)
* (2023/2/4) ガウス過程回帰: [notebooks/gp_regression.ipynb](notebooks/gp_regression.ipynb)

### バンディット

* (2023/1/29) バンディットアルゴリズムの基本: [notebooks/bandit_algorithms.ipynb](notebooks/bandit_algorithms.ipynb)
* (2023/2/5) 敵対的バンディット: [notebooks/bandit_algorithms.ipynb](notebooks/bandit_algorithms.ipynb)
* (2023/2/8) 文脈付きバンディット: [notebooks/contextual_bandit.ipynb](notebooks/contextual_bandit.ipynb)
* (2023/2/9) 線形バンディット: [notebooks/contextual_bandit.ipynb](notebooks/contextual_bandit.ipynb)
* (2023/2/24) Self-Normalized Bound for Vector Valued Martingales: [notebooks/improved_linear_bandit.ipynb](notebooks/improved_linear_bandit.ipynb) 
* (2023/2/25) YadokoriとDaniのバンディットアルゴリズムの比較: [notebooks/improved_linear_bandit.ipynb](notebooks/improved_linear_bandit.ipynb) 
* (2023/2/26) 探索の理論 (UCB編): [notebooks/UCB_regret_proof.ipynb](notebooks/UCB_regret_proof.ipynb) 

### 強化学習

* (2023/1/18) Linear MDPについての説明と実験: [notebooks/linearMDP.ipynb](notebooks/linearMDP.ipynb)
* (2023/2/5) マルチステップ強化学習 (On-policy推定編): [notebooks/multi_step_RL.ipynb](notebooks/multi_step_RL.ipynb)
* (2023/2/6) マルチステップ強化学習 (Off-policy推定編): [notebooks/multi_step_RL.ipynb](notebooks/multi_step_RL.ipynb)
* (2023/2/6) マルチステップ強化学習 (マルチステップ制御編): [notebooks/multi_step_RL.ipynb](notebooks/multi_step_RL.ipynb)
* (2023/2/7) MDPについて (Garnet MDP): [notebooks/Markov_Decision_Process.ipynb](notebooks/Markov_Decision_Process.ipynb)
* (2023/2/10) 適合価値反復法: [notebooks/fitted_Q_iteration.ipynb](notebooks/fitted_Q_iteration.ipynb)
* (2023/2/12) Generalized RL (適合Q学習などの一般化): [notebooks/generalied_RL.ipynb](notebooks/generalized_RL.ipynb)
* (2023/2/13) Generalized RL (確率的な作用素で一般化): [notebooks/generalied_RL.ipynb](notebooks/generalized_RL.ipynb)
* (2023/2/14~17) マルチステップRLのスライド: [notebooks/Multi_step_RL.pdf](notebooks/Multi_step_RL.pdf)
* (2023/2/19) 方策勾配法 (マルチステップRL): [notebooks/policy_gradient.ipynb](notebooks/policy_gradient.ipynb)
* (2023/2/22) Reward Free RL: [notebooks/reward_free_RL.ipynb](notebooks/reward_free_RL.ipynb)
* (2023/2/23) 教育用強化学習修行Notebook (行列形式の動的計画法編): [notebooks/exercise_RL.ipynb](notebooks/exercise_RL.ipynb)
* (2023/2/23) Reward Free RL (RF-EXPRESS): [notebooks/reward_free_RL.ipynb](notebooks/reward_free_RL.ipynb)

### その他機械学習
* (2023/2/20~21) Transformer: [notebooks/transformer.ipynb](notebooks/transformer.ipynb)

### その他数学

* (2023/1/30) テイラーの定理: [notebooks/taylor_theorem.ipynb](notebooks/taylor_theorem.ipynb)
