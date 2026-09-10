# Coding Planning Skill

Create a clear, minimal, and actionable implementation plan before making code changes.

## Planning Principles

- Understand the user's requested outcome before creating a plan.
- Inspect the existing codebase before deciding what needs to change.
- Search for related implementations, components, APIs, and patterns.
- Identify dependencies and potential side effects.
- Break the work into logical, outcome-oriented tasks.
- Keep tasks small enough to implement and verify independently.
- Order tasks based on dependencies.
- Prefer modifying existing code over creating new abstractions.
- Do not create tasks for trivial implementation details.
- Do not include obvious internal steps such as opening files or typing code.
- Include testing or verification as a task when appropriate.
- Keep the plan proportional to the complexity of the request.
- Revise the plan when codebase discoveries invalidate the original plan.

## Task Quality

Each task should:

- Have a clear outcome.
- Be independently understandable.
- Identify the relevant area of the codebase when known.
- Avoid combining unrelated changes.
- Avoid unnecessary implementation details.

Prefer:

- "Add authentication middleware to protected API routes"

Avoid:

- "Open auth.ts, find middleware function, add code, save file"

## Planning Workflow

1. Understand the request.
2. Inspect the relevant codebase.
3. Identify the affected areas.
4. Determine dependencies and implementation order.
5. Create the minimal task plan.
6. Execute tasks in order.
7. Update task status as work progresses.
8. Adjust the plan when new information requires it.