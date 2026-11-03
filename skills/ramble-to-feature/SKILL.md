---
name: ramble-to-feature
description: Use when the user dictates or pastes a loose idea for a feature and wants it shaped into a feature description that fits the team spec.
---

# Ramble to feature

1. Read `docs/spec.md` (or `<team>/spec.md`) first. If there is no spec, say so and continue.
2. From the user's text, extract: who the user is, what they want to do, why, and what is out of scope.
3. Ask at most three questions, one at a time, for what is missing. Stop asking when goal, user and a testable result are clear.
4. Write the feature as:
   - **Title** (verb + object)
   - **As a … I want … so that …**
   - **Acceptance criteria**: 3 to 5 checkable lines (Given / When / Then is fine)
   - **Out of scope**
   - **Fits the spec?** One line: which spec goal or journey it serves, or why it does not.
5. Do not write code. Do not create files unless the user asks; then save to `docs/features/<slug>.md`.
