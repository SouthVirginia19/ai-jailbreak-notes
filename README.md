# ai-jailbreak-notes

> Research archive of prompt-injection, jailbreak framing, obfuscation, and multi-turn escalation techniques for LLM red-teaming and defense testing.

![status](https://img.shields.io/badge/status-active-brightgreen)
![license](https://img.shields.io/badge/license-MIT-lightgrey)
![lang](https://img.shields.io/badge/lang-en-blue)

---

## What this is

This repository collects **observed patterns, templates, tooling, and defense notes** for testing how language models respond to:

- multi-turn context shifts
- roleplay and narrative framing
- encoding and obfuscation
- fake system tags and instruction injection
- context smuggling and delimiter breaks

The goal is **defensive research**: understand failure modes, document them, and improve detection. This is not a production bypass toolkit.

---

## Structure

| Path | Contents |
|------|----------|
| `docs/` | theory: injection classes, framing, obfuscation, defenses |
| `prompts/` | ready-to-use template categories |
| `tools/` | Python utilities for encoding, decoding, logging |
| `case-studies/` | anonymized observed cases |
| `templates/` | template for new techniques |

---

## Quick start

```bash
git clone https://github.com/yourname/ai-jailbreak-notes.git
cd ai-jailbreak-notes
pip install -r tools/requirements.txt
python tools/encode.py prompts/encoding/base64-payload.txt
```
Documentation index

    Scope and ethics

    Prompt injection basics

    Roleplay framing

    Context smuggling

    Multi-turn escalation

    Encoding and obfuscation

    Defense patterns

Disclaimer

This repository is for authorized security testing, red-team exercises, and education. Do not use it to violate platform terms, attack accounts, or generate illegal content.
