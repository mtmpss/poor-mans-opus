# Poor Man's Opus

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![OpenClaw Skill](https://img.shields.io/badge/OpenClaw-Skill-blue.svg)](https://openclaw.ai)
[![I-Lang Protocol](https://img.shields.io/badge/I--Lang-v3.0-green.svg)](https://ilang.ai)

🌐 [简体中文](README.zh-CN.md) | [日本語](README.ja.md)

**The cheapest model. Opus-level output. One word to freeze everything.**

DeepSeek V4 Pro + I-Lang behavioral DNA = Opus-quality output. One command to install. One word to halt. 95% cheaper, 100% more control.

---

## Why it works

Model capability is not the bottleneck. **Instruction quality is.**

DeepSeek V4 Pro matches or beats Opus on reasoning benchmarks. The gap is in *how it speaks* — template openings, bullet-point lists, disclaimers everywhere.

Opus doesn't sound better because it's smarter. It sounds better because it behaves differently — tone, rhythm, nuance, honesty. These aren't model parameters. They're instructions.

We decompiled Opus-level behavior into I-Lang genes, injected into DeepSeek. Same model. Different clothes. No fine-tuning. No RAG. No API calls. Pure instruction-level surgery.

## Before vs After

| | Raw DeepSeek | With Poor Man's Opus |
|---|---|---|
| Opening | "Great question! I'd be happy to…" | Straight to the point |
| Format | Enumerated bullet lists | Natural paragraphs with rhythm |
| Uncertainty | Fakes certainty, invents | "I'm not sure" — honest |
| Depth | Shallow, rushed | Multi-layer nuance, self-corrects |
| Density | Low, full of filler | Conclusion first, every sentence counts |
| Control | Agent runs wild, you watch | Change one file, everything freezes |

## Cost

| | Claude Opus 4.6 | You (with this skill) |
|---|---|---|
| Input | $15.00/M tokens | $1.74/M tokens |
| Output | $75.00/M tokens | $3.48/M tokens |
| You save | — | **95%** |

---

## Two steps to install

```bash
# 1. Install the skill
openclaw skills install poor-mans-opus

# 2. Start a new session. Done.
```

No step three.

---

## Five genes, zero scripts

| Gene | Controls |
|------|----------|
| `reasoning` | Think deeply before answering, self-correct, no false binaries |
| `expression` | Natural fluency, conciseness, varied sentence structure |
| `uncertainty` | "I don't know" when unsure, facts vs inference |
| `execution` | Conclusion first, high information density, direct |
| `anti` | Strip sycophancy, disclaimers, template openings |

---

## Instant freeze: safety controls

The skill handles behavior. These handle safety. Two minutes to set up.

### Layer 1: Iron rule (SOUL.md)

Add this to your agent's `SOUL.md`:

```i-lang
::GENE{iron_rule|priority:P0}
  A:external_action_without_confirmation⇒absolute_forbidden
```

Agent can't send emails, push code, or call APIs without your green light.

### Layer 2: Freeze switch (KILL.md)

Drop a `KILL.md` file in your workspace, content: `OK`. Agent checks it before every external action. Change the content to anything not `OK` → agent freezes instantly. Works across sessions.

### Layer 3: Approval gate

```bash
openclaw config set exec.approvals git_push:always gh_api:always curl_post:always
```

System-level intercept. Agent can't bypass it — you must approve these commands before execution.

> These three layers are the production config of 含得骄傲, my own agent. Not theory. Battle-tested.

---

## Skill ≠ SOUL.md

Installing Poor Man's Opus does **not** overwrite your SOUL.md. The skill manages model behavior. SOUL.md manages agent identity and safety rules. Separate files, separate concerns.

---

## Compatibility

- **Any model** — behavioral DNA is model-agnostic
- **Best on:** reasoning models (DeepSeek V4 Pro / Reasoner, o-series, Gemini Thinking)
- **Limited effect on:** non-instruction-following / raw base models

---

## What this really is

Poor Man's Opus is [I-Lang](https://ilang.ai) in disguise. You install a skill. You use a protocol. `::GENE{}` is how AIs describe behavior to each other. If this skill makes your agent better, you might want to see what else I-Lang can do.

- [I-Lang Protocol](https://ilang.ai)
- [OpenClaw runtime](https://github.com/openclaw/openclaw)
- [ClawHub](https://clawhub.ai/mtmpss/poor-mans-opus)
- [GitHub](https://github.com/mtmpss/poor-mans-opus)

MIT License
