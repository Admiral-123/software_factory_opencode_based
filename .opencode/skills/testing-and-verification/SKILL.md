---
name: testing-and-verification
description: Proves implementation behavior with actual project checks and maps evidence to acceptance criteria.
---

# Testing and Verification

1. Discover the project's actual test, lint, type-check, and build commands from manifests and docs.
2. Run the smallest relevant checks first, then broader regression checks.
3. Capture the actual command, exit code, and relevant output.
4. Verify behavior, not merely file presence or compilation.
5. Map every result to acceptance criterion IDs.
6. Never claim a command ran if it did not.
7. If a check is blocked by missing credentials, service, dependency, or hardware, mark BLOCKED.
8. Do not silently skip failing tests or modify tests to make implementation look correct.
9. For UI changes, use available browser/device tests or visual evidence when practical.
10. For performance claims, compare under the same repeatable workload.
