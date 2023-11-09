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
41. (2023/3/7) Task-agnostic探索の理論: [notebooks/RL_reward_free_task_agnostic.ipynb](notebooks/RL_reward_free_task_agnostic.ipynb) 
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
67. (2023/4/07) エントロピー最大化と探索（途中）: [RL_reward_free_max_ent.ipynb](notebooks/RL_reward_free_max_ent.ipynb)
68. (2023/4/08) 強化学習の便利な関数（有限ホライゾン）: [notebooks/RL_utils.ipynb](notebooks/RL_utils.ipynb) 
69. (2023/4/09) 強化学習の便利な関数（探索用）: [notebooks/RL_utils.ipynb](notebooks/RL_utils.ipynb) 
70. (2023/4/09) エントロピー最大化と探索（EntGameアルゴリズム）: [RL_reward_free_max_ent.ipynb](notebooks/RL_reward_free_max_ent.ipynb)
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
104. (2023/5/24) 制約付きMDP（OptCMDP）: [notebooks/RL_CMDP_explore_exploit_LP.ipynb](notebooks/RL_CMDP_explore_exploit_LP.ipynb) 
105. (2023/5/24) Schur標準形、Rayleigh商: [notebooks/LA_matrix_definite.ipynb](notebooks/LA_matrix_definite.ipynb) 
106. (2023/5/25) 有限ホライゾンでの線型計画法: [notebooks/RL_as_LP_finite_horizon.ipynb](notebooks/RL_as_LP_finite_horizon.ipynb) 
107. (2023/5/25) OptCMDPの実装: [notebooks/RL_CMDP_explore_exploit_LP.ipynb](notebooks/RL_CMDP_explore_exploit_LP.ipynb) 
108. (2023/5/27) ベクトル空間: [notebooks/LA_vector_space.ipynb](notebooks/LA_vector_space.ipynb) 
109. (2023/5/28) 計量、内積: [notebooks/LA_vector_space.ipynb](notebooks/LA_vector_space.ipynb) 
110. (2023/5/28) 標準形: [notebooks/LA_normal_form.ipynb](notebooks/LA_normal_form.ipynb) 
111. (2023/5/29) PAC-Bayes: [notebooks/MATH_PAC_Bayes.ipynb](notebooks/MATH_PAC_Bayes.ipynb) 
112. (2023/5/29) Stabilityと汎化誤差バウンド: [notebooks/MATH_PAC_stability.ipynb](notebooks/MATH_PAC_stability.ipynb) 
113. (2023/5/30) 階数標準形の実装: [notebooks/LA_normal_form.ipynb](notebooks/LA_normal_form.ipynb) 
114. (2023/5/31) 制約違反なしのCMDP: [notebooks/RL_CMDP_explore_exploit_LP.ipynb](notebooks/RL_CMDP_explore_exploit_LP.ipynb) 
115. (2023/6/01) 整数行列: [notebooks/LA_integer_matrix.ipynb](notebooks/LA_integer_matrix.ipynb) 
116. (2023/6/01) 行列形式の有限ホライゾンでのLP: [notebooks/RL_as_LP_finite_horizon.ipynb](notebooks/RL_as_LP_finite_horizon.ipynb) 
117. (2023/6/02) 双対法によるCMDPの解法: [notebooks/RL_CMDP_dual.ipynb](notebooks/RL_CMDP_dual.ipynb) 
118. (2023/6/06) ロバスト最適化: [notebooks/OPT_robust_optimization.ipynb](notebooks/OPT_robust_optimization.ipynb) 
119. (2023/6/07) 行列形式の有限ホライゾンでのLP（主問題）: [notebooks/RL_as_LP_finite_horizon.ipynb](notebooks/RL_as_LP_finite_horizon.ipynb) 
120. (2023/6/08) 凸最適化としてのロバストMDP: [notebooks/RL_robust_MDP_convex..ipynb](notebooks/RL_robust_MDP_convex..ipynb) 
121. (2023/6/08) 制約付きMDPと強双対性: [notebooks/RL_CMDP_zero_duality_gap.ipynb](notebooks/RL_CMDP_zero_duality_gap.ipynb) 
122. (2023/6/09) 占有率の集合の凸性: [notebooks/RL_occupancy_measure.ipynb](notebooks/RL_occupancy_measure.ipynb) 
123. (2023/6/11) ロバストMDPの理論（正則化との関係）: [notebooks/RL_robust_MDP_and_regularization.ipynb](notebooks/RL_robust_MDP_and_regularization.ipynb) 
124. (2023/6/12) 線形計画法のContraction Lemmaによる変形の注記: [notebooks/RL_as_LP.ipynb](notebooks/RL_as_LP.ipynb)
125. (2023/6/13) 最適化と双対問題：[notebooks/CVX_duality.ipynb](notebooks/CVX_duality.ipynb)
126. (2023/6/14) ロバストMDPでの完全双対性について文献の補足　：[notebooks/RL_as_LP_finite_horizon](notebooks/RL_as_LP_finite_horizon.ipynb) と [notebooks/RL_robust_MDP](notebooks/RL_robust_MDP.ipynb)
127. (2023/6/15) 劣勾配法: [notebooks/OPT_subgradient.ipynb](notebooks/OPT_subgradient.ipynb) 
128. (2023/6/16) 勾配法: [notebooks/OPT_gradient.ipynb](notebooks/OPT_gradient.ipynb) 
129. (2023/6/21) ロバストMDPと確率的制約: [notebooks/OPT_robust_chance_constraint.ipynb](notebooks/OPT_robust_chance_constraint.ipynb) 
130. (2023/7/01) 制約付き最適化（最適性条件）: [notebooks/OPT_constraint.ipynb](notebooks/OPT_constraint.ipynb)
131. (2023/7/05) 感度解析: [notebooks/CVX_sensitivity_analysis.ipynb](notebooks/CVX_sensitivity_analysis.ipynb)
132. (2023/7/06) ロバストMDPにおけるRectangularity: [notebooks/RL_robust_rectangularity.ipynb](notebooks/RL_robust_rectangularity.ipynb)
133. (2023/7/12) Danskinの定理: [notebooks/CVX_Danskin_theorem.ipynb](notebooks/CVX_Danskin_theorem.ipynb)
134. (2023/7/13) 凸関数は連続: [notebooks/CVX_convex_functions.ipynb](notebooks/CVX_convex_functions.ipynb)
135. (2023/7/24) 制約付きMDPとラグランジュ関数（途中）: [notebooks/RL_CMDP_Lagrange.ipynb](notebooks/RL_CMDP_Lagrange.ipynb) 
136. (2023/7/25) 制約付きMDPとラグランジュ関数: [notebooks/RL_CMDP_Lagrange.ipynb](notebooks/RL_CMDP_Lagrange.ipynb) 
137. (2023/7/29) 連合Q学習: [notebooks/RL_federated_Q.ipynb](notebooks/RL_federated_Q.ipynb) 
138. (2023/7/30) PACベイズ制御: [notebooks/CONTROL_PAC_Bayes.ipynb](notebooks/CONTROL_PAC_Bayes.ipynb) 
139. (2023/8/04) 制約付きMDPと強双対性（修正）: [notebooks/RL_CMDP_zero_duality_gap.ipynb](notebooks/RL_CMDP_zero_duality_gap.ipynb) 
140. (2023/8/07) ロバストMDPと強双対性: [notebooks/RL_robust_MDP_zero_duality.ipynb](notebooks/RL_robust_MDP_zero_duality.ipynb) 
141. (2023/8/11) 凸ではない価値関数: [notebooks/RL_value_function.ipynb](notebooks/RL_value_function.ipynb) 
142. (2023/8/15) PACベイズとメタ学習: [notebooks/MATH_PAC_Bayes_Meta_Learning.ipynb](notebooks/MATH_PAC_Bayes_Meta_Learning.ipynb) 
143. (2023/8/16) 色々なMinimax双対定理と証明: [notebooks/MATH_minimax_theorems.ipynb](notebooks/MATH_minimax_theorems.ipynb) 
144. (2023/8/17) FanのMinimax定理について: [notebooks/MATH_minimax_theorems.ipynb](notebooks/MATH_minimax_theorems.ipynb) 
145. (2023/8/20) Minimax双対性の必要条件と十分条件について: [notebooks/MATH_minimax_conditions.ipynb](notebooks/MATH_minimax_conditions.ipynb) 
146. (2023/8/21) バリア関数法: [notebooks/MATH_barrier_function_method.ipynb](notebooks/MATH_barrier_function_method.ipynb) 
147. (2023/8/24) ロバストMDPとNP困難: [notebooks/RL_robust_MDP_NP_hard.ipynb](notebooks/RL_robust_MDP_NP_hard.ipynb)
148. (2023/8/25) Policy searchとNP困難: [notebooks/RL_policy_search_NP_hard.ipynb](notebooks/RL_policy_search_NP_hard.ipynb)
149. (2023/8/26) 凸ではない価値関数について追記: [notebooks/RL_value_function.ipynb](notebooks/RL_value_function.ipynb) 
150. (2023/8/28) マルチタスク模倣学習と表現学習: [notebooks/RL_multi_task_imitation_learning.ipynb](notebooks/RL_multi_task_imitation_learning.ipynb) 
151. (2023/8/30) MDPにおける安全な探索: [notebooks/RL_CMDP_safe_exploration.ipynb](notebooks/RL_CMDP_safe_exploration.ipynb) 
152. (2023/9/01) CMDPにおける動的計画法: [notebooks/RL_CMDP_by_DP.ipynb](notebooks/RL_CMDP_by_DP.ipynb) 
153. (2023/9/03) CMDPにおける動的計画法（non-stationary）: [notebooks/RL_CMDP_by_DP_non_stationary.ipynb](notebooks/RL_CMDP_by_DP_non_stationary.ipynb) 
154. (2023/9/04) CMDPにおける動的計画法（non-stationary）の修正: [notebooks/RL_CMDP_by_DP_non_stationary.ipynb](notebooks/RL_CMDP_by_DP_non_stationary.ipynb) 
155. (2023/9/08) 制約付きMDPと強双対性（エントロピー）: [notebooks/RL_CMDP_zero_duality_gap_entropy.ipynb](notebooks/RL_CMDP_zero_duality_gap_entropy.ipynb) 
156. (2023/9/15) 整数計画問題とNP困難: [notebooks/MATH_integer_programming_is_NP_hard.ipynb](notebooks/MATH_integer_programming_is_NP_hard.ipynb) 
157. (2023/9/16) CMDPの実行可能解を見つけるのはNP困難: [notebooks/RL_CMDP_feasibility_NP_hard.ipynb](notebooks/RL_CMDP_feasibility_NP_hard.ipynb) 
158. (2023/9/17) CMDPの実行可能解を見つけるのはNP困難（更新）: [notebooks/RL_CMDP_feasibility_NP_hard.ipynb](notebooks/RL_CMDP_feasibility_NP_hard.ipynb) 
159. (2023/9/24) LQR: [notebooks/RL_LQR.ipynb](notebooks/RL_LQR.ipynb) 
160. (2023/9/25) LQRと半正定値計画問題: [notebooks/RL_LQR_as_SDP.ipynb](notebooks/RL_LQR_as_SDP.ipynb) 
161. (2023/9/25) 制約付きLQR: [notebooks/RL_LQR_safe.ipynb](notebooks/RL_LQR_safe.ipynb) 
162. (2023/9/28) Mean-Variance MDPとNP困難: [notebooks/RL_mean_variance_MDP_NP_hard.ipynb](notebooks/RL_mean_variance_MDP_NP_hard.ipynb) 
163. (2023/9/28) Domain-Randomizationの数理（途中）: [notebooks/RL_multi_task_domain_randomization.ipynb](notebooks/RL_multi_task_domain_randomization.ipynb) 
164. (2023/9/29) Convex MDPについて: [notebooks/RL_Convex_MDP.ipynb](notebooks/RL_Convex_MDP.ipynb) 
165. (2023/10/1) LQRの方策勾配法: [notebooks/RL_LQR_policy_gradient.ipynb](notebooks/RL_LQR_policy_gradient.ipynb) 
166. (2023/10/1) 線形システムにおけるSystem Level Synthesis: [notebooks/RL_LQR_SLS_finite_horizon.ipynb](notebooks/RL_LQR_SLS_finite_horizon.ipynb) 
167. (2023/10/1) LQRによる経路追従（途中で諦め）: [notebooks/RL_LQR_path_tracking.ipynb](notebooks/RL_LQR_path_tracking.ipynb) 
168. (2023/10/2) LQRにおけるダイナミクスの推定とロバストな制御: [notebooks/RL_LQR_estimation_and_robustness.ipynb](notebooks/RL_LQR_estimation_and_robustness.ipynb) 
169. (2023/10/3) 文脈付きMDP: [notebooks/RL_multi_task_contextual_MDP.ipynb](notebooks/RL_multi_task_contextual_MDP.ipynb) 
170. (2023/10/4) マルチタスク強化学習: [notebooks/RL_multi_task.ipynb](notebooks/RL_multi_task.ipynb) 
171. (2023/10/4) Latent MDP: [notebooks/RL_multi_task_latent_MDP.ipynb](notebooks/RL_multi_task_latent_MDP.ipynb) 
172. (2023/10/4) マルチタスクMDPにおける文脈の推定: [notebooks/RL_multi_task_context_identification.ipynb](notebooks/RL_multi_task_context_identification.ipynb) 
173. (2023/10/8) LQRの便利な関数: [notebooks/RL_LQR_utils.ipynb](notebooks/RL_LQR_utils.ipynb) 
174. (2023/10/9) System Level Synthesisの導出について: [notebooks/RL_LQR_SLS_finite_horizon.ipynb](notebooks/RL_LQR_SLS_finite_horizon.ipynb) 
175. (2023/10/10) Robust System Level Synthesis: [notebooks/RL_LQR_robust_synthesis.ipynb](notebooks/RL_LQR_robust_synthesis.ipynb) 
176. (2023/10/13) System Level Synthesisの説明: [notebooks/RL_LQR_SLS_finite_horizon.ipynb](notebooks/RL_LQR_SLS_finite_horizon.ipynb) 
177. (2023/10/16) SLSによるH∞制御: [notebooks/RL_LQR_SLS_finite_horizon.ipynb](notebooks/RL_LQR_SLS_finite_horizon.ipynb) 
178. (2023/10/16) SLSによるロバスト制御: [notebooks/RL_LQR_SLS_finite_horizon.ipynb](notebooks/RL_LQR_SLS_finite_horizon.ipynb) 
179. (2023/10/16) SLSによるノイズあり制約付き制御: [notebooks/RL_LQR_SLS_finite_horizon.ipynb](notebooks/RL_LQR_SLS_finite_horizon.ipynb) 
180. (2023/10/18) RLにおける汎化の難しさ: [notebooks/RL_multi_task_generalization_intractable.ipynb](notebooks/RL_multi_task_generalization_intractable.ipynb) 
181. (2023/10/18) 観測だけからの模倣学習: [notebooks/RL_imitation_from_observation.ipynb](notebooks/RL_imitation_from_observation.ipynb) 
182. (2023/10/18) 報酬設計によるサンプル効率の向上: [notebooks/RL_reward_shaping.ipynb](notebooks/RL_reward_shaping.ipynb) 
183. (2023/10/19) 平均報酬強化学習: [notebooks/RL_AverageReward.ipynb](notebooks/RL_AverageReward.ipynb) 
184. (2023/10/20) 強化学習とリプシッツ連続: [notebooks/RL_Continuous_Lipschitz.ipynb](notebooks/RL_Continuous_Lipschitz.ipynb) 
185. (2023/10/24) RLHFの理論: [notebooks/RL_RLHF.ipynb](notebooks/RL_RLHF.ipynb) 
186. (2023/10/25) データソースが複数ある場合のオフライン強化学習: [notebooks/RL_offline_perturbed_data.ipynb](notebooks/RL_offline_perturbed_data.ipynb) 
187. (2023/10/26) データを利用したロバスト最適化（微妙）: [notebooks/OPT_robust_learning_uncertainty_set_deprecated.ipynb](notebooks/OPT_robust_learning_uncertainty_set_deprecated.ipynb) 
188. (2023/10/29) データを利用したロバスト最適化: [notebooks/OPT_robust_learning_based.ipynb](notebooks/OPT_robust_learning_based.ipynb) 
189. (2023/11/1) カーネル強化学習: [notebooks/RL_Continuous_Kernel.ipynb](notebooks/RL_Continuous_Kernel.ipynb) 
190. (2023/11/3) Bellman rank: [notebooks/RL_Bellman_rank.ipynb](notebooks/RL_Bellman_rank.ipynb) 
191. (2023/11/3) モデルフリー平均報酬強化学習: [notebooks/RL_AverageReward_model_free.ipynb](notebooks/RL_AverageReward_model_free.ipynb) 
192. (2023/11/3) Bilinear class: [notebooks/RL_Bilinear_class.ipynb](notebooks/RL_Bilinear_class.ipynb) 
193. (2023/11/4) 制約違反なしのCMDP: [notebooks/RL_CMDP_zero_constraint_violation.ipynb](notebooks/RL_CMDP_zero_constraint_violation.ipynb) 
194. (2023/11/5) Witness rank: [notebooks/RL_witness_rank.ipynb](notebooks/RL_witness_rank.ipynb) 
195. (2023/11/6) RLとFenchel Rockafellar双対性とDICE: [notebooks/RL_Convex_Fenchel_Duality_and_DICE.ipynb](notebooks/RL_Convex_Fenchel_Duality_and_DICE.ipynb) 
196. (2023/11/7) 制約違反なしのCMDPの証明の続き（まだ途中）: [notebooks/RL_CMDP_zero_constraint_violation.ipynb](notebooks/RL_CMDP_zero_constraint_violation.ipynb) 
197. (2023/11/8) RLの証明で便利な定理: [notebooks/RL_useful_lemma.ipynb](notebooks/RL_useful_lemma.ipynb) 
198. (2023/11/8) CMDPでの探索の証明の修正: [notebooks/RL_CMDP_explore_exploit_LP.ipynb](notebooks/RL_CMDP_explore_exploit_LP.ipynb) 
199. (2023/11/9) CMDPでの双対法のリグレット: [notebooks/RL_CMDP_explore_exploit_dual.ipynb](notebooks/RL_CMDP_explore_exploit_dual.ipynb) 

<!-- 151. (2023/8/29) Action gapと強化学習: [notebooks/RL_action_gap.ipynb](notebooks/RL_action_gap.ipynb)  -->
<!-- 35. (2023/2/25) マルチタスクバンディット: [notebooks/BANDIT_linear_improved.ipynb](notebooks/BANDIT_linear_improved.ipynb)  -->

---

## 分野別のNotebook一覧

### 線形代数

* (2023/4/07) 行列と行列式: [LA_matrix_determinant.ipynb](notebooks/LA_matrix_determinant.ipynb)
* (2023/4/28) ゲルシュゴリンの定理: [notebooks/LA_Gershgorin_circle_theorem.ipynb](notebooks/LA_Gershgorin_circle_theorem.ipynb)
* (2023/5/21) 正定値対称行列: [notebooks/LA_matrix_definite.ipynb](notebooks/LA_matrix_definite.ipynb) 
* (2023/5/24) Schur標準形、Rayleigh商: [notebooks/LA_matrix_definite.ipynb](notebooks/LA_matrix_definite.ipynb) 
* (2023/5/27) ベクトル空間: [notebooks/LA_vector_space.ipynb](notebooks/LA_vector_space.ipynb) 
* (2023/5/28) 標準形: [notebooks/LA_normal_form.ipynb](notebooks/LA_normal_form.ipynb) 
* (2023/6/01) 整数行列: [notebooks/LA_integer_matrix.ipynb](notebooks/LA_integer_matrix.ipynb) 


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
* (2023/6/13) 最適化と双対問題：[notebooks/CVX_duality.ipynb](notebooks/CVX_duality.ipynb)
* (2023/7/05) 感度解析: [notebooks/CVX_sensitivity_analysis.ipynb](notebooks/CVX_sensitivity_analysis.ipynb)
* (2023/7/12) Danskinの定理: [notebooks/CVX_Danskin_theorem.ipynb](notebooks/CVX_Danskin_theorem.ipynb)


### 最適化

* (2023/6/06) ロバスト最適化: [notebooks/OPT_robust_optimization.ipynb](notebooks/OPT_robust_optimization.ipynb) 
* (2023/6/15) 劣勾配法: [notebooks/OPT_subgradient.ipynb](notebooks/OPT_subgradient.ipynb) 
* (2023/6/16) 勾配法: [notebooks/OPT_gradient.ipynb](notebooks/OPT_gradient.ipynb) 
* (2023/6/21) ロバストMDPと確率的制約 [notebooks/OPT_robust_chance_constraint.ipynb](notebooks/OPT_robust_chance_constraint.ipynb) 
* (2023/10/29) データを利用したロバスト最適化: [notebooks/OPT_robust_learning_based.ipynb](notebooks/OPT_robust_learning_based.ipynb) 


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
    * (2023/3/7) Task-agnostic探索の理論: [notebooks/RL_reward_free_task_agnostic.ipynb](notebooks/RL_reward_free_task_agnostic.ipynb) 
    * (2023/4/09) エントロピー最大化と探索（EntGameアルゴリズム）: [RL_reward_free_max_ent.ipynb](notebooks/RL_reward_free_max_ent.ipynb)
* ロバストMDP：
    * (2023/3/8) ロバストMDP: [notebooks/RL_robust_MDP.ipynb](notebooks/RL_robust_MDP.ipynb) 
    * (2023/3/10) ロバストMDPの理論（モデルベース＆Generative model）: [notebooks/RL_robust_MDP.ipynb](notebooks/RL_robust_MDP.ipynb) 
    * (2023/3/13) ロバストMDPの理論（正則化との関係）: [notebooks/RL_robust_MDP_and_regularization.ipynb](notebooks/RL_robust_MDP_and_regularization.ipynb) 
    * (2023/4/27) ロバストQ学習: [RL_robust_Q_learning](notebooks/RL_robust_Q_learning.ipynb)
    * (2023/6/08) 凸最適化としてのロバストMDP: [notebooks/RL_robust_MDP_convex..ipynb](notebooks/RL_robust_MDP_convex..ipynb) 
    * (2023/8/07) ロバストMDPと強双対性: [notebooks/RL_robust_MDP_zero_duality.ipynb](notebooks/RL_robust_MDP_zero_duality.ipynb) 
    * (2023/8/24) ロバストMDPとNP困難: [notebooks/RL_robust_MDP_NP_hard.ipynb](notebooks/RL_robust_MDP_NP_hard.ipynb)
* 制約付きMDP：
    * (2023/5/24) 制約付きMDP（OptCMDP）: [notebooks/RL_CMDP_explore_exploit_LP.ipynb](notebooks/RL_CMDP_explore_exploit_LP.ipynb) 
    * (2023/6/02) 双対法によるCMDPの解法: [notebooks/RL_CMDP_dual.ipynb](notebooks/RL_CMDP_dual.ipynb) 
    * (2023/6/08) 制約付きMDPと強双対性: [notebooks/RL_CMDP_zero_duality_gap.ipynb](notebooks/RL_CMDP_zero_duality_gap.ipynb) 
    * (2023/8/30) MDPにおける安全な探索: [notebooks/RL_CMDP_safe_exploration.ipynb](notebooks/RL_CMDP_safe_exploration.ipynb) 
    * (2023/9/01) CMDPにおける動的計画法: [notebooks/RL_CMDP_by_DP.ipynb](notebooks/RL_CMDP_by_DP.ipynb) 
    * (2023/9/03) CMDPにおける動的計画法（non-stationary）: [notebooks/RL_CMDP_by_DP_non_stationary.ipynb](notebooks/RL_CMDP_by_DP_non_stationary.ipynb) 
    * (2023/9/08) 制約付きMDPと強双対性（エントロピー）: [notebooks/RL_CMDP_zero_duality_gap_entropy.ipynb](notebooks/RL_CMDP_zero_duality_gap_entropy.ipynb) 
    * (2023/9/16) CMDPの実行可能解を見つけるのはNP困難: [notebooks/RL_CMDP_feasibility_NP_hard.ipynb](notebooks/RL_CMDP_feasibitlity_NP_hard.ipynb) 
    * (2023/11/4) 制約違反なしのCMDP: [notebooks/RL_CMDP_zero_constraint_violation.ipynb](notebooks/RL_CMDP_zero_constraint_violation.ipynb) 
    * (2023/11/9) CMDPでの双対法のリグレット: [notebooks/RL_CMDP_explore_exploit_dual.ipynb](notebooks/RL_CMDP_explore_exploit_dual.ipynb) 
* 平均報酬強化学習：
    * (2023/10/19) 平均報酬強化学習: [notebooks/RL_AverageReward.ipynb](notebooks/RL_AverageReward.ipynb) 
    * (2023/11/3) モデルフリー平均報酬強化学習: [notebooks/RL_AverageReward_model_free.ipynb](notebooks/RL_AverageReward_model_free.ipynb) 
* 連合強化学習：
    * (2023/7/29) 連合Q学習: [notebooks/RL_federated_Q.ipynb](notebooks/RL_federated_Q.ipynb) 
* マルチステップ強化学習：
    * (2023/2/5) マルチステップ強化学習: [notebooks/RL_multi_step.ipynb](notebooks/RL_multi_step.ipynb)
    * (2023/2/14~17) マルチステップRLのスライド: [slides/RL_multi_step.pdf](slides/RL_multi_step.pdf)
    * (2023/2/19) 方策勾配法 (マルチステップRL): [notebooks/RL_policy_gradient.ipynb](notebooks/RL_policy_gradient.ipynb)
* 模倣学習：
    * (2023/3/14) 模倣学習: [notebooks/RL_imitation_learning.ipynb](notebooks/RL_imitation_learning.ipynb) 
    * (2023/8/28) マルチタスク模倣学習と表現学習: [notebooks/RL_multi_task_imitation_learning.ipynb](notebooks/RL_multi_task_imitation_learning.ipynb) 
    * (2023/10/18) 観測だけからの模倣学習: [notebooks/RL_imitation_from_observation.ipynb](notebooks/RL_imitation_from_observation.ipynb) 
* オフライン：
    * (2023/10/25) データソースが複数ある場合のオフライン強化学習: [notebooks/RL_offline_perturbed_data.ipynb](notebooks/RL_offline_perturbed_data.ipynb) 
* Mean-Variance MDP：
    * (2023/9/28) Mean-Variance MDPとNP困難: [notebooks/RL_mean_variance_MDP_NP_hard.ipynb](notebooks/RL_mean_variance_MDP_NP_hard.ipynb.ipynb) 
* 連続MDP：
    * (2023/10/20) 強化学習とリプシッツ連続: [notebooks/RL_Continuous_Lipschitz.ipynb](notebooks/RL_Continuous_Lipschitz.ipynb) 
    * (2023/11/1) カーネル強化学習: [notebooks/RL_Continuous_Kernel.ipynb](notebooks/RL_Continuous_Kernel.ipynb) 
* 一般のRL：
    * (2023/2/7) MDPについて (Garnet MDP): [notebooks/RL_Markov_Decision_Process.ipynb](notebooks/RL_Markov_Decision_Process.ipynb)
    * (2023/2/27-28) UCB-VIの理論 (モデルベース): [notebooks/RL_UCB_VI_regret_proof.ipynb](notebooks/RL_UCB_VI_regret_proof.ipynb) 
    * (2023/3/4) UCB-Hoeffdingの理論 (モデルフリー): [notebooks/RL_UCB_H_regret_proof.ipynb](notebooks/RL_UCB_H_regret_proof.ipynb) 
    * (2023/3/5) 遷移確率の推定について: [notebooks/RL_transition_estimation_proofs.ipynb](notebooks/RL_transition_estimation_proofs.ipynb) 
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
    * (2023/6/09) 占有率の集合の凸性: [notebooks/RL_occupancy_measure.ipynb](notebooks/RL_occupancy_measure.ipynb) 
    * (2023/8/11) 凸ではない価値関数: [notebooks/RL_value_function.ipynb](notebooks/RL_value_function.ipynb) 
    * (2023/8/25) Policy searchとNP困難: [notebooks/RL_policy_search_NP_hard.ipynb](notebooks/RL_policy_search_NP_hard.ipynb)
    * (2023/9/29) Convex MDPについて: [notebooks/RL_Convex_MDP.ipynb](notebooks/RL_Convex_MDP.ipynb) 
    * (2022/10/18) 報酬設計によるサンプル効率の向上: [notebooks/RL_reward_shaping.ipynb](notebooks/RL_reward_shaping.ipynb) 
    * (2023/10/24) RLHFの理論: [notebooks/RL_RLHF.ipynb](notebooks/RL_RLHF.ipynb) 
    * (2023/11/3) Bellman rank: [notebooks/RL_Bellman_rank.ipynb](notebooks/RL_Bellman_rank.ipynb) 
    * (2023/11/3) Bilinear class: [notebooks/RL_Bilinear_class.ipynb](notebooks/RL_Bilinear_class.ipynb) 
    * (2023/11/5) Witness rank: [notebooks/RL_witness_rank.ipynb](notebooks/RL_witness_rank.ipynb) 
    * (2023/11/6) RLとFenchel Rockafellar双対性とDICE: [notebooks/RL_Convex_Fenchel_Duality_and_DICE.ipynb](notebooks/RL_Convex_Fenchel_Duality_and_DICE.ipynb) 
    * (2023/11/8) RLの証明で便利な定理: [notebooks/RL_useful_lemma.ipynb](notebooks/RL_useful_lemma.ipynb) 
* マルチタスク系：
    * (2023/10/3) 文脈付きMDP: [notebooks/RL_multi_task_contextual_MDP.ipynb](notebooks/RL_multi_task_contextual_MDP.ipynb) 
    * (2023/9/28) Domain-Randomizationの数理（途中）: [notebooks/RL_multi_task_domain_randomization.ipynb](notebooks/RL_multi_task_domain_randomization.ipynb) 
    * (2023/8/28) マルチタスク模倣学習と表現学習: [notebooks/RL_multi_task_imitation_learning.ipynb](notebooks/RL_multi_task_imitation_learning.ipynb) 
    * (2023/10/4) マルチタスク強化学習: [notebooks/RL_multi_task.ipynb](notebooks/RL_multi_task.ipynb) 
    * (2023/10/4) Latent MDP: [notebooks/RL_multi_task_latent_MDP.ipynb](notebooks/RL_multi_task_latent_MDP.ipynb) 
    * (2023/10/4) マルチタスクMDPにおける文脈の推定: [notebooks/RL_multi_task_context_identification.ipynb](notebooks/RL_multi_task_context_identification.ipynb) 
    * (2023/10/18) RLにおける汎化の難しさ: [notebooks/RL_multi_task_generalization_intractable.ipynb](notebooks/RL_multi_task_generalization_intractable.ipynb) 
* LQR：
    * (2023/9/24) LQR（有限ホライゾン）: [notebooks/RL_LQR.ipynb](notebooks/RL_LQR.ipynb) 
    * (2023/9/25) LQRと半正定値計画問題: [notebooks/RL_LQR_as_SDP.ipynb](notebooks/RL_LQR_as_SDP.ipynb) 
    * (2023/9/25) 制約付きLQR: [notebooks/RL_LQR_safe.ipynb](notebooks/RL_LQR_safe.ipynb) 
    * (2023/10/1) LQRの方策勾配法: [notebooks/RL_LQR_policy_gradient.ipynb](notebooks/RL_LQR_policy_gradient.ipynb) 
    * (2023/10/1) 線形システムにおけるSystem Level Synthesis: [notebooks/RL_LQR_SLS_finite_horizon.ipynb](notebooks/RL_LQR_SLS_finite_horizon.ipynb) 
    * (2023/10/1) LQRによる経路追従（途中で諦め）: [notebooks/RL_LQR_path_tracking.ipynb](notebooks/RL_LQR_path_tracking.ipynb) 
    * (2023/10/2) LQRにおけるダイナミクスの推定とロバストな制御: [notebooks/RL_LQR_estimation_and_robustness.ipynb](notebooks/RL_LQR_estimation_and_robustness.ipynb) 
    * (2023/10/8) LQRの便利な関数: [notebooks/RL_LQR_utils.ipynb](notebooks/RL_LQR_utils.ipynb) 
    * (2023/10/10) Robust System Level Synthesis: [notebooks/RL_LQR_robust_synthesis.ipynb](notebooks/RL_LQR_robust_synthesis.ipynb) 
* 一般の制御：
    * (2023/7/30) PACベイズ制御: [notebooks/CONTROL_PAC_Bayes.ipynb](notebooks/CONTROL_PAC_Bayes.ipynb) 
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
* (2023/5/29) PAC-Bayes: [notebooks/MATH_PAC_Bayes.ipynb](notebooks/MATH_PAC_Bayes.ipynb) 
* (2023/5/29) Stabilityと汎化誤差バウンド: [notebooks/MATH_PAC_stability.ipynb](notebooks/MATH_PAC_stability.ipynb) 
* (2023/8/15) PACベイズとメタ学習: [notebooks/MATH_PAC_Bayes_Meta_Learning.ipynb](notebooks/MATH_PAC_Bayes_Meta_Learning.ipynb) 
* (2023/8/16) 色々なMinimax双対定理と証明: [notebooks/MATH_minimax_theorems.ipynb](notebooks/MATH_minimax_theorems.ipynb) 
* (2023/8/17) FanのMinimax定理について: [notebooks/MATH_minimax_theorems.ipynb](notebooks/MATH_minimax_theorems.ipynb) 
* (2023/8/20) Minimax双対性の必要条件と十分条件について: [notebooks/MATH_minimax_conditions.ipynb](notebooks/MATH_minimax_conditions.ipynb) 
* (2023/8/21) バリア関数法: [notebooks/MATH_barrier_function_method.ipynb](notebooks/MATH_barrier_function_method.ipynb) 
* (2023/9/15) 整数計画問題とNP困難: [notebooks/MATH_integer_programming_is_NP_hard.ipynb](notebooks/MATH_integer_programming_is_NP_hard.ipynb) 


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
* [ ] PACベイズにでてくるSafe probabilityの話、MDVIに使えないか？
