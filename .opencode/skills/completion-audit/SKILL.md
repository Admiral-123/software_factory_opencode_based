---
name: completion-audit
description: Performs the final evidence-based audit and produces an honest project completion report.
---

# Completion Audit

For each MUST requirement:
1. Find its acceptance criterion IDs.
2. Find actual evidence for each criterion.
3. Mark PASS, FAIL, BLOCKED, or NOT RUN.
4. Check that tests correspond to the current working-tree state.
5. Review the diff and remaining known issues.

Final status:
- VERIFIED: all MUST criteria pass and required checks pass.
- PARTIALLY VERIFIED: some behavior works but mandatory criteria remain unproven.
- BLOCKED: missing access, credentials, environment, or decisions prevent completion.
- FAILED: a required behavior does not work.

Include implemented work, checks and results, evidence, known limitations, and next steps. Never equate "code written" with "project done".
