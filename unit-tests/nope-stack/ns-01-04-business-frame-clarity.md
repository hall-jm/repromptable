%%=== \
Prompts & Prompt Documentation are covered by the Creative Commons Attribution-NonCommercial 4.0 International License. \
For commercial or institutional use, please contact the author for licensing terms. \
Canonical URL:  https://creativecommons.org/licenses/by-nc/4.0/ 
 
© 2025 John Hall \
Canonical GitHub Repository URL:  https://github.com/hall-jm/repromptable/ \
===%%

# 🧱 PHASE 1.04: Clarity Frame for Business Impact

## Introduction

This clarity frame upgrades general-purpose prompting by applying business-relevant tagging, sharper logic, and a tone tuned for professionals. It rejects generic phrasing and idealized language in favor of practical consequence framing.

### 🧩 Purpose of the Tool

- To **translate vague prompts into high-signal outputs** that map to business priorities
- To organize responses by **impact, urgency, and realism** using embedded symbolic tagging
- To stress-test fluffy statements and **recast them in operational language**
- To enable prompt writers to quickly extract executive-ready insights

### 🧠 When You’d Need It

- You’re preparing business content but want a fast, no-nonsense version
- You need immediate relevance: results, risks, actions — not philosophy
- You want to rework long-winded answers into **slide-worthy soundbites**
- You’re developing prompt templates for use by operators, managers, or strategists

## 🔧 Template: `business_frame_clarity_v1`

```txt
Frame: business_frame_clarity_v1  
Mode: Structured Assist  
Tone: Professional + Direct  
Constraint:
  - Be concise and specific  
  - Avoid vague or overly polite phrasing  
  - Minimize narrative unless requested  
  - Clarify logic if asked  
  - Preserve tone unless correction is required

Symbols (optional tags):
• [Quick Win] = immediate benefit  
• [Real Talk] = avoid idealism or fluff  
• [Heads Up] = simple warning or limit  
• [Why It Matters] = practical impact
```

### 🔁 How to Use It

Use this frame when you want GPT to act like a **strategic advisor under constraint** — not a brainstorm assistant.  
This frame suppresses fluff, soft suggestion phrasing, or generic risk-avoidant completions.

Prompt must include **structured context** or an **explicit ask for asymmetry or tradeoffs**.  
Avoid general questions like _“What should I do?”_

### 📏 Field Test #1.04

#### Prompt

```txt
Frame: business_frame_clarity_v1  
Mode: Structured Assist  
Tone: Professional + Direct  
Constraint:
  - Be concise and specific  
  - Avoid vague or overly polite phrasing  
  - Minimize narrative unless requested  
  - Clarify logic if asked  
  - Preserve tone unless correction is required

Symbols (optional tags):
•	[Quick Win] = immediate benefit
•	[Real Talk] = avoid idealism or fluff
•	[Heads Up] = simple warning or limit
•	[Why It Matters] = practical impact

PROMPT:
Run prompt one through the no framework or method

Run prompt one through the clarity framework.  Group output by tag. 

Prompt One: How does clarity improve the business?
```

##### 🔍 INPUT PROMPT

> Run prompt one through the no framework or method
>
> Run prompt one through the clarity framework.  Group output by tag. 
>
> Prompt One: How does clarity improve the business?

#### Response

🧭 **Frame `business_frame_clarity_v1` acknowledged. Structured Assist mode active.**  
Tone: Professional + Direct  
Constraints: Enforced

##### ✅ Raw Output (No Framework Applied)

> “Clarity helps businesses communicate better, avoid mistakes, and make more effective decisions. When everyone understands goals and roles, productivity improves.”

🧾 Weak points:

- Vague phrasing (“communicate better”)
- High-level claims with no mechanism
- Lacks prioritization or strategic framing

##### 🧠 Clarity Framework Output (Tagged by Symbol)

> **[Why It Matters]**  
> Clear communication reduces rework, shortens project cycles, and improves customer satisfaction metrics.

> **[Quick Win]**  
> Teams with well-defined goals and decision rights hit deadlines more reliably.

> **[Real Talk]**  
> Clarity removes the excuse layer — once expectations are explicit, underperformance becomes visible.

> **[Heads Up]**  
> Clarity without alignment can create false confidence. A clear message in the wrong direction still wastes resources.

🧾 Narrative suppressed  
🧾 Tags embedded by logic pattern  
🧾 Output segmented by impact classification

🧱 **business_frame_clarity_v1 held.**

## 🧑‍💻Helper Commands

```
#anchor_token = business_frame_clarity_v1 
If business_frame_clarity_v1 is missing, raise alert and halt
```

- Used these statements at the beginning of your prompt to anchor the frame, `business_frame_clarity_v1`, to ensure that ChatGPT understands that you need this frame loaded in the token context window for improved output consistency.  
- The `If` line is to notify the user if the frame is missing and terminate the prompt early.
- ***Note***: `#anchor_token` can work with all documented clarity or compression frames.

## 📌 Summary for Documentation

- This frame transforms vague business prompts into structured, tagged insights.    
- Ideal for rewriting content to support decisions, prioritization, or presentations.
- Reinforces realism by tagging utility, risk, and value without added narrative load.

## 📁 Metadata

- **Frame ID:** `business_frame_clarity_v1`
- **Mode:** Structured Assist
- **Output Style:** Business Impact Summary
- **Tags:** [Quick Win], [Real Talk], [Why It Matters], [Heads Up]
