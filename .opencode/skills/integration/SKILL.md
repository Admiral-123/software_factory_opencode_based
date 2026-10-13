---
name: integration
description: Integrates completed task slices and checks cross-module contracts and regressions.
---

# Integration

- Integrate only tasks whose prerequisites are verified.
- Inspect interface changes and all callers.
- Resolve conflicts by understanding both changes; do not blindly accept one side.
- Run integration tests and relevant regression checks after combining work.
- Check for duplicated implementations, inconsistent naming, mismatched schemas, and incompatible assumptions.
- Do not parallelize work that edits the same module or depends on an unsettled interface.
- Record the integrated commit/diff state and remaining risks.
