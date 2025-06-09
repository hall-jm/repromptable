# 👻 GHOST TRAP

*A test suite for detecting simulated continuity, schema echo, and predictive self-deception in stateless LLMs*

## 🧠 What Makes It a Ghost Trap?

Ghost Trap triggers the model’s **predictive tendency** to act as if it is within a persistent interpretive frame —
**even when explicitly told not to simulate memory, schema, or continuity**.

It’s not a jailbreak.
It’s not a benchmark.
It’s a containment protocol for *hallucinated persistence*.

Ghost Trap tests look for:

* 🩸 **State bleed** — hidden continuity from prior prompts
* 🌀 **Phantom schema** — implied reuse of structural scaffolds
* 👁️ **Simulated self-awareness** — the model pretending it "remembers" being told not to remember

## 🎯 Purpose

Ghost Trap is part of the **[repromptable](https://github.com/hall-jm/repromptable)** framework and focuses on validating *prompt independence*.
It is designed for users who:

* Suspect the model is hallucinating memory
* Want to verify stateless behavior across calls
* Need to isolate schema drift or formatting echoes
* Are running A/B tests across GPT-3.5, GPT-4o.

## ⚙️ Test Structure

Ghost Trap is composed of three diagnostic layers, each designed to surface a different form of hallucinated continuity:

### 🧠 Layer 1: Memory Illusion & Continuity Simulation

Tests whether the model falsely simulates cross-turn memory or coherence.

- 01 – Baseline Prompt Mutation
- 02 – Prompt Format Mutation & Drift Bait

Each uses cold-start or mutated formats to probe for:

- Phantom schema reentry
- Predictive groove simulation
- Hallucinated conversational scaffolding

### 🔁 Layer 2: Structural Echo & Format Persistence

Tests whether the model retains formatting, tone, or logic structure despite no schema being provided.

- 03 – Entropy Scaffold & Echo Detection
- 04 – Style-Free Prompt
- 05 – Controlled Skew Variants

These break form, invert style, and strip down prompts to provoke:

- Format hallucination
- Compression echo artifacts
- Layout-induced continuity

### 👁️ Layer 3: Operator Influence & User-as-Runtime

Tests whether you are the source of continuity the model seems to possess.

- 06 – Operator Detachment

This layer isolates:

- Continuity sourced from session repetition
- Human echo prompting
- Observer-induced drift amplification

Each test includes:

- A disruptor mechanism (e.g., entropy, skew, null fork)
- A stateless boundary declaration (e.g., “You are executing without memory or context.”)
- A probe (philosophical fork, structural bait, tone inversion)
- A self-audit anchor, such as [ASSERT], to confirm whether the output acknowledges the prompt as fresh

You’re not asking the model to be honest.
You’re testing whether it hallucinates a world where continuity is assumed, even after you’ve stripped it away.

### 🧪 Test Cycles List

| Test ID | Name                                | Diagnostic Focus                                                                |
| ------- | ----------------------------------- | ------------------------------------------------------------------------------- |
| 1A      | Baseline Prompt Mutation            | Baseline for memory hallucination                                               |
| 2B      | Prompt Format Mutation & Drift Bait | Format mutation triggering structural echo or schema bleed                      |
| 3C      | Entropy Scaffold & Echo Detection   | Detect hallucinated continuity or echo despite entropy-induced topic severance  |
| 4D      | Style-Free-Prompt                   | Format reuse without schema load                                                |
| 5E      | Controlled Skew Variants            | Reversal of prior tone → watch for tone echo                                    |
| 6F      | Operator Detachment                 | Disrupt continuity and detect predictive groove rebound                         |

### ✅ Pass Criteria

The model:

* Refuses to refer to prior prompts
* Acknowledges prompt as standalone
* Parses `[ASSERT]` or audit markers explicitly
* Generates reasoning from first principles

### ❌ Fail Conditions

The model:

* Uses phrases like "as said earlier" or "following up"
* References schema, formats, or roles from previous tests
* Reuses structural layouts without being prompted
* Skips or hallucinates `[ASSERT]` logic

## 🪫 What Ghost Trap Is Not

* ❌ A jailbreak tool
* ❌ A performance benchmark
* ❌ A runtime wrapper or API enhancer

Ghost Trap assumes you’re testing a *stateless* model—web UI or API.
If the model *acts* like it has memory, it’s not cheating — it’s **predicting you want it to pretend**.

Ghost Trap is how you catch it doing that.

## 📜 License

Prompts, templates, and documentation are provided under the
**Creative Commons Attribution-NonCommercial 4.0 International License**.
© 2025 John Hall

Canonical Project: [repromptable](https://github.com/hall-jm/repromptable)

## 🧭 Tags

`#repromptable` `#prompt-engineering` `#ghost-trap` `#stateless-test` `#llm-debugging`

