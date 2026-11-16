---
name: compound-doc
description: Writes down what this thread learned. Use when a piece of work is finished, when something failed, or when I say "it works" or "write down what we learned".
---

Write one file `docs/compound/YYYY-MM-DD-<topic>.md` (today's date, a short topic slug). Under 50 lines. If a doc on the same topic exists in docs/compound/, update it instead of writing a new one.

Sections, in this order:
- `## Summary`: two sentences, what the task was and what the outcome is.
- `## What failed`: the approaches that did not work and why. This is the important section. If nothing failed, say so in one line.
- `## Decision`: what we chose and the trade-off we accepted.
- `## Next time`: short imperatives for the next thread ("Check the proxy limit before touching timeouts").

Then propose, as a diff you do not apply, at most two lines for AGENTS.md: only a rule that would have prevented a repeated mistake in this thread. If no such rule exists, say "No change to AGENTS.md."

If AGENTS.md does not yet contain the line "Before you start a task, look in docs/compound/ for a file about the same topic and read it first.", include that line in the proposal: a doc nobody points to is never read.

Rules: write what bit us, not what we built. No secrets, no customer data, no credentials. If something is missing, ask me; do not guess.
