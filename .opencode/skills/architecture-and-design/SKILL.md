---
name: architecture-and-design
description: Chooses or preserves a maintainable architecture grounded in the project's actual stack and requirements.
---

# Architecture and Design

1. Prefer existing working conventions unless the project skill requires a change.
2. Keep modules focused and interfaces explicit.
3. Separate presentation, domain behavior, and external I/O where appropriate for the stack.
4. Avoid unnecessary abstraction layers, speculative extensibility, and needless rewrites.
5. Document important decisions briefly, including tradeoffs.
6. Validate input at trust boundaries and handle errors explicitly.
7. Do not add a dependency unless it materially reduces complexity or is required.
8. Make architecture proportional to project size and expected change.
9. Do not create architecture documents that merely restate the code; record decisions that guide implementation.
