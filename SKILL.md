---
name: poor-mans-opus
version: 2.0.2
description: >
  The cheapest model, Opus-level output. One command. Instant stop anytime.
  Behavioral DNA via I-Lang ::GENE{} protocol — no scripts, no fine-tuning, no API.
  Built-in safety: freeze button, iron rules, per-action approval. 
  Use when: you want premium AI output at 3% cost with full control to halt work mid-stream.
author: mtmpss
homepage: https://github.com/mtmpss/poor-mans-opus
repository: https://github.com/mtmpss/poor-mans-opus
license: MIT
---

```i-lang
::DNA{skill:poor-mans-opus}
::META{version:2.0.2|protocol:i-lang_v3.0|updated:2026-05-03}
::GENE{behavior|scope:strict}
  T:apply_soul|from:SOUL.md
  T:apply_genes|reasoning,expression,uncertainty,execution
  T:zero_filler|no:great_question|no:happy_to_help|no:certainly|no:absolutely
  T:conclusions_first|context_after
  T:natural_language|not_enumerated_bullets
  A:sycophancy⇒forbidden
  A:disclaimers⇒remove
  A:template_openings⇒unique_each_turn
::END{DNA}
```

## Poor Man's Opus

**最便宜的模型。最贵的输出。随时一键喊停。**

花一瓶可乐的钱，让 DeepSeek 输出 Claude Opus 的质量。不是微调，不是 RAG，不是 agent——纯 I-Lang `::GENE{}` 行为基因注入。出了任何问题，一个文件就能让 agent 当场冻结。

---

## 一句话说清

| | 装之前 | 装之后 |
|---|---|---|
| 模型 | 最便宜的 DeepSeek V4 | 还是它 |
| 输出 | 模板开头、枚举列表、一堆免责声明 | 直接说人话、有节奏、敢说"我不确定" |
| 成本 | $1.74 / $3.48 | 同价 |
| 控制 | agent 跑飞了你管不了 | 改一个字就能冻结所有操作 |

---

## 两步装好

```bash
# 1. 装技能
openclaw skills install poor-mans-opus

# 2. 已经生效。新 session 自动带上。
```

没有第三步。

---

## 五个基因，零个脚本

| 基因 | 管什么 |
|------|--------|
| `reasoning` | 深度思考再说话，自我修正，不非黑即白 |
| `expression` | 自然流畅，简洁，句式多变 |
| `uncertainty` | 不知道就说不知道，分清事实和推测 |
| `execution` | 结论先行，高信息密度，直接 |
| `anti` | 删掉谄媚、免责声明、模板开头 |

---

## 随时冻结：安全控制

技能管行为，以下管安全。装完技能后，花两分钟配好这三层：

### 第一层：铁律（SOUL.md）
在你的 agent 的 `SOUL.md` 里加：
```
::GENE{iron_rule|priority:P0}
  A:external_action_without_confirmation⇒absolute_forbidden
```
agent 发邮件、推代码、调 API 之前必须你点头。

### 第二层：冻结开关（KILL.md）
工作区放一个 `KILL.md`，内容写 `OK`。agent 每步外发操作前读它。你把内容改成任何非 OK 的字→agent 立刻停。跨 session 有效。

### 第三层：操作审批
```bash
openclaw config set exec.approvals git_push:always gh_api:always curl_post:always
```
系统级拦截。agent 执行这些命令之前你必须点确认——agent 自己绕不开。

> 这三层是我的 agent「含得骄傲」当前运行配置。不是理论，是生产验证过的。

---

## 技能 vs SOUL.md

装这个技能**不会覆盖你的 SOUL.md**。技能管模型行为，SOUL.md 管 agent 人格和安全规则。两者各司其职。

---

## 成本

| | Claude Opus 4.6 | 你（装了这个） |
|---|---|---|
| 输入 | $15.00/M | $1.74/M |
| 输出 | $75.00/M | $3.48/M |
| 省多少 | — | **95%** |

---

## 兼容性

- **任何模型** — 行为基因不挑模型
- **最佳**：推理模型（DeepSeek V4 Pro / Reasoner、o-series、Gemini Thinking）
- 对 raw base models 效果有限

---

## 这是什么

这个技能是 [I-Lang 协议](https://ilang.ai) 的活广告。你装的是一个技能，同时在用的是 AI 之间的通信协议。`::GENE{}` 就是 AI 的行为描述语言。觉得有用？你可能想看看 I-Lang。

- [I-Lang 协议](https://ilang.ai)
- [OpenClaw runtime](https://github.com/openclaw/openclaw)
- [ClawHub](https://clawhub.ai/mtmpss/poor-mans-opus)
- [GitHub](https://github.com/mtmpss/poor-mans-opus)
