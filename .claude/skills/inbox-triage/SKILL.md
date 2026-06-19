---
name: inbox-triage
description: Process everything in inbox/ and route each item to its proper home (projects, people, areas, raw, ops). Triggers on - process my inbox, triage inbox, clean inbox, empty my inbox, route my inbox.
---

# Inbox triage

Take every item in `inbox/`, decide where it belongs, move it after the user confirms.

## Process

1. List everything in `inbox/`. If empty, say so and stop.
2. Read each item and classify it:
   - About a specific person → `people/<name>/` (create the person if new, from `_templates/person.md`)
   - About an active project → that project's folder; add a line to the project README log if relevant
   - Source material worth keeping (article, transcript, reference) → `raw/`, and offer to ingest it into the wiki
   - A task or commitment → add it to `_ops/this-week.md` (this week) or the relevant project's Now list
   - An idea with no home yet → `areas/` or leave a note proposing a new project
   - A decision that got made → append to `_ops/decisions.md`
3. Present the full routing plan as a table: item, destination, why. Wait for confirmation.
4. Move the files (never delete; anything truly worthless goes to `archive/inbox/`). Update `updated:` frontmatter where touched.
5. Confirm: "inbox is empty, N items routed."

## Rules

- One confirmation for the whole batch, not per item.
- When unsure between two homes, pick one and say why; do not ask about every item.
- A file mentioning a person AND a project goes to the project, with a one-line pointer added to the person's profile history.
