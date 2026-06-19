---
name: new-project
description: Create a project folder with a structured README from the template. Triggers on - new project, start a project, create project, kick off.
---

# New project

1. Ask (if not given): the project name and what done looks like in one sentence.
2. Create `projects/<kebab-name>/README.md` from `_templates/project.md`: outcome, deadline if known, the single next physical action, a starter plan of 3-5 steps.
3. Ask whether this project belongs in this week's focus; if yes, add it to `_ops/this-week.md`.
4. If the project replaces or conflicts with a current priority, say so out loud and log the call in `_ops/decisions.md`.

## Rules

- Every project README answers, at a glance: what is the outcome, what is the next action, what is the status.
- Projects have ends. If the user describes something with no end state, suggest `areas/` instead.
