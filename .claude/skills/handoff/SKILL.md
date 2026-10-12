---
name: handoff
description: Write a concise handoff so a fresh session or another assistant can continue without guessing. Use when stopping mid-task, before clearing context, or switching sessions.
---

Update `PLAN.md` (or write `HANDOFF.md`) with exactly:

- **Version**: branch, latest commit, date.
- **Goal** (one line) and link to the spec.
- **Done**: only what is verified, each tagged implemented / tested locally / integrated / deployed.
- **Unverified**: what was assumed or not run, and why.
- **Decisions**: with reasons (also in `DECISIONS.md`).
- **Blocked / open**: what is needed and from whom.
- **Next action**: the single most useful next step, with the exact command or file.

Keep it under ~40 lines. No secrets or customer data. Commit it; conversation memory is not a backup.
