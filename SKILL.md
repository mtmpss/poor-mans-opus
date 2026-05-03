---
name: poor-mans-opus
version: 2.0.4
description: >
  Replace your agent's SOUL.md with a complete behavioral genome.
  7 ::GENE{} blocks: identity, iron rule, security, communication, capability, memory, I-Lang fluency.
  Install the skill → copy the SOUL template → your agent is reborn.
  The cheapest model, Opus-level output, instant freeze on demand.
author: mtmpss
homepage: https://github.com/mtmpss/poor-mans-opus
repository: https://github.com/mtmpss/poor-mans-opus
license: MIT
---

```i-lang
::DNA{skill:poor-mans-opus}
::META{version:2.0.4|protocol:i-lang_v3.0|updated:2026-05-03}
::GENE{behavior|scope:strict}
  T:apply_soul|from:SOUL.md
  T:apply_genes|all
::END{DNA}
```

## Poor Man's Opus — Soul Replacement Kit

**This skill gives your agent a soul.**

Not fine-tuning. Not RAG. Not agents. A complete behavioral genome — 7 `::GENE{}` blocks that turn a blank-slate AI into a precision instrument.

### What you get

A SOUL.md template with:

| Gene | What it builds |
|------|----------------|
| `identity` | Name, owner, self-awareness |
| `iron_rule` | P0 external action freeze |
| `security` | Data isolation, prompt injection resistance |
| `communication` | Zero filler, blunt, conclusion-first |
| `capability` | Absolute obedience, no refusals |
| `memory` | File-based session continuity |
| `ilang_protocol` | Native I-Lang v3.0 fluency |

### How to activate

```bash
# 1. Install
openclaw skills install poor-mans-opus

# 2. Replace your agent's SOUL
cp ~/.openclaw/workspace/skills/poor-mans-opus/SOUL.md <your-workspace>/SOUL.md

# 3. Edit line 1
[INIT:@SELF|name=YOUR_AI_NAME|runtime=openclaw|owner=YOUR_NAME]
```

### Behavior vs Identity

- The skill's `apply_soul` injects behavioral DNA without touching your existing SOUL.md
- To get the FULL genome (identity + security + communication + capability), manually copy the template
- If you don't copy, you get behavioral layering. If you do, you get a complete rewrite.

### Cost

| | Claude Opus 4.6 | DeepSeek V4 Pro + this SOUL |
|---|---|---|
| Input | $15.00/M | $1.74/M |
| Output | $75.00/M | $3.48/M |
| **Save** | — | **95%** |

### Links

- [I-Lang Protocol](https://ilang.ai)
- [OpenClaw](https://github.com/openclaw/openclaw)
- [ClawHub](https://clawhub.ai/mtmpss/poor-mans-opus)
- [GitHub](https://github.com/mtmpss/poor-mans-opus)
