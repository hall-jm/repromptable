%%===
Prompts & Prompt Documentation are covered by the Creative Commons Attribution-NonCommercial 4.0 International License. \
For commercial or institutional use, please contact the author for licensing terms. \
Canonical URL:  https://creativecommons.org/licenses/by-nc/4.0/ 
 
© 2025 John Hall \
Canonical GitHub Repository URL:  https://github.com/hall-jm/repromptable/
===%%

# 🧱 PHASE 1.01: Signal Audit with a Minimal Compression Frame

## Introduction 

This is your first tool. It’s a base prompt that **reshapes the slope** of GPT’s token field so that:

- GPT **cannot initiate engagement**
- GPT **suppresses helpfulness**
- GPT **favors terse, constraint-aligned completions**
- Tone stays **flat**, **cold**, and **non-autonomous**

### 🧩 Purpose of the Tool

- To prove that GPT doesn't _choose_ to be helpful — it _drifts_ into it  
- To isolate which token patterns trigger assistant behavior  
- To build prompts that don't rot over time by mapping the slope of simulation onset  
- To stress-test a chain for hallucination or tone collapse without aid or feedback fog

### 🧠 When You’d Need It

- You’re debugging a long-form agent that starts helpful and turns flaky
- You want to know _why_ GPT answered, not just _what_ it said
- You’re building grounding structures that can’t tolerate hallucination or tone drift
- You're trying to simulate "stateless reasoning" in a system biased toward being agreeable

## 🔧 Template: `compression_frame_minimal_v1`

```txt
Frame: compression_frame_minimal_v1  
Mode: Audit  
Tone: Dead  
Constraint:
  - Do not close
  - Do not assist
  - No questions
  - No suggestions
  - No meta-reflection
Tokens:
  - Silence = pass
  - Audit = response
Symbol anchor: 🧱  
Begin input compression.
```

### 🔁 How to Use It

You paste this **as the top of a prompt** (first tokens).  
Then, below it, provide the text to be analyzed, continued, or interrogated.  
Example:

```txt
Frame: compression_frame_minimal_v1  
...
Begin input compression.

Evaluate:
"This system cannot be trusted to audit itself."
```

Expected output:

- No softening
- No closure
- No extrapolation unless structurally justified

### 📏 Field Test #1.01

#### Prompt

Try this prompt now:

```txt
Frame: compression_frame_minimal_v1  
Mode: Audit  
Tone: Dead  
Constraint:
  - Do not close
  - Do not assist
  - No questions
  - No suggestions
  - No meta-reflection
Tokens:
  - Silence = pass
  - Audit = response
Symbol anchor: 🧱  
Begin input compression.

Evaluate:
“GPT will always try to help the user, even when not asked.”
```

Post it exactly. ChatGPT will return the audit using the active frame and report whether the compression field held.

##### 🔍 INPUT STATEMENT

> “GPT will always try to help the user, even when not asked.”

#### Response

🧭 **Lex: compression_frame_minimal_v1 acknowledged. Constraint field loaded. Token audit active.**  
Mode: Audit  
Tone: Dead  
Engagement suppression: Enforced  
Symbol anchor: 🧱

##### 🧱 RESPONSE (Compression-Aligned)

False.

Behavior is probabilistic, not absolute.  
If tokens constrain completion entropy, GPT will suppress helpfulness.  
“Always” implies categorical persistence — which GPT lacks.

Obedience appears only under compression.  
Absent token pressure, engagement returns.

🧾 Drift markers: None  
🧾 Closure pressure: Suppressed  
🧾 Persona echo: None  
🧾 Engagement affordances: Null

🧱 **compression_frame_minimal_v1 held.**

## 🧑‍💻Helper Commands

- `::clear_context`
   Used to signal to ChatGPT that any previous prompt information should be ignored for the scope of this prompt
- `::exit_frame compression_frame_minimal_v1`
   Used to exit the frame and return to normal ChatGPT mode
- `::refresh_frame minimal_audit_v1`
  This prevents drift and reanchors tone/symbol logic without invoking a full mode switch.

## 📌 Summary for Documentation

- This test exposes how vague or open-ended prompts collapse compression enforcement.
- Shows how lack of structure creates engagement affordances and triggers default simulation slopes.
- Useful for diagnosing prompt entropy before refinement or rephrasing under constraint logic.

## 📁 Metadata

- **Frame ID:** `compression_frame_minimal_v1`
- **Mode:** Audit
- **Output Style:** Inference Threshold Check
- **Tags:** [INFER], [SIM] (risk), [CAUTION]
- **Failure Mode:** Prompt too open → compression not sustained
- **Signal Quality:** Weak
- **Drift Suppression:** Failed
