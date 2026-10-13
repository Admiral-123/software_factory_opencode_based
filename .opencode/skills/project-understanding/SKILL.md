---
name: project-understanding
description: Inspects the existing project and converts the project skill into a grounded picture of current state, constraints, and gaps.
---

# Project Understanding

1. Read `the_project/project_skill.md` fully.
2. Inspect the top-level tree, manifests, entry points, tests, configuration examples, and relevant docs.
3. Identify the language/framework from actual files, not guesses.
4. Record existing conventions, commands, architecture, and current behavior.
5. Separate observed facts from assumptions.
6. Do not read large unrelated files or generated/vendor directories.
7. Do not start coding during the understanding phase.
8. Create/update `the_project/docs/FACTORY_STATE.md` with a short repository map, current phase, confirmed facts, open questions, and next step.

If an existing project conflicts with the skill, report the conflict and propose the least disruptive path. Ask before destructive migrations.
