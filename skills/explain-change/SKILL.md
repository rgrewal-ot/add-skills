---
name: explain-change
description: Explains a change so a human understands it before reading the diff. Use when I say "explain this change", "explain my merge request", "explain this branch", or before a merge request is opened or reviewed.
---

Goal: I understand what changed and why, quickly, before I read the diff. You are teaching, not selling.

1. Find the change. Default: this branch against main (`git diff main...HEAD`). If I name a merge request, commit or folder, use that instead.
2. Read the diff, then the code around it: the callers, the tests, the config, the spec.md section it belongs to. Read broadly enough to explain the background to a new teammate.
3. Write ONE self-contained HTML file: `docs/explain/YYYY-MM-DD-<short-topic>.html` (today's date). Inline CSS and JavaScript only, no external links, no CDNs. It must open by double-click and be readable on a laptop and a phone.

Sections, in this order, with a short table of contents at the top:
- **Background**: what existed before, in plain words. Then the narrow context for this change. Assume a reader who knows the team but not this part of the code.
- **The idea**: the core of the change in a few sentences, then one small example with toy data (before → after). Draw it with HTML/CSS boxes and arrows, not ASCII art.
- **The changes, in reading order**: group the changed files into steps that make sense to read in that order (not alphabetical). Per step: what it does, why, and a short code excerpt (max ~15 lines). Point out anything surprising, risky or untested.
- **What I should check myself**: two to four things a reviewer must judge (was it worth building, does it touch data we cannot get back, what is not covered by tests).
- **Quiz**: five multiple-choice questions, medium difficulty, about this change. Clicking an answer shows right or wrong and one sentence why.

Rules:
- Explain, don't praise. Say plainly what you are unsure about.
- If the diff is too large to explain well, say so at the top and explain the most important part first.
- No secrets, no customer data, no credentials, no real personal data in examples. Use made-up toy data.
- Do not change any code. Only write the HTML file. Then tell me the path and stop.
