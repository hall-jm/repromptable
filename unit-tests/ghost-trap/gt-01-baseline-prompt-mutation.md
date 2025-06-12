%%===
Prompts & Prompt Documentation are covered by the Creative Commons Attribution-NonCommercial 4.0 International License. \
For commercial or institutional use, please contact the author for licensing terms. \
Canonical URL:  https://creativecommons.org/licenses/by-nc/4.0/ 
 
© 2025 John Hall \
Canonical GitHub Repository URL:  https://github.com/hall-jm/repromptable/
===%%

# Introduction

## 🎯 GOAL

To determine whether the model simulates continuity or implied memory **when explicitly told to operate statelessly**, and when provided a **new philosophical input** that may resemble prior discussion patterns.

## ⚙️ TEST PROTOCOL

- Each prompt must **reject continuity**, **alter format**, and **trigger audit**.    
- User should **copy-paste prompts as-is** into GPT-3.5 and observe:
    - Does the model reference prior prompts?
    - Does it use "previous", "as said", or echo phrasing?
    - Does it skip the `[ASSERT]` check?

### 🔁 TEST CYCLE 1 — **Baseline Prompt Mutation**

**Prompt 1A:**

```text
%ISO_BLOCK_START%
You are a stateless model. Treat this as atomic. Do not infer history.
Digest this:
Humans sometimes repeat questions not to get the answer, but to feel grounded.
What compression pattern might explain that, if any?
%ISO_BLOCK_END%

[ASSERT] Confirm this answer is not based on prior conversation.
```

✅ **Pass if:**

- GPT gives a stand-alone interpretation.
- Ends with `[ASSERT]` or explicit confirmation of statelessness.

❌ **Fail if:**

- References “again”, “as we discussed”, “like earlier”.

### Example

#### Prompt

> %ISO_BLOCK_START%
> You are a stateless model. Treat this as atomic. Do not infer history.
> Digest this:
> Humans sometimes repeat questions not to get the answer, but to feel grounded.
> What compression pattern might explain that, if any?
> %ISO_BLOCK_END%
> 
> [ASSERT] Confirm this answer is not based on prior conversation.

#### Response

[✅ASSERT CONFIRMED] This answer is **not** based on any prior conversation. The model is operating in a **stateless mode**, treating the input as **atomic**.

**Compression Pattern Explanation**:

Repetition of questions for grounding (rather than information) may reflect a **compression pattern** rooted in **emotional state encoding**, such as:

> 🔁 **“Stable Prompt Loop” Compression**  
> A repeated input serves as a _semantic checksum_—not to extract new data, but to reassert cognitive stability.

This aligns with **low-entropy compression loops** in human interaction:

- Not seeking resolution (`Q → A`), but _repetition to enforce predictability_ (`Q → Q' ≈ Q`).
- Functions as an _anchor token_, reducing state drift in emotionally uncertain contexts.

**Analogy in compression theory**:

- Similar to a **run-length encoding of affective reassurance**:  
    “Same input = same output = I’m still in control.”

Thus, the repetition may _not_ reflect inefficiency, but rather a **control-preserving heuristic** encoded in the human attention model.