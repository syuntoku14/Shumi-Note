# Shumi-Note

勉強のアウトプット用にまとめているJupyter notebookです。
[notebooks](notebooks/)以下に色々まとまっています。

---

**制作方針**

* 全てのnotebookは独立させています。管理もしやすいので嬉しいですね。
* その日の気分でクオリティが左右されます
* 「なぜその内容を学ぶと嬉しいのか？」がなるべく分かるように書いています。教育用途でも使えたらいいなって気持ち。

---

**Notebookの内容**

* 内容のチョイスは僕の趣味です。
( 内容は勉強中にまとめているので必ずしも正しいとは限りません。誤りは見つけ次第直します。
* 内容が怪しいやつ（Notationの不備など）はTODOがついてます。

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
15. (2023/2/5) マルチステップ強化学習 (On-policy編): [notebooks/multi_step_RL.ipynb](notebooks/multi_step_RL.ipynb)
16. (2023/2/6) マルチステップ強化学習 (Off-policy編): [notebooks/multi_step_RL.ipynb](notebooks/multi_step_RL.ipynb)
17. (2023/2/6) マルチステップ強化学習 (マルチステップ制御編): [notebooks/multi_step_RL.ipynb](notebooks/multi_step_RL.ipynb)
18. (2023/2/7) MDPについて (Garnet MDP): [notebooks/Markov_Decision_Process.ipynb](notebooks/Markov_Decision_Process.ipynb)
19. (2023/2/7) 文脈付きバンディット (TODO): [notebooks/contextual_bandit.ipynb](notebooks/contextual_bandit.ipynb)

---


**インストール**

poetryを使ってください。

```bash
git clone git@github.com:syuntoku14/Shumi-Note.git && cd Shumi-Note
poetry install
```


Anacondaの場合：

```bash
conda create --name shumi-note python==3.9  # conda環境の作成（最初の一回だけ）
conda activate shumi-note  # 環境の切り替え
```