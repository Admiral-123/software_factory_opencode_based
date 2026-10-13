---
name: context-management
description: Preserves progress and minimizes token/context consumption during long coding tasks and free-tier model sessions.
---

# Context Management

- Read the project skill, current state, current task, and only the files relevant to that task.
- Do not load every skill; load skills just in time.
- Prefer targeted search and small excerpts to whole-file dumps.
- Avoid repeating the full project description in every prompt.
- Persist important decisions and current status in `the_project/docs/FACTORY_STATE.md`.
- Keep task artifacts concise: current objective, constraints, changed files, checks/results, blockers, next action.
- Before context exhaustion, stop after a safe checkpoint and write a handoff.
- On resume, read the handoff and verify repository state before continuing.
- Never assume memory of an earlier model session.
- Use one task per model context when practical.
