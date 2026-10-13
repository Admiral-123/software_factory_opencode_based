---
name: factory-orchestrator
description: Runs the Universal Software Factory workflow for the project in ../the_project. Use at the start of a project run or when deciding the next factory phase.
---

# Factory Orchestrator

## First actions
1. Read root `AGENTS.md`.
2. Read `the_project/project_skill.md`.
3. Inspect the repository under `the_project/` before proposing changes.
4. Read `the_project/docs/FACTORY_STATE.md` if it exists.
5. Load only the phase skill needed now.

## Phase protocol
Use these named phases and record the current phase in `the_project/docs/FACTORY_STATE.md`:

`UNDERSTAND → PLAN → IMPLEMENT → VERIFY → REPAIR → REVIEW → INTEGRATE → AUDIT`

### UNDERSTAND
- Summarize objective, users, MUST requirements, constraints, and out-of-scope items.
- Inspect existing files, stack, tests, and current behavior.
- Identify unknowns that materially affect architecture or data safety.
- Ask only focused blocking questions.

### PLAN
- Map each MUST requirement to acceptance criteria and verification evidence.
- Split work into small, dependency-aware tasks.
- Each task should ideally fit within one modest model context and change a small coherent slice.
- Define task scope, likely files, dependencies, and checks before coding.
- Do not begin a large implementation from a vague high-level plan.

### IMPLEMENT
- Select one ready task.
- Read its relevant source and tests.
- Make the smallest coherent change.
- Do not refactor unrelated code.
- Update tests and docs when behavior changes.
- Update the persistent state before moving on.

### VERIFY
- Run the strongest available relevant checks.
- Inspect the real output and exit status.
- Map results back to acceptance criteria.
- Mark checks PASS, FAIL, BLOCKED, or NOT RUN.

### REPAIR
- Fix the demonstrated root cause, not just the visible symptom.
- Retry at most twice for the same failure without a materially different diagnosis.
- If still failing, inspect assumptions, simplify, or mark BLOCKED and explain why.

### REVIEW
- Inspect the full diff.
- Look for security flaws, data loss, missing edge cases, brittle assumptions, test weakening, and unrelated changes.
- Resolve blocking findings before integration.

### INTEGRATE
- Ensure task interfaces fit together.
- Run relevant integration and regression checks.
- Resolve conflicts deliberately; never discard changes without understanding them.

### AUDIT
- Evaluate every MUST requirement against its acceptance criteria and evidence.
- Produce a verification report.
- Never claim full completion if any MUST criterion is failed, blocked, or unverified.

## Free-tier operating mode
- Do not load all skills at once.
- Do not paste the whole repository into context.
- Keep a compact state file and task notes.
- Do one task per iteration; parallelize only if file ownership and interfaces are genuinely independent.
- If the model context is near its limit, write a handoff and stop cleanly.
