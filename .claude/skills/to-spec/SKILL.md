---
name: to-spec
description: Turn settled decisions into a short feature spec (problem, solution, user stories, edge cases, interfaces, acceptance criteria) and a dependency-ordered task list. Use for significant features, not small edits.
disable-model-invocation: true
---

Write the spec to `specs/<feature>.md`. Persist behavior, not the chat.

Sections:
- **Problem / Solution**: user-visible result, 2-5 sentences.
- **User stories**: include edge cases found during `/clarify`.
- **Boundary**: inspect the real architecture and name the module/interface where behavior is verified. Do not invent abstractions.
- **Acceptance criteria**: observable, testable, including denied/failure cases.
- **Reversibility**: affected users/data, migration compatibility, rollout, rollback. Charges, messages and destructive data changes cannot be reverted like code.
- **Tasks**: thin vertical slices (UI + API + data + test), with dependencies and a done condition each. Tasks sharing files or migrations are sequential.
- **Out of scope** and **Open questions**.

Update the spec when evidence changes it; it's a destination, not a waterfall contract. Link it from `PLAN.md`.
