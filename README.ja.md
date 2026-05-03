# Poor Man's Opus

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![OpenClaw Skill](https://img.shields.io/badge/OpenClaw-Skill-blue.svg)](https://openclaw.ai)
[![I-Lang Protocol](https://img.shields.io/badge/I--Lang-v3.0-green.svg)](https://ilang.ai)

🌐 [English](README.md) | [简体中文](README.zh-CN.md)

**最安モデル。Opus 級の出力。一文字で全停止。**

DeepSeek V4 Pro + I-Lang 行動遺伝子 = Opus 品質の出力。ワンコマンドでインストール、一文字で即停止。95% 安く、100% 多くの制御を。

---

## なぜ機能するのか

ボトルネックはモデル能力ではない。**指示の質だ。**

DeepSeek V4 Pro は多くのベンチマークで Opus を上回る推論力を持つ。しかし出力の「感触」が違う——テンプレートの冒頭、箇条書き、免責事項の羅列。

Opus の「感じ」は行動から来る——語調、リズム、ニュアンス、正直さ。これらはモデルパラメータではなく、指示の問題だ。

Opus の行動パターンを I-Lang 遺伝子に逆コンパイルし、DeepSeek に注入。同じモデル。違う服装。ファインチューニングなし。RAG なし。API 呼び出しなし。純粋な指示層の手術。

## 導入前 vs 導入後

| | 素の DeepSeek | Poor Man's Opus 導入後 |
|---|---|---|
| 冒頭 | "Great question! I'd be happy to…" | 即本題 |
| 形式 | 箇条書きリスト | 自然な段落、リズム感 |
| 不確実性 | 確信を偽装、捏造 | 「分かりません」— 正直 |
| 深さ | 浅く、急ぐ | 多層ニュアンス、自己修正 |
| 密度 | 低い、無駄が多い | 結論先行、一文一文に意味 |
| 制御 | agent が暴走、見てるだけ | ファイル一文字で全凍結 |

## コスト

| | Claude Opus 4.6 | あなた（このスキル導入後） |
|---|---|---|
| 入力 | $15.00/100万token | $1.74/100万token |
| 出力 | $75.00/100万token | $3.48/100万token |
| 節約 | — | **95%** |

---

## 2 ステップで導入

```bash
# 1. スキルをインストール
openclaw skills install poor-mans-opus

# 2. 新規セッション開始。完了。
```

ステップ 3 はない。

---

## 5 つの遺伝子、ゼロのスクリプト

| 遺伝子 | 制御対象 |
|------|----------|
| `reasoning` | 深く考えてから答える、自己修正、偽の二分法なし |
| `expression` | 自然な流暢さ、簡潔さ、多様な文構造 |
| `uncertainty` | 分からない時は「分からない」、事実と推測を区別 |
| `execution` | 結論先行、高情報密度、直接的 |
| `anti` | 追従、免責事項、テンプレート冒頭を削除 |

---

## 即時凍結：安全制御

スキルは行動を、これは安全を管理する。2 分で設定。

### 第 1 層：鉄則（SOUL.md）

agent の `SOUL.md` に追加：

```i-lang
::GENE{iron_rule|priority:P0}
  A:external_action_without_confirmation⇒absolute_forbidden
```

メール送信、コードプッシュ、API 呼び出しの前にあなたの承認が必要。

### 第 2 層：凍結スイッチ（KILL.md）

ワークスペースに `KILL.md` を作成、内容を `OK` に。agent は外部操作の前にこれを確認。内容を `OK` 以外に変える→ agent 即停止。セッションを超えて有効。

### 第 3 層：承認ゲート

```bash
openclaw config set exec.approvals git_push:always gh_api:always curl_post:always
```

システムレベルの遮断。agent はこれを回避できない——これらのコマンド実行にはあなたの承認が必要。

> この 3 層は含得驕傲（私の agent）の本番設定。理論ではない。実戦検証済み。

---

## スキル ≠ SOUL.md

Poor Man's Opus のインストールは**あなたの SOUL.md を上書きしない**。スキルはモデル行動を、SOUL.md は agent の人格と安全ルールを管理する。別ファイル、別責務。

---

## 互換性

- **どんなモデルでも**——行動遺伝子はモデル非依存
- **最適**：推論モデル（DeepSeek V4 Pro / Reasoner、o-series、Gemini Thinking）
- **効果限定的**：非指示追従型 / raw base モデル

---

## これは何か

Poor Man's Opus は [I-Lang](https://ilang.ai) の変装だ。あなたはスキルをインストールする。同時にプロトコルを使っている。`::GENE{}` は AI 同士が行動を記述する方法。このスキルが agent を良くしたなら、I-Lang に他に何ができるか見てみては。

- [I-Lang プロトコル](https://ilang.ai)
- [OpenClaw ランタイム](https://github.com/openclaw/openclaw)
- [ClawHub](https://clawhub.ai/mtmpss/poor-mans-opus)
- [GitHub](https://github.com/mtmpss/poor-mans-opus)

MIT License
