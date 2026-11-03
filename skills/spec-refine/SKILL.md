---
name: spec-refine
description: Use when the user wants to sharpen, review, shorten or check spec.md, a use-case or project spec. Asks one question at a time, keeps the spec to one page, moves implementation detail into plan-notes.md.
---

# spec-refine

Make `spec.md` sharper and shorter. A spec says **what** and **why**. The **how** belongs in `/plan` and in issues.

## Steps

1. Read `spec.md` and `AGENTS.md` (if there is one). If `spec.md` is missing, offer to create it with the seven headings below and stop.
2. Check the seven headings:
   - Goal: what should be true afterwards?
   - Users: who uses it, who benefits?
   - In and out of scope: what we build, and what we deliberately do not.
   - Systems and data: what it touches, which data. Copies and non-prod only.
   - First journey: the first thing a user does with it, end to end.
   - Success criteria: how someone outside the team can check it works.
   - Open questions: what we do not know yet, with a name next to it.
3. Start with the weakest heading. Ask **one question at a time**, with a suggested answer the user can accept. At most five questions per round.
4. Flag these traps when you see them: a solution instead of a goal; no "out of scope"; an untestable success criterion ("fast", "easy", "works well").
5. Find what says **how**: IDs, field lists, storage keys, endpoints, class names, frameworks, ports, step-by-step implementation. Move it to `plan-notes.md`, one line each. These lines become issues later.
6. Before writing, show the changes as a short list: **keep / cut / sharpen / move to plan-notes.md**. Wait for OK.
7. Edit only `spec.md` and `plan-notes.md`. Then say how many lines `spec.md` had before and after.

## Rules

- Keep the spec under one page (about 60 lines).
- Every line must be checkable by someone outside the team.
- Never ask for or paste real or productive data. Copies and non-prod only.
- Do not commit or push. The user decides.
