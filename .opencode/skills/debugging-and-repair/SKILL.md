---
name: debugging-and-repair
description: Diagnoses failures from evidence and performs bounded root-cause repairs rather than random edits.
---

# Debugging and Repair

- Start from the exact failing assertion, error message, stack trace, or observed mismatch.
- Reproduce the failure where possible.
- State a short hypothesis and why the evidence supports it.
- Change the smallest relevant area.
- Rerun the failing check first, then relevant regression checks.
- Do not make unrelated changes while debugging.
- After two unsuccessful attempts, stop repeating the same strategy. Reassess the diagnosis and report blockers honestly.
- Keep a record of what was tried and what evidence changed.
