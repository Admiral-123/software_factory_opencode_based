# Project Skill — [Project Name]

> This document is the project-specific source of truth. Describe outcomes and constraints; the factory derives the implementation plan. Keep it concise but unambiguous.

## 1. Project identity
- **Name:**
- **One-sentence purpose:**
- **Target users:**
- **Existing repository:** `.` (relative to this file unless stated otherwise)
- **Project stage:** new / existing / refactor / bug fix

## 2. Desired outcome
Describe what the finished project must let a user accomplish. Focus on observable behavior, not implementation guesses.

## 3. Requirements
Use stable IDs. Mark each requirement MUST, SHOULD, or COULD.

- **REQ-001 — MUST:** [Specific behavior]
- **REQ-002 — SHOULD:** [Specific behavior]

## 4. Acceptance criteria
Every MUST requirement needs at least one observable pass/fail criterion.

- **AC-001:** Given [starting state], when [action], then [observable result].
  - Verification: [test, command, browser flow, or manual evidence]
- **AC-002:** ...

## 5. Stack and constraints
- **Required stack (if any):**
- **Existing conventions to preserve:**
- **Architecture requirements:**
- **Platforms/browsers/devices:**
- **Performance/accessibility requirements:**
- **Dependencies to avoid:**

If the stack is not prescribed, inspect the existing project and choose the simplest defensible option. Explain the choice before adding major dependencies.

## 6. Data, integrations, and security
- **Data model and ownership:**
- **External services/APIs:**
- **Authentication/authorization:**
- **Secrets policy:** never commit secrets; document required environment variables by name only.
- **Privacy and retention:**
- **Threats or abuse cases:**

Write `N/A` where appropriate.

## 7. UX and behavior
- **Core user journeys:**
- **Important empty/loading/error states:**
- **Visual direction or reference:**
- **Accessibility requirements:**

## 8. Out of scope
Explicitly list what must not be built in this iteration.

## 9. Change boundaries
- **Protected files/data:**
- **Actions requiring approval:**
- **Backward compatibility requirements:**
- **Migration/rollback expectations:**

## 10. Verification requirements
Specify relevant checks, not just “test it”.

- Static analysis/lint:
- Unit tests:
- Integration tests:
- End-to-end tests:
- Build/package:
- Security checks:
- Visual/performance evidence:

The factory must inspect the repository to discover available commands and must not invent successful results.

## 11. Definition of done
The project is done only when:
- [ ] Every MUST requirement maps to an acceptance criterion.
- [ ] All runnable mandatory checks pass.
- [ ] Unavailable checks are marked BLOCKED, never PASS.
- [ ] No known blocking security or correctness issues remain.
- [ ] Changes are reviewed for regressions and unrelated edits.
- [ ] Documentation and setup instructions match the actual implementation.
- [ ] The final report lists evidence, limitations, and remaining work.
