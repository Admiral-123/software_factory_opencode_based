---
name: code-review
description: Reviews changes against the project skill for correctness, security, regressions, and maintainability.
---

# Code Review

Review the actual diff, not just the implementation summary.

Check:
- Requirement and acceptance-criteria coverage.
- Edge cases and error paths.
- Security, privacy, authorization, and secret handling.
- Data loss, migrations, and backwards compatibility.
- Interface consistency and dependency direction.
- Meaningful tests and whether they prove the claim.
- Unrelated edits, unnecessary dependencies, disabled checks, and weakened tests.

Findings must include severity, location, why it matters, and a concrete remedy. Resolve blocking findings before declaring a task verified. Review scores are advisory; passing mandatory checks and resolving blocking issues are required.
