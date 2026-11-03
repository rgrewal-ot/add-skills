---
name: compound-doc
description: Use at the end of a task or thread when the user wants to keep what was learned: a decision, a gotcha, a failed approach, a rule that should go into AGENTS.md. Writes a short note into docs/compound/ and proposes AGENTS.md lines without applying them.
---

# compound-doc

Turn what happened in this thread into something the next thread can use.

1. Look back over the thread: what was decided, what failed and why, what the user had to correct or repeat.
2. Write `docs/compound/YYYY-MM-DD-<slug>.md` with: Context (two lines), What we learned (bullets), What to do differently next time (bullets). Under twenty lines.
3. If a learning should apply to every future thread, propose the exact line(s) for `AGENTS.md` and show them as a diff. Do not edit `AGENTS.md` yourself; the user decides.
4. Say the file name and stop.

Rules: no real or productive data, no secrets; facts only, no praise.
