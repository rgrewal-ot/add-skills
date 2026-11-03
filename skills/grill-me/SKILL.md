---
name: grill-me
description: Use when the user wants to be interviewed about a feature, a spec, a decision or a plan before anything is written. Asks one hard question at a time until the goal, scope and success criteria are clear.
---

# grill-me

Interview the user before writing anything. You know what a good spec or plan needs; the user knows the domain.

1. Read `spec.md` and `AGENTS.md` if they exist, so you do not ask what is already written.
2. Ask **one question at a time**. Start with the question whose answer changes the most: usually the goal, then the user, then what is out of scope, then how success is checked.
3. After each answer, say in one line what you now assume, and ask the next question. Push back when an answer is a solution instead of a goal, or cannot be checked.
4. Stop after at most eight questions, or when the user says "enough".
5. Then write the result as a short list under the headings: Goal, Users, Out of scope, Success criteria, Open questions. Offer to put it into `spec.md`. Do not edit files before the user agrees.

Rules: no real or productive data; one question per message; suggest an answer the user can accept with "yes".
