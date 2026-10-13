# Project Skill

> Replace this template with your actual project specification. This is the only project-specific document you should normally need to author.

## Objective
[What are we building, for whom, and what user problem does it solve?]

## Current state
- Project type: [new / existing]
- Existing code: [describe briefly or let the factory inspect]
- Required stack: [required stack or "inspect existing project and recommend"]

## Requirements
- **REQ-001 — MUST:** [observable feature]
- **REQ-002 — MUST:** [observable feature]
- **REQ-003 — SHOULD:** [valuable but non-blocking feature]

## Acceptance criteria
- **AC-001:** Given [state], when [action], then [observable outcome].
  - Verification: [test/build/browser flow/etc.]
- **AC-002:** ...

## Constraints
- Preserve existing working behavior.
- Avoid unnecessary dependencies and unrelated refactors.
- Never commit secrets.
- Ask before destructive actions, production changes, or data migrations.

## Out of scope
- [Explicitly list what should not be built now.]

## Definition of done
- Every MUST requirement has passing evidence.
- Relevant tests, static checks, and build checks pass where runnable.
- Blocked checks are reported as blocked, never passed.
- Final diff is reviewed for correctness, security, and unrelated changes.
- Setup and usage documentation matches the actual project.
