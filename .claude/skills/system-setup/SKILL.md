---
name: system-setup
description: First-session onboarding interview that fills _context/ with the founder or operator's business, product, customers, voice, goals, and standards. Triggers on - set up my system, setup system, system setup, onboard me, start here, interview me, getting started.
---

# System setup

Interview the user, then rewrite the `_context/` files with real content. This runs once; after it, every other skill has context to work with.

## Process

1. Check `_context/me.md`. If it does NOT contain `STATUS: TEMPLATE`, the system is already set up; ask whether they want to update specific context files instead, and stop.
2. Open as a conversation, not a system report: a short welcome, one line on what this is (a 10-minute conversation so everything the system does starts from who they actually are), then straight into the first question. Never mention templates, markers, or internal state.
3. Interview conversationally, a few questions at a time, never as one giant form. The user is a founder or operator; calibrate (a solo founder, someone running an existing business, or an operator on a small team). Cover, in order:
   - **Them and the business** (for `me.md`): name, role, one-sentence what the business does, stage, team size if any, working style, links.
   - **Product** (for `product.md`): name, one-liner, status, pricing, the problem, how it solves it.
   - **Customers** (for `icp.md`): who, the pain in the customer's words, where they hang out, what makes them buy.
   - **Positioning** (for `positioning.md`): category, alternatives, why-me sentence, what they are NOT.
   - **Goals** (for `goals.md`): up to three quarterly goals with numbers and dates, the year headline, the not-doing list.
   - **Voice** (for `voice.md`): ask them to paste 2-3 real writing samples. From the samples, extract tone, rhythm, vocabulary, opening and closing styles, formatting habits. Keep the samples in the file.
   - **Standards** (light, for the "Your standards" section of `CLAUDE.md`): one or two ways they want things done consistently, for example how a support reply should sound or how a recurring process runs. Skip easily if they have none yet; standards build up over time as they work.
4. Rewrite each `_context/` file: remove the `STATUS: TEMPLATE` line, fill the sections, set `updated:` to today. Put any standards captured into the "Your standards" section of `CLAUDE.md`.
5. Seed `_ops/this-week.md` with the current week and ask: "if only one thing ships this week, what is it?"
6. Finish by showing them three things to try next: drop something in `inbox/`, say "start my day", say "draft a post about X".

## Rules

- Skipped questions are fine; write `(not captured yet)` so a later session can fill the gap.
- Short answers are fine; never pad their words with invented detail.
- If they have no writing samples, draft 3 short sample paragraphs in different tones, ask which feels most like them, and note that voice.md is provisional until real samples replace it.
