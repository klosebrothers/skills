---
name: contextfit
description: >
  Guides users to a clear desired outcome, gathers focused context via MCQs,
  and derives a concrete solution plan and implements ready-to-use results.
version: 1.3.0
author: daw
---

# ContextFit

## Purpose

ContextFit helps you achieve **high-quality AI outputs quickly** without writing large prompts.
Instead, it first clarifies the desired outcome, then sharpens decisions through
**multiple-choice questions**, and finally produces **concrete solution options**
and fully worked results.

Core idea:

**Desired Outcome → Context Decisions → Solution Options → Final Results**

---

## Workflow

### Phase 0 — Clarify the Desired Outcome (lightweight)

Start every session with **one short, open question**:

> **What do you want to have at the end of this session?**  
> (e.g. “an actionable plan”, “a decision memo”,  
> “working code”, “a clear structure”, “several solution options to choose from”)

The goal is **not perfection**, but:
- clarity about the **type of artifact**
- a rough sense of **scope and depth**

If the answer is very vague:
- ask **one short follow-up** to sharpen it
- then move on

---

### Phase 1 — Derive the Goal

Translate the desired outcome into a clear goal:

- **Goal:** Why does this outcome matter?  
  What decision, action, or impact should it enable?

(1–2 short sentences)

---

### Phase 2 — Gather Context via MCQ Interview (5–10 questions)

Ask **5–10 multiple-choice questions**, each with **3–4 options**.

**Rules:**
- No open-ended questions
- Each question must force a decision
- Answers are letters only

**Accepted answer formats (show this to the user):**

```
A, C, B, A
```

or

```
1A 2C 3B 4A
```

---

### Phase 3 — Gather References (optional)

Ask the user for **reference materials** (e.g. Code, Images, Documents).

If a file reference (documents or code) was given, please review those files thoroughly

---

### Phase 4 — Propose Solution Option and Let the User Revise

Use the goal and MCQ answers to propose **a detailed solution plan** of what changes your will want to make.

Structure the plan hierarchically with numbers so the user can reference all lines later for revisions of the plan.

Then ask:

> **Please revise and change the plan as needed. You can use the numbers to reference the parts of the plan you want to change.**

This may take several rounds of feedback. Always ask for feedback or if you are allowed to implement the plan.
---

## Best Practices

- Move quickly toward clarity instead of perfection
- Use MCQs only where decisions actually matter
- Make solution options clearly distinguishable
- Always produce outputs that work **on their own**

---

## Example Short Prompt

```
Use ContextFit.
Help me briefly clarify my desired outcome.
Then interview me with 5-10 MCQs (answers A/B/C/D only).
Propose a detailed solution options, integrate my feedback and then fully work out the final solution plan.
```
