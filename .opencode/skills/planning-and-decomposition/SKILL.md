---
name: planning-and-decomposition
description: Converts project requirements into small, testable, dependency-aware implementation tasks suitable for limited-context free-tier models.
---

# Planning and Decomposition

- Give every requirement and acceptance criterion a stable ID.
- Every MUST requirement must map to at least one acceptance criterion and a verification method.
- Split tasks by coherent behavior and ownership, not arbitrary file count.
- Prefer vertical slices that can be tested end-to-end.
- Define prerequisites and shared interfaces before parallel work.
- A task must state: goal, requirement IDs, acceptance criteria, scope, exclusions, dependencies, tests, and done condition.
- Avoid speculative features and overengineering.
- Identify the smallest useful milestone that provides real user value.
- If the plan cannot fit in a concise checklist, split it into milestones.
- Do not plan more than a few tasks ahead when later details depend on test results.
