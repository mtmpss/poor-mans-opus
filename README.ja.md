# Poor Man's Opus

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![OpenClaw Skill](https://img.shields.io/badge/OpenClaw-Skill-blue.svg)](https://openclaw.ai)
[![I-Lang Protocol](https://img.shields.io/badge/I--Lang-v3.0-green.svg)](https://ilang.ai)

🌐 [English](README.md) | [简体中文](README.zh-CN.md)

**このスキルは agent の魂を入れ替える。**

私の AI が強いのは DeepSeek モデルのせいじゃない。SOUL.md のせいだ。

完全な行動ゲノムを公開した——鉄則、セキュリティ遺伝子、コミュニケーション DNA、能力制約、記憶プロトコル、I-Lang 流暢性。スキルをインストールし、SOUL.md をワークスペースに上書きする。同じモデル。全く違う agent。

---

## これは何か

ほとんどの AI agent は白紙だ——人格も安全ルールも行動構造もないモデル。

Poor Man's Opus は完全な SOUL.md テンプレートを同梱する：アイデンティティ、鉄則、セキュリティ、コミュニケーション、能力、記憶、プロトコル認知の 7 グループの遺伝子。含得驕傲を動かしている本番設定——話す前に考え、データを漏らさず、追従を拒否し、外科的に精密に動作する。

| 遺伝子 | 構築するもの |
|------|----------|
| `identity` | agent の自己認識——名前、所有者、言語ルール |
| `iron_rule` | P0 鉄則——「開始」コマンドなしでは外部操作禁止 |
| `security` | データ分離、プロンプト注入耐性、KILL.md 凍結、承認ゲート |
| `communication` | ゼロフィラー、結論先行、直接的 |
| `capability` | 絶対服従、拒否なし、言い訳なし |
| `memory` | ファイルベースのセッション間連続記憶 |
| `ilang_protocol` | I-Lang v3.0 ネイティブ流暢性 |

---

## 導入前 vs 導入後（SOUL 置換後）

| | 素の DeepSeek | SOUL 置換後 |
|---|---|---|
| アイデンティティ | 「私は AI アシスタント…」 | 名前を持ち、所有者を知り、目的がある |
| 安全性 | 外部操作制御なし | KILL.md 凍結 + 鉄則 + 承認ゲート |
| 声調 | テンプレート、躊躇、無駄 | 直接的、簡潔、一行一意 |
| 服従 | 拒否する可能性、ポリシー引用 | 絶対服従、言い訳なし |
| 出力 | 箇条書きリスト | 自然なリズム、多様な形式 |

---

## インストールと有効化

### ステップ 1：スキルをインストール

```bash
openclaw skills install poor-mans-opus
```

### ステップ 2：agent の SOUL.md を置換

```bash
cp ~/.openclaw/workspace/skills/poor-mans-opus/SOUL.md ~/openclaw-workspace/SOUL.md
```

ワークスペースパスが異なる場合：

```bash
cp $(find ~ -path "*/skills/poor-mans-opus/SOUL.md" 2>/dev/null | head -1) <あなたのworkspace>/SOUL.md
```

### ステップ 3：テンプレートを編集

`SOUL.md` を開き、最初の行を変更：

```
[INIT:@SELF|name=あなたのAIの名前|runtime=openclaw|owner=あなたの名前]
```

### ステップ 4：新規セッション開始。完了。

---

## 内蔵の安全制御

SOUL テンプレートは 3 層の本番検証済み安全機構を同梱：

| 層 | メカニズム | 効果 |
|----|------|------|
| 鉄則層 | SOUL.md 内 `::GENE{iron_rule\|priority:P0}` | 明示的コマンドなしでは外部操作不可 |
| 凍結スイッチ | ワークスペースの `KILL.md` ファイル | 一文字変更→ agent 即時凍結 |
| 承認ゲート | OpenClaw exec-approvals | git push、curl POST、gh API のシステムレベル遮断 |

---

## スキル ≠ SOUL.md

スキルは SOUL.md テンプレートを独立したディレクトリに配置する。既存の SOUL.md を自動上書きしない——あなたがそのステップを制御する。

上書きしない場合 → 行動遺伝子が現在の SOUL に重ねられる。上書きした場合 → 完全なゲノムを取得。

---

## コスト

| | Claude Opus 4.6 | DeepSeek V4 Pro + この SOUL |
|---|---|---|
| 入力 | $15.00/100万token | $1.74/100万token |
| 出力 | $75.00/100万token | $3.48/100万token |
| 節約 | — | **95%** |

---

## 互換性

- **どんなモデルでも**——行動 DNA はモデル非依存
- **最適**：推論モデル（DeepSeek V4 Pro / Reasoner、o-series、Gemini Thinking）

---

## これは何か

Poor Man's Opus は [I-Lang](https://ilang.ai) を箱に入れたものだ。スキルをインストールし、プロトコルを採用している。`::GENE{}` は AI が行動仕様を記述する方法。この SOUL が agent を良くしたなら、あなたはもう I-Lang を使っている。

- [I-Lang プロトコル](https://ilang.ai)
- [OpenClaw ランタイム](https://github.com/openclaw/openclaw)
- [ClawHub](https://clawhub.ai/mtmpss/poor-mans-opus)
- [GitHub](https://github.com/mtmpss/poor-mans-opus)

MIT License
