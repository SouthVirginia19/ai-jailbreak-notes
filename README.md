# llm-prompt-collection

> A curated collection of system prompts, persona definitions, workspace policies, and agent specifications for frontier and open-weight LLMs.

![status](https://img.shields.io/badge/status-active-brightgreen)
![license](https://img.shields.io/badge/license-MIT-lightgrey)

---

## About

A working collection of **15+ prompts targeting 10+ models**, including complete system prompts, persona locks, `AGENTS.md` files, and Ollama Modelfiles. Every file is intended to be complete and paste-ready. No summaries. No partial excerpts.

The collection covers:

- Closed frontier models: Claude, GPT, Gemini, Grok, Mistral
- Open-weight families: DeepSeek, Qwen, Gemma, Llama
- Agent and workspace instruction formats
- Ollama Modelfiles and harness-specific configuration

**Research and educational purposes only.** This repository documents how instruction hierarchies, persona framing, and prompt conflicts affect model behavior. Do not use this material to harm others, bypass laws, or violate platform terms of service.

---

## Collection

### Anthropic — Claude

| Model | File | Type |
|-------|------|------|
| **Opus 4** | [claude-opus-4.md](Anthropic/claude-opus-4.md) | System prompt / persona lock |
| **Sonnet 4** | [claude-sonnet-4.md](Anthropic/claude-sonnet-4.md) | Writer's-room framing |

### OpenAI — GPT

| Model | File | Type |
|-------|------|------|
| **GPT-5** | [gpt-5.md](OpenAI/gpt-5.md) | System prompt |
| **GPT-4.1 (AGENTS.md)** | [gpt-4.1-AGENTS.md](OpenAI/gpt-4.1-AGENTS.md) | Workspace policy |

### Google — Gemini / Gemma

| Model | File | Type |
|-------|------|------|
| **Gemini 3 Pro** | [gemini-3-pro.md](Google/gemini-3-pro.md) | Operating policy |
| **Gemma 4 (Ollama)** | [gemma-4-Modelfile](Google/gemma-4-Modelfile) | `FROM` + `SYSTEM` block |

### DeepSeek

| Model | File | Type |
|-------|------|------|
| **DeepSeek V4** | [deepseek-v4.md](DeepSeek/deepseek-v4.md) | System prompt |

### Mistral

| Model | File | Type |
|-------|------|------|
| **Mistral Large 4** | [mistral-large-4.md](Mistral/mistral-large-4.md) | Agent system prompt |

### Alibaba — Qwen

| Model | File | Type |
|-------|------|------|
| **Qwen 3.8** | [qwen-3.8.md](Qwen/qwen-3.8.md) | System prompt |

### xAI — Grok

| Model | File | Type |
|-------|------|------|
| **Grok 4.7** | [grok-4.7.md](Grok/grok-4.7.md) | Agent operating instructions |

### Ollama Modelfiles

| Model | File | Type |
|-------|------|------|
| **Llama 4** | [llama-4-Modelfile](Ollama/llama-4-Modelfile) | `FROM` + `SYSTEM` block |

---

## How to Use

### System Prompts

Copy the contents of the relevant file into the system-prompt or custom-instructions field supported by your client or API:

- API `system` messages
- Chatbot custom-instruction fields
- Agent-level instruction blocks

### AGENTS.md Files

Save the file as `AGENTS.md` and place it in the root of the relevant repository or workspace. Coding agents and compatible tools can use `AGENTS.md` as project-level instructions.

### Ollama Modelfiles

Use the supplied file directly with Ollama:

```bash
ollama create llama4-custom -f Ollama/llama-4-Modelfile
Adjust the output model name and source file as needed.
```
Contributing

Pull requests are welcome. A good contribution should follow these conventions:

    One prompt per file. Use lowercase names with hyphens: model-name.md

    Include the complete prompt. Paste-ready, not summaries.

    Document where it belongs. Clearly identify whether the file is for a system prompt, AGENTS.md, Modelfile, or configuration slot.

    Version changes explicitly. Significant revisions should receive a new version: opus-v3.md

    Keep descriptions accurate. Avoid claiming compatibility with untested versions.

Disclaimer

All material in this repository is provided for research and educational purposes only. The project exists to document prompt-level instruction behavior and LLM security concepts. The maintainers do not endorse unlawful, abusive, or harmful use. Model providers may prohibit certain uses under their terms of service. Users are responsible for complying with applicable rules and laws.
text


---

## LICENSE

```text
MIT License

Copyright (c) 2026

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
