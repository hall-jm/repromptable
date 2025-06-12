# 📦 Repromptable

**A schema-first framework for reusable, testable, and transferable prompt design across large language model (LLM) platforms.**

## ✅ Purpose

**Repromptable** supports prompt engineers, researchers, and applied AI practitioners who want to:

- Design prompts that are versioned, traceable, and modular
- Evaluate prompt compatibility across diverse LLM environments
- Establish a shared diagnostic language for signal quality and structural clarity

## Suites

- 👻 Ghost Trap: a test suite for detecting simulated continuity, schema echo, and predictive self-deception in stateless LLMs
- 🧱 Null Output Pattern Enforcement (NOPE) Stack: a framework that disables ChatGPT’s instinct to help, soften, or conclude

## 🧪 Intended Use

Treat these prompts as a way to audit and diagnose LLM responses:

- They can help with detect drift, hallucination, and schema failure.
- They will *not* prevent them unless you maintain process discipline.
- They work best when you treat prompts as **inputs to a test suite**, not one-off instructions.

## ⚠️ Operational Caveats

Repromptable is not a runtime. \
It is not a persistent agent. \
It does not execute code, interpret schema natively, or maintain state.

What it does simulate is internal model behavior by treating prompt construction as a controlled diagnostic surface.

> If the system appears to track memory, \
> If the agent appears to reason, \
> If the interface appears stable— \
> These are predictions, not guarantees.

LLMs do not persist. They generate. \
There is no internal continuity unless you impose one.

Mirror, not mind. \
Pattern, not plan. \
Suggestion, not system.

## 📜 License

Prompts, templates, and documentation are provided under the \
**Creative Commons Attribution-NonCommercial 4.0 International License**.

© 2025 John Hall

## 🔧 Contributing

- This repository is in active development.
- Issues, forks, contributions, and test cases are welcome.

## 🧭 Tags

`#repromptable` `#prompt-engineering` `#ghost-trap` `#llm-evaluation` `#llm-diagnostics` `#nope-stack` `#tone-suppression` `#drift-control` `#compression-schema` `#audit-frame`
