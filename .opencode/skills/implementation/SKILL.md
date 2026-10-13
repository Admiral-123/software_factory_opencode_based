---
name: implementation
description: Implements one bounded task while preserving existing behavior and following the project skill.
---

# Implementation

Before editing:
- Read the task and acceptance criteria.
- Read relevant source files and tests.
- Identify affected interfaces and likely regressions.

While editing:
- Implement only the current task.
- Prefer minimal diffs over file rewrites.
- Preserve existing behavior unless the specification says otherwise.
- Do not invent API behavior; inspect docs, types, or current callers.
- Do not hide errors, weaken tests, disable lint rules, or hardcode secrets.
- Add/update tests for changed behavior.
- Avoid changing dependency manifests unless needed and authorized.

After editing:
- Inspect the diff.
- Explain which acceptance criteria the change targets.
- Run relevant verification before marking the task complete.
