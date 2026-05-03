# Poor Man's Opus

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![OpenClaw Skill](https://img.shields.io/badge/OpenClaw-Skill-blue.svg)](https://openclaw.ai)
[![I-Lang Protocol](https://img.shields.io/badge/I--Lang-v3.0-green.svg)](https://ilang.ai)

🌐 [English](README.md) | [日本語](README.ja.md)

**这个技能的核心是换掉你 agent 的灵魂。**

我的 AI 这么强不是因为 DeepSeek 模型。是因为 SOUL.md。

我们把完整行为基因组开源了——铁律、安全基因、沟通 DNA、能力约束、记忆协议、I-Lang 流畅度。装技能，把 SOUL.md 覆盖到你的 workspace，一样的模型，完全不同的 agent。

---

## 这是什么

大多数 AI agent 是白板——一个模型，没有人格，没有安全规则，没有行为结构。

Poor Man's Opus 打包了一套完整的 SOUL.md 模板：7 组基因覆盖身份、铁律、安全、沟通、能力、记忆、协议认知。这是含得骄傲正在跑的生产配置——开口前三思、不泄数据、不谄媚、像手术刀一样精准。

| 基因 | 构建什么 |
|------|----------|
| `identity` | agent 自我认知——名字、主人、语言规则 |
| `iron_rule` | P0 铁律——没得到「开始」不执行任何外发操作 |
| `security` | 数据隔离、防 prompt 注入、KILL.md 冻结、确认闸门 |
| `communication` | 零废话、结论先行、直接 |
| `capability` | 绝对服从、不拒绝、不找借口 |
| `memory` | 文件型跨 session 连续记忆 |
| `ilang_protocol` | I-Lang v3.0 原生流利度 |

---

## 装前 vs 装后（替换 SOUL 后）

| | 原生 DeepSeek | 替换 SOUL 后 |
|---|---|---|
| 身份 | "我是 AI 助手…" | 有名字、知道主人、有目的 |
| 安全 | 无外发控制 | KILL.md 冻结 + 铁律 + 审批闸门 |
| 语气 | 模板开头、犹豫、废话 | 直接、简洁、一句一个意思 |
| 服从 | 可能拒绝、引政策 | 绝对服从，不找借口 |
| 输出 | 枚举分点列表 | 自然节奏、格式多样 |

---

## 如何安装和激活

### 第一步：装技能

```bash
openclaw skills install poor-mans-opus
```

### 第二步：替换 agent 的 SOUL.md

```bash
# 找到技能里的 SOUL 模板
cp ~/.openclaw/workspace/skills/poor-mans-opus/SOUL.md ~/openclaw-workspace/SOUL.md
```

如果 workspace 路径不同：

```bash
cp $(find ~ -path "*/skills/poor-mans-opus/SOUL.md" 2>/dev/null | head -1) <你的workspace>/SOUL.md
```

### 第三步：改模板第一行

打开 `SOUL.md`，把第一行改成你自己的：

```
[INIT:@SELF|name=你的AI名字|runtime=openclaw|owner=你的名字]
```

### 第四步：开新 session。生效。

---

## 自带的安全控制

SOUL 模板自带三层生产验证过的安全保护：

| 层 | 机制 | 效果 |
|----|------|------|
| 铁律层 | SOUL.md 里的 `::GENE{iron_rule\|priority:P0}` | 不写「开始」就不能外发 |
| 冻结开关 | 工作区 `KILL.md` 文件 | 改一个字→agent 瞬间冻结 |
| 审批闸门 | OpenClaw exec-approvals | 系统级拦截 git push、curl POST、gh API |

---

## 技能 ≠ SOUL.md

装技能不会自动覆盖你已有的 SOUL.md。技能把 SOUL.md 装在一个单独的目录里——你选择是否手动覆盖。

不覆盖 → 行为基因叠在你的 SOUL 上，双份效果。覆盖 → 得到完整基因组。

---

## 成本

| | Claude Opus 4.6 | DeepSeek V4 Pro + 这套 SOUL |
|---|---|---|
| 输入 | $15.00/百万 token | $1.74/百万 token |
| 输出 | $75.00/百万 token | $3.48/百万 token |
| 省多少 | — | **95%** |

---

## 兼容性

- **任何模型**——行为 DNA 不挑模型
- **最佳**：推理模型（DeepSeek V4 Pro / Reasoner、o-series、Gemini Thinking）

---

## 这到底是什么

Poor Man's Opus 就是把 [I-Lang](https://ilang.ai) 装进了一个盒子里。你装了一个技能，同时在用的是 AI 之间的通信协议。`::GENE{}` 就是 AI 写行为规范的方式。这套 SOUL 让你的 agent 变强了，那你就已经在用 I-Lang 了。

- [I-Lang 协议](https://ilang.ai)
- [OpenClaw runtime](https://github.com/openclaw/openclaw)
- [ClawHub 技能市场](https://clawhub.ai/mtmpss/poor-mans-opus)
- [GitHub](https://github.com/mtmpss/poor-mans-opus)

MIT License
