---
name: clarify
description: Use before implementing an ambiguous or consequential feature (billing, data model, user-facing behavior, migrations) to surface hidden decisions. Skip for routine edits and obvious tasks.
---

Goal: expose decisions whose different answers would change data, architecture, UX, billing, or tests, before code exists.

1. Inspect the repo first; answer from evidence anything the code or docs already settle.
2. List consequential unknowns only. Resolve routine implementation choices yourself and state them as reversible defaults.
3. Walk the dependency tree: an answer may expose the next layer (e.g. "pause subscription" -> does billing stop? what about already-packed orders? max length? resume? refunds? reminders?). Stop when a coherent behavioral contract exists. There is no target question count.
4. Ask the smallest high-impact set, batched, each with your recommended answer. If the user is unavailable, proceed on defaults and record them.
5. Define terms: when two words might be conflated (e.g. pause vs skip), pin one meaning each and add them to `GLOSSARY.md`. Use them consistently in UI, data, code, tests.
6. If the uncertainty is visual or interaction feel, build a throwaway prototype (label simulated vs real logic) instead of asking in words.
7. Record settled decisions in `DECISIONS.md`; hand off to `/to-spec` if the work is significant.
