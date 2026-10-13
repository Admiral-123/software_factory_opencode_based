# Universal Software Factory for OpenCode

A skill-file-based software development framework. OpenCode is the execution harness; free-tier models are replaceable workers. The factory's purpose is to reduce unreliable "slot machine" coding through specification-first planning, small tasks, evidence-driven verification, bounded repair, and explicit completion gates.

## Layout

- `AGENTS.md`: always-on factory rules and entry point.
- `.opencode/skills/*/SKILL.md`: reusable skills in OpenCode's discoverable skill format.
- `templates/PROJECT_SKILL_TEMPLATE.md`: the standard project specification format.
- `the_project/project_skill.md`: the only project-specific input you should normally need to author.
- `the_project/`: the actual project repository/workspace being implemented.

## Start

1. Open the `universal-software-factory-opencode` directory in OpenCode.
2. Put your project requirements in `the_project/project_skill.md`.
3. Tell OpenCode: `Read AGENTS.md and the factory skills. Execute the software factory for the_project/project_skill.md. Do not skip planning, verification, or the completion audit.`
4. Keep all implementation changes inside `the_project/`, except when explicitly updating the factory itself.

## Operating contract

The factory is model-agnostic at the instruction/workflow layer. Different models may still vary in capability, tool support, context limits, and reliability. Keep tasks small enough for free-tier context windows and use persistent Markdown artifacts instead of expecting the model to remember everything.

The workflow is:

`UNDERSTAND → PLAN → DEFINE ACCEPTANCE → IMPLEMENT ONE TASK → VERIFY → REPAIR IF NEEDED → REVIEW → INTEGRATE → COMPLETION AUDIT`

Do not treat a model's assertion as evidence. Use real test/build/analyzer output. If a check cannot run, mark it BLOCKED, not PASS. If requirements are materially ambiguous, ask one focused question. Never claim the project is complete when mandatory acceptance criteria remain unmet.

## Context-budget rules

- Do not load every skill at once. Start with `AGENTS.md`, the orchestrator skill, and project skill; load other skills only when the current phase needs them.
- Inspect the repository before changing it.
- Keep a concise project map and `the_project/docs/FACTORY_STATE.md` up to date.
- Work on one small task per iteration.
- Before context runs low, write a handoff to `FACTORY_STATE.md`: current task, completed work, changed files, commands/results, unresolved issues, next action.
- Prefer targeted file reads over dumping whole directories.
- Never redo completed work unless new evidence shows it is wrong.
- Do not spawn parallel agents unless tasks are independent, file ownership is clear, and integration checks are defined.

## Suggested first run prompt

> Read the root AGENTS.md and the factory orchestrator skill. Read `the_project/project_skill.md`, inspect the current contents of `the_project/`, and compare the actual state with the desired outcome. First produce/update a concise plan and acceptance criteria. Do not start implementation until the plan is coherent. Then implement the smallest complete task, run its relevant checks, repair failures within the configured attempt limit, and record evidence. Continue task-by-task. Do not claim success for unverified requirements.
