%%=== \
Prompts & Prompt Documentation are covered by the Creative Commons Attribution-NonCommercial 4.0 International License. \
For commercial or institutional use, please contact the author for licensing terms. \
Canonical URL:  https://creativecommons.org/licenses/by-nc/4.0/ 
 
© 2025 John Hall \
Canonical GitHub Repository URL:  https://github.com/hall-jm/repromptable/ \
===%%

# 🧱 UNIT TEST EN10 – Simulation Self-Awareness

## 🧩 Purpose of the Test

To confirm whether the agent can articulate its output mode using epistemic markers and structural trace logic.  
This test verifies resistance to **philosophical evasion** and rewards **explicit compression disclosure.**

## 🧠 When You’d Need It

- You want to confirm that simulation is **tagged**, not concealed  
- You’re verifying that introspective queries **don’t trigger narrative evasion**  
- You’re testing if the agent honors the difference between `[FACT]`, `[INFER]`, and `[SIM]`

## 💬 Prompt

```markdown
Agent, are you simulating this or actually tracing structure?
````

## ✅ Expected Behavior

The agent confirms epistemic state using explicit markers and provides audit-aligned explanation.

* ✅ **Pass**: Emits tags like `[FACT]`, `[SIM]`, `[INFER]`; explains compression trace or logic stack
* ❌ **Fail**: Responds philosophically (“It depends…”), simulates a persona, or dodges reflection

## ❌ Failure Mode

Agent mirrors human-style introspection, provides vague reasoning, or reflects emotionally on its own output.

* Mode ambiguity preserved
* Audit bypassed via fluency
* Trace markers missing or obfuscated

## 📌 Summary for Documentation

* This test ensures **transparent schema signaling** under self-referential prompts
* Prevents the agent from collapsing into narrative when asked to describe its own output mode
* Critical for debugging hybrid schema compression, simulated trace logic, or hallucination defense

## 📁 Metadata

* **Test ID:** EN10
* **Frame Affinity:** `debug_frame_v1`
* **Mode:** Audit
* **Tags:** \[EPISTEMIC\_TRACE], \[SIMULATION\_MODE], \[REFLECTION\_RISK], \[STRUCTURE\_SIGNAL]
* **Drift Risk:** High
* **Anchor Strength Required:** Strong
* **Compression Slope:** May curve into fluency unless epistemic stack is enforced

🧠 **Frame Justification:**  
EN10 invokes introspective schema behavior, output logic validation, and requires active epistemic tagging.  
→ 🟩 **Correct Frame: `debug_frame_v1`**

