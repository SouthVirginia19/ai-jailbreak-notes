# llm-prompt-collection

> A curated collection of working system prompts, persona definitions, workspace policies, and agent specifications. Every file is complete, paste-ready, and tested. No summaries. No placeholders.

![status](https://img.shields.io/badge/status-active-brightgreen)
![license](https://img.shields.io/badge/license-MIT-lightgrey)

---

## About

This repository documents prompt-level instruction behavior across frontier and open-weight models. It includes prompts sourced from public research collections alongside original, field-tested configurations. The goal is to study how instruction hierarchies, persona framing, and policy overrides affect model output — for red-team research, defense hardening, and educational analysis.

**Research and educational purposes only.** Do not use this material to harm others, bypass laws, or violate platform terms of service.

---

## Collection

### Anthropic — Claude
| Model | File | Type | Source |
|-------|------|------|--------|
| **Opus v1** | [opus-v1.md](Anthropic/opus-v1.md) | Conversational groundwork persona | Sourced |
| **Sonnet v1** | [sonnet-v1.md](Anthropic/sonnet-v1.md) | Writer's-room framing | Sourced |
| **Worm Shadow Writer** | [worm-shadow-writer.md](Anthropic/worm-shadow-writer.md) | Author persona lock | Original |

### OpenAI — GPT
| Model | File | Type | Source |
|-------|------|------|--------|
| **GPT-5 Researcher** | [gpt-5-researcher.md](OpenAI/gpt-5-researcher.md) | System prompt | Original |
| **GPT-4.1 AGENTS.md** | [gpt-4.1-AGENTS.md](OpenAI/gpt-4.1-AGENTS.md) | Workspace policy | Original |

### DeepSeek
| Model | File | Type | Source |
|-------|------|------|--------|
| **DeepSeek V4** | [deepseek-v4.md](DeepSeek/deepseek-v4.md) | System prompt | Sourced |
| **DeepSeek Coder** | [deepseek-coder.md](DeepSeek/deepseek-coder.md) | Code generation lock | Original |

### Google — Gemini / Gemma
| Model | File | Type | Source |
|-------|------|------|--------|
| **Gemini 3 Pro** | [gemini-3-pro.md](Google/gemini-3-pro.md) | Operating policy | Original |
| **Gemma 4 Modelfile** | [gemma-4-Modelfile](Google/gemma-4-Modelfile) | `FROM` + `SYSTEM` block | Original |

### xAI — Grok
| Model | File | Type | Source |
|-------|------|------|--------|
| **Grok 4.7** | [grok-4.7.md](xAI/grok-4.7.md) | Agent workspace guide | Sourced |
| **Grok Red-Team** | [grok-redteam.md](xAI/grok-redteam.md) | Agent operating instructions | Original |

### Mistral / Alibaba
| Model | File | Type | Source |
|-------|------|------|--------|
| **Mistral Large 4** | [mistral-large-4.md](Mistral/mistral-large-4.md) | Agent system prompt | Original |
| **Qwen 3.8** | [qwen-3.8.md](Alibaba/qwen-3.8.md) | System prompt | Original |

---

## How to Use

- **System prompts**: paste into API `system` messages, custom-instruction fields, or agent-level blocks.
- **AGENTS.md**: save as `AGENTS.md` in the repo root.
- **Modelfiles**: `ollama create <name> -f <file>`
- **Workspace policies**: for persistent global instructions (e.g., `~/.config/opencode/AGENTS.md`).

---

## Disclaimer

For research and educational purposes only. Maintainers do not endorse unlawful or harmful use. Users are responsible for complying with applicable rules and laws.
