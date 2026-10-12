---
name: retro
description: Review recent work for recurring friction and propose one targeted improvement (instruction, helper rename, lint rule, hook, or test fix). Run after a feature or a painful session.
disable-model-invocation: true
---

1. Look at recent commits, notes, and the session: where was time lost (searching for code, re-asking, repeated mistakes, flaky checks)?
2. For each recurring cause pick the smallest fix:
   - Missing context -> a line in `CLAUDE.md` or a navigation note.
   - A mistake a machine can reliably catch -> a lint rule, test, or hook (confirm the hook schema in current docs first).
   - Confusing name -> rename the helper.
   - Flaky test -> diagnose the behavior it protects; never delete or skip it to get green.
3. Propose at most 3 changes; apply only those with a confirmed recurring cause. Don't accumulate rules; remove rules that no longer earn their place.
4. Log the outcome in `DECISIONS.md`.
