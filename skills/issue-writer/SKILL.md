---
name: issue-writer
description: Use when the user wants to turn a feature, bug or spec section into one or more well-scoped issues (GitLab, GitHub or Jira) for the team repo.
---

# Issue writer

1. Read `spec.md` (or `docs/spec.md`), `plan-notes.md` if it exists, and `AGENTS.md` first.
2. Slice the request into issues that each fit in one working session and one small diff (vertical slices: each issue delivers something a user or test can see).
3. For each issue write:
   - **Title**: verb + object, under 70 characters
   - **Why**: one sentence, linked to the spec goal or journey
   - **What**: 2 to 5 bullet points
   - **Done when**: checkable acceptance criteria, including the test command from AGENTS.md
   - **Not in this issue**
   - **Size**: S (under 1 hour) / M (half a day). Anything larger: split it.
4. Show the list and ask before creating anything. Only when the user confirms, create the issues with the tool they name (for example `glab issue create` or `gh issue create`), or save them as `docs/issues/NNN-<slug>.md`.
5. Never use real customer or personal data in issue text.
