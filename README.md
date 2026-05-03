# Poor Man's Opus

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![OpenClaw Skill](https://img.shields.io/badge/OpenClaw-Skill-blue.svg)](https://openclaw.ai)
[![I-Lang Protocol](https://img.shields.io/badge/I--Lang-v3.0-green.svg)](https://ilang.ai)

**最便宜的模型。最贵的输出。随时一键喊停。**

DeepSeek V4 Pro + I-Lang 行为基因 = Opus 级别输出质量。一条命令装好，一个字就能冻结。省 95% 的钱，多 100% 的控制。

---

## 为什么它能工作

模型能力不是瓶颈。**指令质量才是。**

DeepSeek V4 Pro 的推理能力在很多 benchmark 上超过 Opus，但输出「感觉」差一截——模板开头、枚举列表、满篇免责声明。

Opus 的「感觉」来自行为——语感、节奏、nuance、诚实度。这些不靠模型参数，靠指令。

我们把 Opus 的行为模式反编译成 I-Lang 基因，注入 DeepSeek。DeepSeek 还是 DeepSeek，穿的衣服变了。没有微调，没有 RAG，没有 API 调用。纯指令层手术。

## 装前 vs 装后

| | 装之前 | 装之后 |
|---|---|---|
| 开头 | "Great question! I'd be happy to…" | 直接进入主题 |
| 格式 | 枚举式分点列表 | 自然段落，有节奏 |
| 不确定性 | 假装确定，编造 | 诚实说「我不确定」 |
| 细节 | 浅尝辄止 | 多层 nuance，自我修正 |
| 信息密度 | 低，充满废话 | 结论先行，每句有信息量 |
| 控制 | agent 跑飞了你管不了 | 改一个文件就能冻结 |

## 成本

| | Claude Opus 4.6 | 你（装了这个） |
|---|---|---|
| 输入 | $15.00/M tokens | $1.74/M tokens |
| 输出 | $75.00/M tokens | $3.48/M tokens |
| 省多少 | — | **95%** |

---

## 两步装好

```bash
# 1. 装技能
openclaw skills install poor-mans-opus

# 2. 开新 session。已经生效。
```

没有第三步。

---

## 随时冻结：安全控制

技能管行为，安全管失控。花两分钟配好三层保护：

### 第一层：铁律（SOUL.md）

```i-lang
::GENE{iron_rule|priority:P0}
  A:external_action_without_confirmation⇒absolute_forbidden
```

agent 发邮件、推代码、调 API 之前必须你点头。

### 第二层：冻结开关（KILL.md）

工作区放 `KILL.md`，内容写 `OK`。agent 每步外发操作前读它。你把内容改成任何非 `OK` 的字→agent 立刻停。跨 session 有效。

### 第三层：操作审批

```bash
openclaw config set exec.approvals git_push:always gh_api:always curl_post:always
```

系统级拦截——agent 执行这些命令前你必须点确认。agent 自己绕不开。

> 这三层是含得骄傲（我的 agent）的生产配置。不是理论，验证过的。

---

## 技能 vs SOUL.md

装 poor-mans-opus **不会覆盖你的 SOUL.md**。技能管模型行为，SOUL.md 管 agent 人格和安全规则。各管各的。

---

## 兼容性

- **任何模型**——行为基因不挑模型
- **最佳 ROI**：推理模型（DeepSeek V4 Pro / Reasoner、o-series、Gemini Thinking）
- 对 raw base models 效果有限

---

## 这是什么

Poor Man's Opus 是 [I-Lang 协议](https://ilang.ai) 的**活广告**。你装的是一个技能，但同时在用的是 AI 之间的通信协议——`::GENE{}` 就是 AI 的行为描述语言。觉得有用？你可能想看看 I-Lang。

- [I-Lang 协议](https://ilang.ai)
- [OpenClaw runtime](https://github.com/openclaw/openclaw)
- [ClawHub 技能市场](https://clawhub.ai)

MIT License
