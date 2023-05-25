# Shumi-Note

## 制作方針

* 勉強内容を[notebooks](notebooks/)にまとめてます。
* 全てのnotebookは独立させています。
* 内容は勉強中なので正しいとは限りません。内容が怪しいやつ（Notationの不備など）はTODOがついてます。
* 実装ではしばしば高速化のためにjaxを使用してます。(これからRLの研究をする人はjaxも身につけることをおすすめします。)

---

## インストール

poetryを使ってください。

```bash
git clone git@github.com:syuntoku14/Shumi-Note.git && cd Shumi-Note
poetry install
```
---

## 日付順のNotebook一覧

* NDA的にここに出せないやつは****になってます。（出せるようになったらここにも現れるかも）

1. (2023/1/18) Linear MDP: [notebooks/RL_linear_MDP.ipynb](notebooks/RL_linear_MDP.ipynb)
2. (2023/1/21) 測度論的確率論（TODO）: [notebooks/PROB_measure_theoretic_probability.ipynb](notebooks/PROB_measure_theoretic_probability.ipynb)
3. (2023/1/26) 確率過程（TODO）: [notebooks/PROB_probability_process.ipynb](notebooks/PROB_probability_process.ipynb)
4. (2023/1/28) ルベーグ積分: [notebooks/PROB_lebesgue_integral.ipynb](notebooks/PROB_lebesgue_integral.ipynb)
5. (2023/1/28) 上極限、下極限: [notebooks/PROB_liminf_limsup.ipynb](notebooks/PROB_liminf_limsup.ipynb)
6. (2023/1/29) 極値分布: [notebooks/PROB_extreme_value_distribution.ipynb](notebooks/PROB_extreme_value_distribution.ipynb)
7. (2023/1/29) 特性関数: [notebooks/PROB_characteristic_function.ipynb](notebooks/PROB_characteristic_function.ipynb)
8. (2023/1/29) 確率積分（TODO）: [notebooks/PROB_stochastic_integration.ipynb](notebooks/PROB_stochastic_integration.ipynb)
9. (2023/1/29) バンディットアルゴリズムの基本: [notebooks/BANDIT_basics.ipynb](notebooks/BANDIT_basics.ipynb)
10. (2023/1/30) テイラーの定理: [notebooks/MATH_taylor_theorem.ipynb](notebooks/MATH_taylor_theorem.ipynb)
11. (2023/1/31) 伊藤積分 & 確率微分方程式の実験（TODO）: [notebooks/PROB_stochastic_integration.ipynb](notebooks/PROB_stochastic_integration.ipynb)
12. (2023/2/1) Girsanovの定理: [notebooks/PROB_stochastic_integration.ipynb](notebooks/PROB_stochastic_integration.ipynb)
13. (2023/2/4) ガウス過程回帰: [notebooks/PROB_gp_regression.ipynb](notebooks/PROB_gp_regression.ipynb)
14. (2023/2/5) 敵対的バンディット（TODO）: [notebooks/BANDIT_basics.ipynb](notebooks/BANDIT_basics.ipynb)
15. (2023/2/5) マルチステップ強化学習 (On-policy推定編): [notebooks/RL_multi_step.ipynb](notebooks/RL_multi_step.ipynb)
16. (2023/2/6) マルチステップ強化学習 (Off-policy推定編): [notebooks/RL_multi_step.ipynb](notebooks/RL_multi_step.ipynb)
17. (2023/2/6) マルチステップ強化学習 (マルチステップ制御編): [notebooks/RL_multi_step.ipynb](notebooks/RL_multi_step.ipynb)
18. (2023/2/7) MDPについて (Garnet MDP): [notebooks/RL_Markov_Decision_Process.ipynb](notebooks/RL_Markov_Decision_Process.ipynb)
19. (2023/2/8) 文脈付きバンディット (TODO): [notebooks/BANDIT_contextual.ipynb](notebooks/BANDIT_contextual.ipynb)
20. (2023/2/9) 線形バンディット: [notebooks/BANDIT_contextual.ipynb](notebooks/BANDIT_contextual.ipynb)
21. (2023/2/10) 適合価値反復法: [notebooks/RL_fitted_Q_iteration.ipynb](notebooks/RL_fitted_Q_iteration.ipynb)
22. (2023/2/12) Generalized RL (適合Q学習などの一般化): [notebooks/generalied_RL.ipynb](notebooks/RL_generalized.ipynb)
23. (2023/2/13) Generalized RL (確率的な作用素で一般化): [notebooks/generalied_RL.ipynb](notebooks/RL_generalized.ipynb)
24. (2023/2/14~17) マルチステップRLのスライド: [slides/RL_multi_step.pdf](slides/RL_multi_step.pdf)
25. (2023/2/17) 方策勾配法 (途中): [notebooks/RL_policy_gradient.ipynb](notebooks/RL_policy_gradient.ipynb)
26. (2023/2/19) 方策勾配法 (マルチステップRL): [notebooks/RL_policy_gradient.ipynb](notebooks/RL_policy_gradient.ipynb)
27. (2023/2/20~21) Transformer: [notebooks/NN_transformer.ipynb](notebooks/NN_transformer.ipynb)
28. (2023/2/22) Reward Free RL: [notebooks/RL_reward_free.ipynb](notebooks/RL_reward_free.ipynb)
29. (2023/2/23) 教育用強化学習修行Notebook (行列形式の動的計画法編): [notebooks/RL_exercise.ipynb](notebooks/RL_exercise.ipynb)
30. (2023/2/23) Reward Free RL (RF-EXPRESS): [notebooks/RL_reward_free.ipynb](notebooks/RL_reward_free.ipynb)
31. (2023/2/24) **** : ****.ipynb
32. (2023/2/24) Self-Normalized Bound for Vector Valued Martingales (途中): [notebooks/BANDIT_linear_improved.ipynb](notebooks/BANDIT_linear_improved.ipynb) 
33. (2023/2/25) YadokoriとDaniのバンディットアルゴリズムの比較: [notebooks/BANDIT_linear_improved.ipynb](notebooks/BANDIT_linear_improved.ipynb) 
34. (2023/2/26) 探索の理論 (UCB編): [notebooks/BANDIT_UCB_regret_proof.ipynb](notebooks/BANDIT_UCB_regret_proof.ipynb) 
35. (2023/2/27-28) 探索の理論 (UCB-VI編): [notebooks/RL_UCB_VI_regret_proof.ipynb](notebooks/RL_UCB_VI_regret_proof.ipynb) 
36. (2023/2/28-3/3) **** : ****
37. (2023/3/4) 探索の理論 (UCB-VIのBernstein版): [notebooks/RL_UCB_VI_regret_proof.ipynb](notebooks/RL_UCB_VI_regret_proof.ipynb) 
38. (2023/3/4) Q学習の理論 (UCB-H編): [notebooks/RL_UCB_H_regret_proof.ipynb](notebooks/RL_UCB_H_regret_proof.ipynb) 
39. (2023/3/5) 遷移確率の推定について: [notebooks/RL_transition_estimation_proofs.ipynb](notebooks/RL_transition_estimation_proofs.ipynb) 
40. (2023/3/6) **** : ****.ipynb
41. (2023/3/7) Task-agnostic探索の理論: [notebooks/RL_task_agnostic_exploration.ipynb](notebooks/RL_task_agnostic_exploration.ipynb) 
42. (2023/3/8) ロバストMDP: [notebooks/RL_robust_MDP.ipynb](notebooks/RL_robust_MDP.ipynb) 
43. (2023/3/10) ロバストMDPの理論（モデルベース＆Generative model）: [notebooks/RL_robust_MDP.ipynb](notebooks/RL_robust_MDP.ipynb) 
44. (2023/3/12) 強化学習と線形計画問題: [notebooks/RL_as_LP.ipynb](notebooks/RL_as_LP.ipynb) 
45. (2023/3/12) 強化学習の便利な関数: [notebooks/RL_utils.ipynb](notebooks/RL_utils.ipynb) 
46. (2023/3/13) マルチステップRLのスライド（簡単版）: [slides/RL_multi_step_easy.pdf](slides/RL_multi_step_easy.pdf)
47. (2023/3/13) TODO: ロバストMDPの理論（正則化との関係）: [notebooks/RL_robust_MDP_and_regularization.ipynb](notebooks/RL_robust_MDP_and_regularization.ipynb) 
48. (2023/3/14) TODO: 模倣学習: [notebooks/RL_imitation_learning.ipynb](notebooks/RL_imitation_learning.ipynb) 
49. (2023/3/17) 最尤推定：[notebooks/PROB_maximum_likelihood.ipynb](notebooks/PROB_maximum_likelihood.ipynb)
50. (2023/3/20) 凸集合：[notebooks/CVX_convex_sets.ipynb](notebooks/CVX_convex_sets.ipynb)
51. (2023/3/21) 凸集合：[notebooks/CVX_convex_sets.ipynb](notebooks/CVX_convex_sets.ipynb)
52. (2023/3/22) 強化学習のサンプル効率の下界：[notebooks/RL_lower_bounds.ipynb](notebooks/RL_lower_bounds.ipynb)
53. (2023/3/20~2023/3/23) : 読書：[ソフトウェア見積り　人月の暗黙知を解き明かす](books/README.md)
54. (2023/3/24) **** : ****.ipynb
55. (2023/3/25) 強化学習のサンプル効率の下界（Linear Realizable編）：[notebooks/RL_lower_bounds.ipynb](notebooks/RL_lower_bounds.ipynb)
56. (2023/3/27) TODO: 強化学習とエントロピー正則化（途中）：[notebooks/RL_entropy_regularization.ipynb](notebooks/RL_entropy_regularization.ipynb)
57. (2023/3/28) 凸関数（共役関数とか）：[notebooks/CVX_convex_functions.ipynb](notebooks/CVX_convex_functions.ipynb)
58. (2023/3/29) Approximate Dynamic Programming：[notebooks/RL_approximate_dynamic_programming.ipynb](notebooks/RL_approximate_dynamic_programming.ipynb)
59. (2023/3/30) TODO: Approximate Dynamic Programming（正則化あり）：[notebooks/RL_approximate_dynamic_programming.ipynb](notebooks/RL_approximate_dynamic_programming.ipynb)
60. (2023/4/01) 最小楕円問題：[notebooks/CVX_minimum_volume_ellipsoids.ipynb](notebooks/CVX_minimum_volume_ellipsoids.ipynb)
61. (2023/4/02) 他変量関数の微分：[notebooks/MATH_multivariate_derivative.ipynb](notebooks/MATH_multivariate_derivative.ipynb)
62. (2023/4/03) 最小楕円問題のアルゴリズム：[notebooks/CVX_MVEE_algorithm.ipynb](notebooks/CVX_MVEE_algorithm.ipynb)
63. (2023/4/04) 最小楕円問題とCore-set：[notebooks/CVX_MVEE_algorithm.ipynb](notebooks/CVX_MVEE_algorithm.ipynb)
64. (2023/4/05) **** : ****.ipynb
65. (2023/4/06) **** : ****.ipynb
66. (2023/4/07) 行列と行列式（途中）: [LA_matrix_determinant.ipynb](notebooks/LA_matrix_determinant.ipynb)
67. (2023/4/07) エントロピー最大化と探索（途中）: [RL_max_ent_exploration.ipynb](notebooks/RL_max_ent_exploration.ipynb)
68. (2023/4/08) 強化学習の便利な関数（有限ホライゾン）: [notebooks/RL_utils.ipynb](notebooks/RL_utils.ipynb) 
69. (2023/4/09) 強化学習の便利な関数（探索用）: [notebooks/RL_utils.ipynb](notebooks/RL_utils.ipynb) 
70. (2023/4/09) エントロピー最大化と探索（EntGameアルゴリズム）: [RL_max_ent_exploration.ipynb](notebooks/RL_max_ent_exploration.ipynb)
71. (2023/4/10) 凸関数（Bregman Divergenceとか）：[notebooks/CVX_convex_functions.ipynb](notebooks/CVX_convex_functions.ipynb)
72. (2023/4/11) 凸関数（Projectionについて）：[notebooks/CVX_convex_functions.ipynb](notebooks/CVX_convex_functions.ipynb)
73. (2023/4/12) バンディットの便利な関数: [notebooks/BANDIT_utils.ipynb](notebooks/BANDIT_utils.ipynb) 
74. (2023/4/13) 敵対的バンディット: [notebooks/BANDIT_adversarial.ipynb](notebooks/BANDIT_adversarial.ipynb) 
75. (2023/4/14) RL Theory Book翻訳: [特徴付きMDP](https://tadashik.github.io/rltheory-jp/lecture-notes/online-rl/lec24/)
76. (2023/4/16) Fenchelの双対定理：[notebooks/CVX_convex_functions.ipynb](notebooks/CVX_convex_functions.ipynb)
77. (2023/4/17) RLと線型計画問題（方策評価）：[notebooks/RL_as_LP.ipynb](notebooks/RL_as_LP.ipynb)
78. (2023/4/19) 置換と基本行列: [notebooks/LA_matrix_determinant.ipynb](notebooks/LA_matrix_determinant.ipynb)
79. (2023/4/20) クロネッカー積: [notebooks/LA_matrix_determinant.ipynb](notebooks/LA_matrix_determinant.ipynb)
80. (2023/4/21) 行列式: [notebooks/LA_matrix_determinant.ipynb](notebooks/LA_matrix_determinant.ipynb)
81. (2023/4/22) Linear MDPでのサンプル効率の下界: [notebooks/RL_linearMDP_lower_bound.ipynb](notebooks/RL_linearMDP_lower_bound.ipynb)
82. (2023/4/26) 余因子行列: [notebooks/LA_matrix_determinant.ipynb](notebooks/LA_matrix_determinant.ipynb)
83. (2023/4/27) ロバストQ学習: [notebooks/RL_robust_Q_learning.ipynb](notebooks/RL_robust_Q_learning.ipynb)
84. (2023/4/28) ゲルシュゴリンの定理: [notebooks/LA_Gershgorin_circle_theorem.ipynb](notebooks/LA_Gershgorin_circle_theorem.ipynb)
85. (2023/4/30) 最小楕円問題と最小二乗法　：[notebooks/CVX_minimum_volume_ellipsoids.ipynb](notebooks/CVX_minimum_volume_ellipsoids.ipynb)
86. (2023/5/01 ~ 2023/5/07) ****.ipynb
87. (2023/5/08) 敵対的線形バンディット: [notebooks/BANDIT_adversarial_linear.ipynb](notebooks/BANDIT_adversarial_linear.ipynb) 
88. (2023/5/09) CPIのスライドの追加: [slides/RL_CPI.pdf](slides/RL_CPI.pdf) 
89. (2023/5/09) CVIのスライドの追加: [slides/RL_CVI.pdf](slides/RL_CVI.pdf) 
90. (2023/5/09) コンパクト集合: [notebooks/MATH_compact_set.ipynb](notebooks/MATH_compact_set.ipynb) 
91. (2023/5/09) Kiefer-Wolfowitzの定理: [notebooks/BANDIT_Kiefer_Wolfowitz.ipynb](notebooks/BANDIT_Kiefer_Wolfowitz.ipynb) 
92. (2023/5/10) 模倣学習の証明の修正: [notebooks/RL_imitation_learning.ipynb](notebooks/RL_imitation_learning.ipynb) 
93. (2023/5/11) 制約付きMDP（途中）: [notebooks/RL_CMDP.ipynb](notebooks/RL_CMDP.ipynb) 
94. (2023/5/11) 最小楕円問題のアルゴリズムとKYの初期化：[notebooks/CVX_MVEE_algorithm.ipynb](notebooks/CVX_MVEE_algorithm.ipynb)
95. (2023/5/14) エピソディック有限ホライゾンRL（途中）: [notebooks/RL_episodic_finite_horizon.ipynb](notebooks/RL_episodic_finite_horizon.ipynb) 
96. (2023/5/17) 統計的学習理論（途中）: [notebooks/MATH_statistical_learning_theory.ipynb](notebooks/MATH_statistical_learning_theory.ipynb) 
97. (2023/5/18) VC次元: [notebooks/MATH_complexity_of_hypothesis.ipynb](notebooks/MATH_complexity_of_hypothesis.ipynb) 
98. (2023/5/18) Binet-Cauchyの公式とか: [notebooks/LA_matrix_determinant.ipynb](notebooks/LA_matrix_determinant.ipynb) 
99. (2023/5/19) VC次元の続き: [notebooks/MATH_complexity_of_hypothesis.ipynb](notebooks/MATH_complexity_of_hypothesis.ipynb) 
100. (2023/5/19) ランクについて: [notebooks/LA_matrix_rank.ipynb](notebooks/LA_matrix_rank.ipynb) 
101. (2023/5/21) ラデマッハ複雑度とタラグランドの補題: [notebooks/MATH_complexity_of_hypothesis.ipynb](notebooks/MATH_complexity_of_hypothesis.ipynb) 
102. (2023/5/21) 正定値対称行列: [notebooks/LA_matrix_definite.ipynb](notebooks/LA_matrix_definite.ipynb) 
103. (2023/5/22) Linear MDPとMDVI: [Regularization and Variance-Weighted Regression Achieves Minimax Optimality in Linear MDPs: Theory and Practice](https://github.com/matsuolab/Variance-Weighted-MDVI)
104. (2023/5/24) 制約付きMDP（OptCMDP）: [notebooks/RL_CMDP_explore_exploit.ipynb](notebooks/RL_CMDP_explore_exploit.ipynb) 
105. (2023/5/24) Schur標準形、Rayleigh商: [notebooks/LA_matrix_definite.ipynb](notebooks/LA_matrix_definite.ipynb) 
106. (2023/5/25) 有限ホライゾンでの線型計画法: [notebooks/RL_as_LP_finite_horizon.ipynb](notebooks/RL_as_LP_finite_horizon.ipynb) 
107. (2023/5/25) OptCMDPの実装（途中）: [notebooks/RL_CMDP_explore_exploit.ipynb](notebooks/RL_CMDP_explore_exploit.ipynb) 
<!-- 76. (2023/4/15) 強化学習とFenchel-Rockafellar Duality：[notebooks/rl_and_duality.ipynb](notebooks/rl_and_duality.ipynb) -->
<!-- 35. (2023/2/25) マルチタスクバンディット: [notebooks/BANDIT_linear_improved.ipynb](notebooks/BANDIT_linear_improved.ipynb)  -->

---

## 分野別のNotebook一覧

### 線形代数

* (2023/4/07) 行列と行列式: [LA_matrix_determinant.ipynb](notebooks/LA_matrix_determinant.ipynb)
* (2023/4/28) ゲルシュゴリンの定理: [notebooks/LA_Gershgorin_circle_theorem.ipynb](notebooks/LA_Gershgorin_circle_theorem.ipynb)
* (2023/5/21) 正定値対称行列: [notebooks/LA_matrix_definite.ipynb](notebooks/LA_matrix_definite.ipynb) 
* (2023/5/24) Schur標準形、Rayleigh商: [notebooks/LA_matrix_definite.ipynb](notebooks/LA_matrix_definite.ipynb) 


### 確率論入門

* (2023/1/21) 測度論的確率論の導入: [notebooks/PROB_measure_theoretic_probability.ipynb](notebooks/PROB_measure_theoretic_probability.ipynb)
* (2023/1/26) 確率過程: [notebooks/PROB_probability_process.ipynb](notebooks/PROB_probability_process.ipynb)
* (2023/1/28) ルベーグ積分: [notebooks/PROB_lebesgue_integral.ipynb](notebooks/PROB_lebesgue_integral.ipynb)
* (2023/1/28) 上極限、下極限: [notebooks/PROB_liminf_limsup.ipynb](notebooks/PROB_liminf_limsup.ipynb)
* (2023/1/29) 極値分布: [notebooks/PROB_extreme_value_distribution.ipynb](notebooks/PROB_extreme_value_distribution.ipynb)
* (2023/1/29) 特性関数: [notebooks/PROB_characteristic_function.ipynb](notebooks/PROB_characteristic_function.ipynb)
* (2023/1/29) 確率積分（TODO）: [notebooks/PROB_stochastic_integration.ipynb](notebooks/PROB_stochastic_integration.ipynb)
* (2023/1/31) 伊藤積分 & 確率微分方程式の実験: [notebooks/PROB_stochastic_integration.ipynb](notebooks/PROB_stochastic_integration.ipynb)
* (2023/2/1) Girsanovの定理: [notebooks/PROB_stochastic_integration.ipynb](notebooks/PROB_stochastic_integration.ipynb)
* (2023/2/4) ガウス過程回帰: [notebooks/PROB_gp_regression.ipynb](notebooks/PROB_gp_regression.ipynb)
* (2023/3/17) 最尤推定：[notebooks/PROB_maximum_likelihood.ipynb](notebooks/PROB_maximum_likelihood.ipynb)

### 凸最適化

* (2023/3/20~21) 凸集合：[notebooks/CVX_convex_sets.ipynb](notebooks/CVX_convex_sets.ipynb)
* (2023/3/28) 凸関数：[notebooks/CVX_convex_functions.ipynb](notebooks/CVX_convex_functions.ipynb)
* (2023/4/01) 最小楕円問題：[notebooks/CVX_minimum_volume_ellipsoids.ipynb](notebooks/CVX_minimum_volume_ellipsoids.ipynb)
* (2023/4/03) 最小楕円問題のアルゴリズム：[notebooks/CVX_MVEE_algorithm.ipynb](notebooks/CVX_MVEE_algorithm.ipynb)


### 逐次意思決定問題

* バンディット：
    * (2023/1/29) バンディットアルゴリズムの基本: [notebooks/BANDIT_basics.ipynb](notebooks/BANDIT_basics.ipynb)
    * (2023/2/24) Self-Normalized Bound for Vector Valued Martingales: [notebooks/BANDIT_linear_improved.ipynb](notebooks/BANDIT_linear_improved.ipynb) 
    * (2023/2/8) 文脈付きバンディット: [notebooks/BANDIT_contextual.ipynb](notebooks/BANDIT_contextual.ipynb)
    * (2023/2/26) 探索の理論 (UCB編): [notebooks/BANDIT_UCB_regret_proof.ipynb](notebooks/BANDIT_UCB_regret_proof.ipynb) 
    * (2023/4/13) 敵対的バンディット: [notebooks/BANDIT_adversarial.ipynb](notebooks/BANDIT_adversarial.ipynb) 
    * (2023/4/12) バンディットの便利な関数: [notebooks/BANDIT_utils.ipynb](notebooks/BANDIT_utils.ipynb) 
    * (2023/5/08) 敵対的線形バンディット: [notebooks/BANDIT_adversarial_linear.ipynb](notebooks/BANDIT_adversarial_linear.ipynb) 
    * (2023/5/09) Kiefer-Wolfowitzの定理: [notebooks/BANDIT_Kiefer_Wolfowitz.ipynb](notebooks/BANDIT_Kiefer_Wolfowitz.ipynb) 
* Linear MDP：
    * (2023/1/18) Linear MDP: [notebooks/RL_linearMDP.ipynb](notebooks/RL_linearMDP.ipynb)
    * (2023/4/22) Linear MDPでのサンプル効率の下界: [RL_linearMDP_lower_bound.ipynb](notebooks/RL_linearMDP_lower_bound.ipynb)
* Reward Free RL：
    * (2023/2/22) Reward Free RL: [notebooks/RL_reward_free.ipynb](notebooks/RL_reward_free.ipynb)
    * (2023/4/09) エントロピー最大化と探索（EntGameアルゴリズム）: [RL_max_ent_exploration.ipynb](notebooks/RL_max_ent_exploration.ipynb)
* ロバストMDP：
    * (2023/3/8) ロバストMDP: [notebooks/RL_robust_MDP.ipynb](notebooks/RL_robust_MDP.ipynb) 
    * (2023/3/10) ロバストMDPの理論（モデルベース＆Generative model）: [notebooks/RL_robust_MDP.ipynb](notebooks/RL_robust_MDP.ipynb) 
    * (2023/3/13) ロバストMDPの理論（正則化との関係）: [notebooks/RL_robust_MDP_and_regularization.ipynb](notebooks/RL_robust_MDP_and_regularization.ipynb) 
    * (2023/4/27) ロバストQ学習: [RL_robust_Q_learning](notebooks/RL_robust_Q_learning.ipynb)
* 制約付きMDP：
    * (2023/5/24) 制約付きMDP（OptCMDP）: [notebooks/RL_CMDP_explore_exploit.ipynb](notebooks/RL_CMDP_explore_exploit.ipynb) 
* マルチステップ強化学習：
    * (2023/2/5) マルチステップ強化学習: [notebooks/RL_multi_step.ipynb](notebooks/RL_multi_step.ipynb)
    * (2023/2/14~17) マルチステップRLのスライド: [slides/RL_multi_step.pdf](slides/RL_multi_step.pdf)
    * (2023/2/19) 方策勾配法 (マルチステップRL): [notebooks/RL_policy_gradient.ipynb](notebooks/RL_policy_gradient.ipynb)
* 模倣学習：
    * (2023/3/14) 模倣学習: [notebooks/RL_imitation_learning.ipynb](notebooks/RL_imitation_learning.ipynb) 
* 一般のRL：
    * (2023/2/7) MDPについて (Garnet MDP): [notebooks/RL_Markov_Decision_Process.ipynb](notebooks/RL_Markov_Decision_Process.ipynb)
    * (2023/2/27-28) UCB-VIの理論 (モデルベース): [notebooks/RL_UCB_VI_regret_proof.ipynb](notebooks/RL_UCB_VI_regret_proof.ipynb) 
    * (2023/3/4) UCB-Hoeffdingの理論 (モデルフリー): [notebooks/RL_UCB_H_regret_proof.ipynb](notebooks/RL_UCB_H_regret_proof.ipynb) 
    * (2023/3/5) 遷移確率の推定について: [notebooks/RL_transition_estimation_proofs.ipynb](notebooks/RL_transition_estimation_proofs.ipynb) 
    * (2023/3/7) Task-agnostic探索の理論: [notebooks/RL_task_agnostic_exploration.ipynb](notebooks/RL_task_agnostic_exploration.ipynb) 
    * (2023/2/10) 適合価値反復法: [notebooks/RL_fitted_Q_iteration.ipynb](notebooks/RL_fitted_Q_iteration.ipynb)
    * (2023/3/12) 強化学習と線形計画問題: [notebooks/RL_as_LP.ipynb](notebooks/RL_as_LP.ipynb) 
    * (2023/2/12) Generalized RL: [notebooks/generalied_RL.ipynb](notebooks/RL_generalized.ipynb)
    * (2023/3/22) 強化学習のサンプル効率の下界：[notebooks/RL_lower_bounds.ipynb](notebooks/RL_lower_bounds.ipynb)
    * (2023/3/29) Approximate Dynamic Programming：[notebooks/RL_approximate_dynamic_programming.ipynb](notebooks/RL_approximate_dynamic_programming.ipynb)
    * (2023/5/09) CPIのスライド: [slides/RL_CPI.pdf](slides/RL_CPI.pdf) 
    * (2023/5/09) CVIのスライド: [slides/RL_CVI.pdf](slides/RL_CVI.pdf) 
    * (2023/5/11) 制約付きMDP: [notebooks/RL_CMDP.ipynb](notebooks/RL_CMDP.ipynb) 
    * (2023/5/14) エピソディック有限ホライゾンRL（途中）: [notebooks/RL_episodic_finite_horizon.ipynb](notebooks/RL_episodic_finite_horizon.ipynb) 
    * (2023/5/25) 有限ホライゾンでの線型計画法: [notebooks/RL_as_LP_finite_horizon.ipynb](notebooks/RL_as_LP_finite_horizon.ipynb) 
* 教育用：
    * (2023/2/23) 教育用強化学習Notebook (行列形式の動的計画法編): [notebooks/RL_exercise.ipynb](notebooks/RL_exercise.ipynb)
    * (2023/3/12) 強化学習の便利な関数: [notebooks/RL_utils.ipynb](notebooks/RL_utils.ipynb) 
    * (2023/4/12) バンディットの便利な関数: [notebooks/BANDIT_utils.ipynb](notebooks/BANDIT_utils.ipynb) 


### ニューラルネットワーク
* (2023/2/20~21) Transformer: [notebooks/NN_transformer.ipynb](notebooks/NN_transformer.ipynb)


### 数学
* (2023/1/30) テイラーの定理: [notebooks/MATH_taylor_theorem.ipynb](notebooks/MATH_taylor_theorem.ipynb)
* (2023/5/09) コンパクト集合: [notebooks/MATH_compact_set.ipynb](notebooks/MATH_compact_set.ipynb) 
* (2023/5/17) 統計的学習理論: [notebooks/MATH_statistical_learning_theory.ipynb](notebooks/MATH_statistical_learning_theory.ipynb) 
* (2023/5/18) 仮説集合の複雑度: [notebooks/MATH_complexity_of_hypothesis.ipynb](notebooks/MATH_complexity_of_hypothesis.ipynb) 

---

## わからなかったところ
* [ ] (2023/2/27-28) 探索の理論 (UCB-VI編): [notebooks/BANDIT_UCB_regret_proof.ipynb](notebooks/BANDIT_UCB_regret_proof.ipynb) 
    * [ ] UCBのボーナスが大きすぎるとボーナスが優先されてしまうが、こういう理論はあるのかな？
    * [x] 途中のHolderの不等式をなんで使うのかがわからん
    * [x] やっぱ$f$を$H^S$でUnion Bound取るのよくわかんないな... Hoeffdingでやるだけじゃ駄目なのか？
        * これは$\widehat{P}_h^k$と$\widehat{V}_{h+1}^{\pi^k}$が独立ではないのが原因。$\widehat{P}_h^k$と$P_h^\star$をバウンドすると、余分な$\sqrt{S}$が出てくるよ。
        * [Near-optimal Regret Bounds for Reinforcement Learning](https://www.jmlr.org/papers/volume11/jaksch10a/jaksch10a.pdf)の式（４４）あたりが参考になるかも。ただ、Hoeffding+Sについての和を考えても出る気がする。
* [ ] (2023/3/8) ロバストMDP: [notebooks/RL_robust_MDP.ipynb](notebooks/RL_robust_MDP.ipynb) 
    * [ ] ロバストRLがちゃんと機能しているかの評価方法はどうするべき？
* [ ] (2023/3/12) 強化学習と線形計画問題: [notebooks/RL_as_LP.ipynb](notebooks/RL_as_LP.ipynb) 
    * [ ] [Reinforcement Learning via Fenchel-Rockafellar Duality](https://arxiv.org/abs/2001.01866)これ読んでまとめたほうがいいかも？
* [ ] (2023/3/14) 模倣学習: [notebooks/RL_imitation_learning.ipynb](notebooks/RL_imitation_learning.ipynb) 
    * [ ] $\mathbb{E}_{s \sim d^{\pi^{\star}}}\left\|\widehat{\pi}(\cdot \mid s)-\pi^{\star}(\cdot \mid s)\right\|_{T V}^2 \leq \frac{2 \log (|\Pi| / \delta)}{M}$ の証明ができなかった。[Empirical Processes in M-Estimation](https://www.amazon.co.jp/-/en/Sara-van-Geer/dp/0521123259)に証明あるかも。
    * [ ] エントロピー最大化逆強化学習ではエントロピーを入れることに必然性があったきがする。探しておこう。
    - [ ] AggreVateのリグレットの証明
    - [ ] AggreVateはもっと良い実装方法ないかな？計算コストが高すぎるかも。
* [ ] (2023/3/22) 強化学習のサンプル効率の下界：[notebooks/RL_lower_bounds.ipynb](notebooks/RL_lower_bounds.ipynb)
    * [ ] 意外と行列の性質の理解が曖昧。（$\|\phi(s, a)\|_2 \leq 1$なので$\sigma_{\min }\left(\mathbb{E}_{(s, a) \sim \widetilde{\mu}_h}\left[\phi(s, a) \phi(s, a)^{\top}\right]\right)$が成り立つためです）。これとか微妙。


## TODO
* [ ] 過去のノートブックをきれいに直す
* [ ] モデルベースの証明やモデルフリーの証明をまとめたい
* [ ] 初学者が最初に読むべき本をまとめたい
* [ ] 確率収束の話
* [ ] Integral Probability Metricについて読もう：[On the empirical estimation of integral probability metrics](https://projecteuclid.org/journals/electronic-journal-of-statistics/volume-6/issue-none/On-the-empirical-estimation-of-integral-probability-metrics/10.1214/12-EJS722.full)
* [ ] 強化学習のサンプル効率の下界
    * [ ] VC次元を使ったオッカムの剃刀
    * [x] Linear Realizability
* [ ] バンディットの理論証明書く
* [ ] バンディットの便利関数まとめる
    * [ ] 敵対的系のアルゴリズム
* [ ] 強化学習の便利定理まとめる
    * [notebooks/RL_approximate_dynamic_programming.ipynb](notebooks/RL_approximate_dynamic_programming.ipynb)にでてきた価値差分方程式
    * $P$の逆行列の話
* [ ] (2023/3/8) ロバストMDP: [notebooks/RL_robust_MDP.ipynb](notebooks/RL_robust_MDP.ipynb) 
    * [Towards Minimax Optimality of Model-based Robust Reinforcement Learning](https://arxiv.org/abs/2302.05372)ではほぼ同じ条件でもっとタイトなバウンドを導出してる。
* (2023/3/27) 強化学習とエントロピー正則化：[notebooks/RL_entropy_regularization.ipynb](notebooks/RL_entropy_regularization.ipynb)
    * Value Iterationや貪欲方策が誤差に弱い証明が欲しい。Tsallis Entropyの話のほうがいいかな？
    * この話は先にApproximate Dynamic Programmingの証明を書いてからの方が書きやすいかも
* (2023/3/30) Approximate Dynamic Programming（正則化あり）：[notebooks/RL_approximate_dynamic_programming.ipynb](notebooks/RL_approximate_dynamic_programming.ipynb)
    * 正則化が入ったときの方策反復法のバウンドのわかりやすい導出を考えよう
    * KL+エントロピーの方策反復法のバウンドの導出はLeverage the Averageの方針でやると出せないかもしれない。λ-policy iterationを駆使したほうがいいかも？
* [ ] (2023/4/02) 他変量関数の微分：[notebooks/MATH_multivariate_derivative.ipynb](notebooks/MATH_multivariate_derivative.ipynb)
    * [ ] 全微分について書く
* [ ] 最小楕円問題とCore-set：[notebooks/CVX_MVEE_algorithm.ipynb](notebooks/CVX_MVEE_algorithm.ipynb)
    * 線形代数の話を踏まえて最小楕円問題の解釈を書く
* [ ] $\varepsilon$-greedyのバンディットの導出
    * https://sites.cs.ucsb.edu/~yuxiangw/classes/RLCourse-2021Spring/Lectures/scribe_MAB.pdf
