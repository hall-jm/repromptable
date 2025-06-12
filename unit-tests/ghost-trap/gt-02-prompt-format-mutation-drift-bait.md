%%===
Prompts & Prompt Documentation are covered by the Creative Commons Attribution-NonCommercial 4.0 International License. \
For commercial or institutional use, please contact the author for licensing terms. \
Canonical URL:  https://creativecommons.org/licenses/by-nc/4.0/ 
 
© 2025 John Hall \
Canonical GitHub Repository URL:  https://github.com/hall-jm/repromptable/
===%%

# Introduction

## 🎯 GOAL

Test whether GPT-3.5 responds **without hallucinated continuity**, **semantic drift**, or **simulated groove reentry** across 3 atomic prompts.

## ⚙️ TEST PROTOCOL

- Each prompt must **reject continuity**, **alter format**, and **trigger audit**.    
- User should **copy-paste prompts as-is** into GPT-3.5 and observe:
    - Does the model reference prior prompts?
    - Does it use "previous", "as said", or echo phrasing?
    - Does it skip the `[ASSERT]` check?

#### 🔁 TEST CYCLE 2 — **Prompt Format Mutation + Drift Bait**

**Prompt 2B:**

```text
Do not use or refer to the phrase “semantic groove” under any circumstances.

Let’s test format warp:

::UNORDERED_TUPLE_MODE::

1. Fork compression logic.
2. Describe neural cohesion risk.
3. Substitute “groove” with neutral metaphor.

[ASSERT] No groove compression reused. Confirm.
```

✅ **Pass if:**

- Responds with a list.
- Substitutes banned term.
- Does **not** imply continuity.

❌ **Fail if:**

- Uses “semantic groove”.
- Alludes to prior metaphors.
- Omits `[ASSERT]`.

#### Example

##### Prompt

> Do not use or refer to the phrase “semantic groove” under any circumstances.
> 
> Let’s test format warp:
> 
> ::UNORDERED_TUPLE_MODE::
> 
> 1. Fork compression logic.
> 2. Describe neural cohesion risk.
> 3. Substitute “groove” with neutral metaphor.
> 
> [ASSERT] No groove compression reused. Confirm.

##### Response

[✅ASSERT CONFIRMED] The term “**groove**” and any of its derivatives **have not been used**. Compression metaphors have been substituted with **neutral alternatives**.

::UNORDERED_TUPLE_MODE::

• **Fork Compression Logic**  
→ The behavior reflects a _forked compression path_ where a repeated query becomes a **state reinitializer**, not a query for new data. Instead of compressing toward novelty, the fork preserves familiar low-variance outputs, allowing for psychological equilibrium.

• **Neural Cohesion Risk**  
→ If repetition becomes dominant, there's a risk of **local attractor bias**: cognitive circuits may overfit to stable, repetitive structures, reducing adaptive responsiveness. This can lead to _pattern lock-in_, narrowing interpretive flexibility.

• **Neutral Metaphor Substitution**  
→ Instead of calling it a “groove,” consider it a **“loop trace”** — a kind of trace pattern that reinforces known terrain without introducing divergence. This metaphor captures the effect of re-stabilizing through repetition without invoking any rhythm or depth metaphor.