---
name: weekly-review
description: Review the week against goals, update _ops/this-week.md and priorities.md, plan the next week. Triggers on - weekly review, plan my week, review my week, close the week, new week.
---

# Weekly review

A 15-minute ritual: look back honestly, then point the new week at what matters.

## Process

1. **Gather**: read the closing week's daily logs (`daily/`), `_ops/this-week.md`, active project READMEs, and `_context/goals.md`.
2. **Look back**, show the user:
   - What shipped (from dailies and project logs)
   - What was planned but did not happen, and the honest pattern if one repeats
   - Wins worth keeping (these feed content-draft later)
3. **Look forward**, ask:
   - "If only one thing ships next week, what is it?"
   - Confirm up to 3 focus items; push back if they conflict with `_context/goals.md` or the not-doing list
4. **Write**:
   - Rewrite `_ops/this-week.md` for the new week (carry honest leftovers, do not silently drop them)
   - Update `_ops/priorities.md` if the standing order changed; note the change in `_ops/decisions.md` if it is a real shift
   - Append a short week summary to the last daily log of the week
5. End with the new week on one screen.

## Rules

- Three focus items maximum; the user can override but say why fewer is better once.
- Carried-over items get marked `(carried, week N)` so chronic carries become visible.
