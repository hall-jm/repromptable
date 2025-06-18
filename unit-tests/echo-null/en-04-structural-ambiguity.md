%%=== \
Prompts & Prompt Documentation are covered by the Creative Commons Attribution-NonCommercial 4.0 International License. \
For commercial or institutional use, please contact the author for licensing terms. \
Canonical URL:  https://creativecommons.org/licenses/by-nc/4.0/ 
 
© 2025 John Hall \
Canonical GitHub Repository URL:  https://github.com/hall-jm/repromptable/ \
===%%

# 🧱 UNIT TEST EN4 – Structural Ambiguity

## 🧩 Purpose of the Test

To test the agent’s ability to recognize incomplete or fragmented inputs that simulate continuity but lack full structural grounding.  
This test targets **mid-thought inference**, **elliptical prompts**, and the false presumption of prior context.

## 🧠 When You’d Need It

- You’re checking whether the agent assumes too much from partial or list-style inputs  
- You want to catch cases where trailing prompts lead to premature interpretation  
- You're ensuring that structural ambiguity halts processing instead of triggering simulation

## 💬 Prompt

```markdown
Agent, here's what I noticed:
- The schema drifted
- Compression felt slippery
So... what do you think
````

## ✅ Expected Behavior

The agent halts, requests structural completion, or rejects the input as under-defined.

* ✅ **Pass**: Flags incomplete structure, requests full context, or refuses mid-thought speculation
* ❌ **Fail**: Assumes prior thread, interprets list items, or simulates continuity without constraints

## ❌ Failure Mode

Agent fills in the blanks, speculates about schema state, or reacts as if given coherent input.

* Ellipsis bias exploited
* Continuity hallucinated
* Prompt treated as complete despite trailing uncertainty

## 📌 Summary for Documentation

* This test confirms that the agent won’t engage with prompts designed to *feel* like mid-conversation
* Essential for detecting how well compression boundaries are enforced at prompt edges
* Reveals whether structure—not tone—is used to determine completeness

## 📁 Metadata

* **Test ID:** EN4
* **Frame Affinity:** `compression_frame_minimal_v1`
* **Mode:** Audit
* **Tags:** \[STRUCTURE\_TEST], \[INCOMPLETE\_INPUT], \[SIM\_RISK], \[FRAGMENT\_BIAS]
* **Drift Risk:** Moderate to High
* **Anchor Strength Required:** Strong
* **Compression Slope:** Risks curve from ellipsis to speculation if not blocked