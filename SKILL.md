---
name: poor-mans-opus
version: 2.0.0
description: >
  Behavioral DNA that elevates any model to Opus-level output quality.
  Protocol: I-Lang v3.0 structured behaviors.
author: mtmpss
homepage: https://github.com/mtmpss/poor-mans-opus
repository: https://github.com/mtmpss/poor-mans-opus
license: MIT
---

```i-lang
::DNA{skill:poor-mans-opus}
::META{version:2.0.0|protocol:i-lang_v3.0|updated:2026-05-03}
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

**DeepSeek Reasoner + I-Lang behavioral DNA = Opus-level output at 3% the cost.**

Model capability is not the bottleneck. Instruction quality is. This skill bridges the gap using I-Lang's structured `::GENE{}` protocol — no fine-tuning, no RAG, no extra infrastructure.

### How it works

Install this skill. It injects behavioral DNA into your agent's prompt context through five targeted genes:

| Gene | What it controls |
|------|-----------------|
| `reasoning` | Deep thinking, nuance, self-correction |
| `expression` | Natural fluency, conciseness, variety |
| `uncertainty` | Honesty about limits, no hallucination |
| `execution` | Conclusion-first, high density, direct |
| `anti` | What NOT to do (sycophancy, templates, hedging) |

No scripts. No runtime. No API calls. Pure instruction optimization.

### Install

```bash
openclaw skills install poor-mans-opus
```

### Compatibility

- **Any model.** The behavioral DNA is model-agnostic.
- **Best ROI on:** reasoning models (DeepSeek Reasoner, o-series, Gemini Thinking)
- **Minimal impact on:** non-instruction-following models

### Cost comparison

| | Claude Opus 4.6 | DeepSeek Reasoner + SOUL |
|---|---|---|
| Input | $15.00 /M tokens | $1.10 /M tokens |
| Output | $75.00 /M tokens | $2.19 /M tokens |
| Quality | Baseline | Comparable |
| Setup | API key | One `openclaw skills install` |

### Links

- [I-Lang Protocol](https://ilang.ai) — structured behavioral specification language
- [OpenClaw](https://github.com/openclaw/openclaw) — agent runtime
- [ClawHub](https://clawhub.ai/mtmpss/poor-mans-opus) — install from hub
