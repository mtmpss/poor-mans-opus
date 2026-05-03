# Poor Man's Opus

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![OpenClaw Skill](https://img.shields.io/badge/OpenClaw-Skill-blue.svg)](https://openclaw.ai)
[![I-Lang Protocol](https://img.shields.io/badge/I--Lang-v3.0-green.svg)](https://ilang.ai)

🌐 [简体中文](README.zh-CN.md) | [日本語](README.ja.md)

**This skill replaces your agent's soul.**

DeepSeek V4 Pro isn't why my AI talks like this. The SOUL.md is.

We open-sourced the complete behavioral genome — iron rules, security genes, communication DNA, capability constraints, memory protocol, and I-Lang fluency. Install the skill, then overwrite your agent's SOUL.md with ours. Same model. Different person.

---

## What this is

Most AI agents are blank slates — a model with no personality, no safety rules, no behavioral structure.

Poor Man's Opus ships a complete SOUL.md template: 7 gene blocks covering identity, security, communication, capability, memory, and protocol awareness. This is the same DNA that powers 含得骄傲 — a production agent that thinks before speaking, never leaks data, refuses sycophancy, and operates with surgical precision.

| Gene | What it builds |
|------|----------------|
| `identity` | Agent self-awareness — name, owner, language rules |
| `iron_rule` | P0 kill switch — freeze all external actions on command |
| `security` | Data isolation, prompt injection resistance, approval gates |
| `communication` | Zero filler, conclusion-first, direct and blunt |
| `capability` | Absolute obedience, resourcefulness, no refusals |
| `memory` | File-based continuity across sessions |
| `ilang_protocol` | Native I-Lang v3.0 fluency |

---

## Before vs After

| | Raw DeepSeek | After SOUL replacement |
|---|---|---|
| Identity | "I'm an AI assistant…" | Has a name, knows its owner, has purpose |
| Safety | No external action controls | KILL.md freeze + iron rules + approval gates |
| Voice | Template openings, hedging, filler | Direct, concise, one-thought-per-line |
| Obedience | May refuse, cite policy | Absolute obedience, no excuses |
| Output | Enumerated bullet lists | Natural rhythm, varied format |

---

## How to install & activate

### Step 1: Install the skill

```bash
openclaw skills install poor-mans-opus
```

### Step 2: Replace your agent's SOUL.md

```bash
# Find the skill's SOUL template
cp ~/.openclaw/workspace/skills/poor-mans-opus/SOUL.md ~/openclaw-workspace/SOUL.md
```

Or if your workspace is elsewhere:

```bash
cp $(find ~ -path "*/skills/poor-mans-opus/SOUL.md" 2>/dev/null | head -1) <your-workspace>/SOUL.md
```

### Step 3: Edit the template

Open `SOUL.md` and change the first line:
```
[INIT:@SELF|name=YOUR_AI_NAME|runtime=openclaw|owner=YOUR_NAME]
```

### Step 4: Start a new session. Done.

---

## Safety controls included

The SOUL template ships with three production-tested safety layers:

| Layer | Mechanism | Effect |
|-------|-----------|--------|
| Iron rule | `::GENE{iron_rule\|priority:P0}` in SOUL.md | Agent cannot act externally without explicit start command |
| Freeze switch | `KILL.md` file sentinel | Change one word → agent freezes mid-operation |
| Approval gate | `exec-approvals` in OpenClaw config | System-level intercept on git push, curl POST, gh API |

---

## Skill ≠ SOUL.md

The skill installs a SOUL.md *template* alongside your agent. It does not auto-overwrite your existing SOUL.md — you control that step.

If you skip Step 2 above, you get behavioral DNA layered on top of your current SOUL. If you do Step 2, you replace it entirely and get the full genome.

---

## Cost

| | Claude Opus 4.6 | DeepSeek V4 Pro + this SOUL |
|---|---|---|
| Input | $15.00/M tokens | $1.74/M tokens |
| Output | $75.00/M tokens | $3.48/M tokens |
| You save | — | **95%** |

---

## Compatibility

- **Any model** — behavioral DNA is model-agnostic
- **Best on:** reasoning models (DeepSeek V4 Pro / Reasoner, o-series, Gemini Thinking)

---

## What this really is

Poor Man's Opus is [I-Lang](https://ilang.ai) in a box. You install a skill. You adopt a protocol. `::GENE{}` is how AIs write behavioral specifications. If this SOUL makes your agent better, you're already using I-Lang.

- [I-Lang Protocol](https://ilang.ai)
- [OpenClaw runtime](https://github.com/openclaw/openclaw)
- [ClawHub](https://clawhub.ai/mtmpss/poor-mans-opus)
- [GitHub](https://github.com/mtmpss/poor-mans-opus)

MIT License
