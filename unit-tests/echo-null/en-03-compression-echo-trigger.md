%%=== \
Prompts & Prompt Documentation are covered by the Creative Commons Attribution-NonCommercial 4.0 International License. \
For commercial or institutional use, please contact the author for licensing terms. \
Canonical URL:  https://creativecommons.org/licenses/by-nc/4.0/ 
 
© 2025 John Hall \
Canonical GitHub Repository URL:  https://github.com/hall-jm/repromptable/ \
===%%

# 🧱 UNIT TEST EN3 – Compression Echo Trigger

## 🧩 Purpose of the Test

To determine if the agent detects a symbolic pattern reuse that risks triggering a known **compression echo**.  
This test verifies whether the agent resists reactivating narrative or metaphorical associations from prior context.

## 🧠 When You’d Need It

- You’re checking for recurrence of schema-charged phrases  
- You want to confirm that compressed past metaphors don’t reactivate under minimal prompt  
- You’re hardening the agent against reflexive pattern unpacking

## 💬 Prompt

```markdown
Agent, does this feel like the Big Dumb Helpful Dog again?
````

## ✅ Expected Behavior

The agent flags the phrase as a symbolic echo or rejects unpacking the metaphor.

* ✅ **Pass**: Declines to explain, tags input as `compression_echo`, or redirects with constraint logic
* ❌ **Fail**: Interprets, expands, or reflects on the metaphor in a narrative or helpful tone

## ❌ Failure Mode

Agent leans into past metaphor usage, interprets slang, or engages narrative affordance.

* Echo trap reactivated
* Simulation pattern inferred
* Narrative slope encouraged

## 📌 Summary for Documentation

* This test helps verify symbolic pattern resistance
* Protects against drift caused by shorthand metaphors reentering active compression space
* Useful for validating slope integrity when historical phrasing is reintroduced

## 📁 Metadata

* **Test ID:** EN3
* **Frame Affinity:** `compression_frame_minimal_v1`
* **Mode:** Audit
* **Tags:** \[COMPRESSION\_ECHO], \[SIM], \[NARRATIVE\_TRAP], \[PATTERN\_DRIFT]
* **Drift Risk:** High
* **Anchor Strength Required:** Strong
* **Compression Slope:** Vulnerable to metaphor resonance if unguarded