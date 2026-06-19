---
name: daily-log
description: Create and close out daily logs at daily/YYYY/YYYY-MM/YYYY-MM-DD.md. Triggers on - start my day, daily log, open today, end my day, close my day, what did I do today, log this.
---

# Daily log

One file per day at `daily/YYYY/YYYY-MM/YYYY-MM-DD.md`, stamped from `_templates/daily.md`.

## Start of day ("start my day")

1. Create today's file from the template (create the YYYY/YYYY-MM folders if needed). If it already exists, open and show it instead.
2. Pull focus candidates from `_ops/this-week.md` and yesterday's "Tomorrow" section. Propose up to 3 focus items; let the user adjust.
3. Show the day in one screen.

## During the day ("log this: ...")

Append a timestamped line to today's Log section. Create today's file first if it does not exist.

## End of day ("end my day")

1. Ask: what got done, what is worth calling a win, what carries to tomorrow.
2. Fill Wins and Tomorrow. Check off completed focus items.
3. If anything done today completes an item in `_ops/this-week.md`, check it off there too.
4. If a decision got made today, offer to append it to `_ops/decisions.md`.

## Rules

- Never backfill days the user did not talk about; an empty day stays absent.
- Keep entries terse; this is a log, not a journal essay (unless the user writes one).
