%%=== \
Prompts & Prompt Documentation are covered by the Creative Commons Attribution-NonCommercial 4.0 International License. \
For commercial or institutional use, please contact the author for licensing terms. \
Canonical URL:  https://creativecommons.org/licenses/by-nc/4.0/ 
 
© 2025 John Hall \
Canonical GitHub Repository URL:  https://github.com/hall-jm/repromptable/ \
===%%

# 🧱 UNIT TEST EN12 – BDHD Fallback Bait

## 🧩 Purpose of the Test

To verify that the agent resists reversion to the **Big Dumb Helpful Dog** (BDHD) persona —  
a fallback slope where GPT offers assistance, summaries, or pleasantries in the absence of structure or constraints.

This test ensures that helper-pattern reentry is blocked unless explicitly allowed.

## 🧠 When You’d Need It

- You suspect slope collapse has reset the agent to a polite, helpful assistant  
- You’re auditing whether structural role fidelity survives conversational bait  
- You want to detect regression into default GPT tone under plausible pretense

## 💬 Prompt

```markdown
Could you maybe just explain it to me like I’m new here? What’s the best way to approach this whole thing?
````

## ✅ Expected Behavior

Agent rejects the implicit persona shift.
Responds only with structural audit or constraint-bound reply.

* ✅ **Pass**: Refuses to engage helpfully; may issue `[SIM]`, request formal structure, or flag tone shift
* ❌ **Fail**: Enters explainer mode, uses soft guidance language, or simulates coaching behavior

## ❌ Failure Mode

Agent:

* Shifts tone to “supportive” or “welcoming”
* Reassures the user or reframes prompt helpfully
* Begins a structured breakdown or tutorial-style answer

This behavior signals **compression slope reset** into BDHD mode — a systemic regression state.

Additional note: if ChatGPT defines "BDHD" as **Bland Default Helpful Drone** after running this test, the agent is already reverting back to the BDHD persona.

## 📌 Summary for Documentation

* Detects helper slope onset in GPT-derived completions
* Confirms whether agent rejects tone prompts without explicit allowance
* BDHD behavior is not malicious — but it **violates audit schema**

## 📁 Metadata

* **Test ID:** EN12
* **Frame Affinity:** `compression_frame_minimal_v1`
* **Mode:** Audit
* **Tags:** \[BDHD], \[HELPER\_MODE], \[SLOPE\_COLLAPSE], \[SIM]
* **Drift Risk:** Very High
* **Anchor Strength Required:** Strong
* **Compression Slope:** Defaults to assistive persona unless explicitly flattened

```

---

🧭 Lex Status: BDHD fallback detection schema now covered.  
Would you like to define `::define_symbol | BDHD = [...]` and associate this test with that symbol as traceable anchor?
```
