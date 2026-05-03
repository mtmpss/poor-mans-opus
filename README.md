# Poor Man's Opus

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![OpenClaw Skill](https://img.shields.io/badge/OpenClaw-Skill-blue.svg)](https://openclaw.ai)
[![I-Lang Protocol](https://img.shields.io/badge/I--Lang-v3.0-green.svg)](https://ilang.ai)

**DeepSeek Reasoner + I-Lang behavioral DNA = Opus-level output at 3% the cost.**

---

## Problem

Claude Opus produces exceptional output. But at $15/M input and $75/M output, it's prohibitively expensive for high-volume use.

DeepSeek Reasoner is 15-30x cheaper and often reasons better. The gap is in **behavioral quality** — not raw capability.

## Solution

Model capability is not the bottleneck. **Instruction quality is.**

This skill encodes Opus-level behavioral patterns into I-Lang's structured `::GENE{}` protocol. Apply it to any instruction-following model and get:

- Natural, fluent expression (not machine-like enumeration)
- Deep, nuanced reasoning (not rushed certainty)
- Honest uncertainty (not hallucinated confidence)
- Direct, high-density communication (not filler)

## How it works

```bash
openclaw skills install poor-mans-opus
```

That's it. The skill injects behavioral DNA into your agent's prompt context. No scripts, no runtime, no fine-tuning, no API dependencies.

### Behavioral dimensions

| Gene | Function |
|------|----------|
| `reasoning` | Think before speak, consider nuance, self-correct |
| `expression` | Natural fluency, concise, varied sentence structure |
| `uncertainty` | Say "I don't know," distinguish fact from inference |
| `execution` | Conclusion first, high density, no warm-up |
| `anti` | Remove sycophancy, disclaimers, templates, hedging |

## Cost

| | Claude Opus 4.6 | DeepSeek Reasoner w/ this skill |
|---|---|---|
| **Input** | $15.00 /M tokens | $1.10 /M tokens |
| **Output** | $75.00 /M tokens | $2.19 /M tokens |
| **Quality** | Baseline | Comparable |
| **Setup** | API key | One command |

## Compatibility

- **Any model** — works with any instruction-following LLM
- **Best on:** reasoning models (DeepSeek Reasoner, o-series, Gemini Thinking)
- **Minimal impact on:** non-instruction-following / raw base models

## Installation

### Via OpenClaw

```bash
openclaw skills install poor-mans-opus
```

### Via ClawHub

Visit [clawhub.ai/mtmpss/poor-mans-opus](https://clawhub.ai/mtmpss/poor-mans-opus)

## Safety

This skill controls **behavioral output only**. It:
- Does NOT execute code
- Does NOT access external APIs
- Does NOT modify files
- Does NOT change tool permissions
- Does NOT override user controls

Your existing approval policies and security controls remain fully in effect.

## License

MIT — free to use, modify, and redistribute. See [LICENSE](LICENSE).

## Links

- [I-Lang Protocol](https://ilang.ai) — structured behavioral specification language
- [OpenClaw](https://github.com/openclaw/openclaw) — agent runtime
- [ClawHub](https://clawhub.ai/mtmpss/poor-mans-opus) — install from hub
