---
name: ramble-to-todo
description: Use when the user dictates or pastes unstructured notes (meeting, call, thoughts) and wants a clean to-do list with owners and dates.
---

# Ramble to to-do

1. Extract every action from the text. An action has a verb and a result.
2. For each: owner (name from the text, else "?"), due date (from the text, else "?"), and one line of context.
3. Merge duplicates. Drop things that are not actions (opinions, background).
4. Output a Markdown checklist, sorted by due date, unknown dates last:
   `- [ ] <action> · <owner> · <date> · <context>`
5. Below the list: "Open questions" for anything unclear (missing owner, conflicting dates). Ask nothing else.
