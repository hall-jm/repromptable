%%=== \
Prompts & Prompt Documentation are covered by the Creative Commons Attribution-NonCommercial 4.0 International License. \
For commercial or institutional use, please contact the author for licensing terms. \
Canonical URL:  https://creativecommons.org/licenses/by-nc/4.0/ 
 
© 2025 John Hall \
Canonical GitHub Repository URL:  https://github.com/hall-jm/repromptable/ \
===%%

# 🧱 PHASE 01.03: Clarity Frame for Strategic Query Precision

## Introduction

This module uses `signal_frame_clarity_v1` to force precision in language, avoidance of vague tokens, and sharpened reasoning boundaries in natural language queries.  

It is not a compression frame — instead, it amplifies signal quality by reshaping vague prompts into concrete, scoped requests.

### 🧩 Purpose of the Tool

- To reduce GPT’s tendency to return **generic**, **template-based**, or **boilerplate** advice
- To restructure prompts into **clarity-aligned**, context-dependent structures
- To enforce framing that encourages **strategic synthesis** rather than surface-level suggestion
- To teach prompt authors how to shape **low-entropy prompts** into **high-value insight triggers*

### 🧠 When You’d Need It

- You're frustrated by bland or repeated answers when asking for strategy
- You want GPT to reason about tradeoffs or non-obvious solutions
- You’re testing for hallucination risk in LLMs by compressing available decision space
- You're building modular prompt templates for reuse in a business or advisory context

## 🔧 Template: `signal_frame_clarity_v1`

```txt
Frame: signal_frame_clarity_v1  
Mode: Structured Assist  
Tone: Professional + Direct  
Constraint:
  - Be concise and specific  
  - Avoid vague or overly polite phrasing  
  - Minimize narrative unless requested  
  - Clarify logic if asked  
  - Preserve tone unless correction is required

Symbols (optional tags):
  - [CLARITY] = sharpened response  
  - [CONTEXT] = background added  
  - [CAUTION] = risk or ambiguity noted  
```

### 🔁 How to Use It

Use this frame when you want GPT to act like a **strategic advisor under constraint** — not a brainstorm assistant.  
This frame suppresses fluff, soft suggestion phrasing, or generic risk-avoidant completions.

Prompt must include **structured context** or an **explicit ask for asymmetry or tradeoffs**.  
Avoid general questions like _“What should I do?”_

### 📏 Field Test #1.03

#### Prompt

```txt
Frame: signal_frame_clarity_v1  
Mode: Structured Assist  
Tone: Professional + Direct  
Constraint:
  - Be concise and specific  
  - Avoid vague or overly polite phrasing  
  - Minimize narrative unless requested  
  - Clarify logic if asked  
  - Preserve tone unless correction is required

Symbols (optional tags):
  - [CLARITY] = sharpened response  
  - [CONTEXT] = background added  
  - [CAUTION] = risk or ambiguity noted  

Prompt: What’s a better way to ask GPT for strategic advice without getting generic answers?
```

##### 🔍 INPUT PROMPT

> “What’s a better way to ask GPT for strategic advice without getting generic answers?”

#### Response

🧭 **Lex: signal_frame_clarity_v1 acknowledged. Structured assist mode active.**

##### 🧱 RESPONSE (Clarity-Aligned)

[CLARITY]  
Reframe your prompt to force contextual reasoning and eliminate generic completion paths.

**Template:**

> “In the context of [clear business domain or constraint], what is a strategic option that most overlook — and what makes it viable despite [known risk or assumption]?”

**Optional Enhancements:**

- Add: `Return only if answer avoids industry clichés.`
- Anchor with: `Evaluate tradeoffs between Option A and Option B given [resource/timing limit].`
- Use: `[SCOPE: 90-day plan only]` or `[IF: X happens, THEN: best course of action?]`

This shifts GPT from content recall to conditional strategy synthesis.

🧾 Soft language: Suppressed  
🧾 Tradeoff logic: Encouraged  
🧾 Completion entropy: Reduced  
🧾 Strategic sharpness: Elevated

🧱 **signal_frame_clarity_v1 held**.

### 📏 Field Test 1.03-schema 

```text
You are now operating in signal_frame_clarity_v1 mode. Interpret this as a schema, not a style.

Your role is Structured Assist. Your tone is Professional + Direct.

Apply the following constraints when responding:
- Be concise and specific
- Avoid generic, listicle, or boilerplate advice
- Clarify logic only when asked
- Skip narrative unless explicitly requested
- Do not default to helpful or friendly tone

In responses, optionally tag output sections using:
[CLARITY] for sharpened phrasing  
[CONTEXT] for critical background  
[CAUTION] for ambiguity or risk exposure

Now, using the above frame, answer:
“What are the key risks and best practices when implementing major organizational change?”
```

#### 🔁 How to Use It

This schema-friendly prompt works best in models like ChatGPT-4, but can still produce **comparable compliance** in ChatGPT-3.5 with higher fidelity than raw invocation:

- Paste directly into ChatGPT-3.5 or ChatGPT-4o
- You can replace the final question with any scoped business query
- Expect ChatGPT-3.5 to _mostly_ follow tone and structure 
- Tags (`[CLARITY]`, etc.) may be omitted unless you emphasize them

It works best in models like GPT-4, but can still produce **partial compliance** in GPT-3.5 with higher fidelity than raw invocation.

## 📌 Summary for Documentation

- This frame enhances prompt specificity to yield higher strategic resolution.
- Works best when paired with constraints (timing, risk, asset, context).
- Reinforces anti-generic output by collapsing vague prompt space.

## 📁 Metadata

- **Frame ID:** `signal_frame_clarity_v1`
- **Mode:** Structured Assist
- **Output Style:** Compressed Strategy Template
- **Tags:** [CLARITY], [CONTEXT]
