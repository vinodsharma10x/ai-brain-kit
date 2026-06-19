---
name: wiki
description: Maintain the two-layer knowledge base - ingest raw/ sources into wiki/ pages, answer questions from the wiki, lint for gaps. Triggers on - ingest this, ingest, add to wiki, query the wiki, what does the wiki say, search the wiki, lint the wiki, wiki audit.
---

# Wiki

The user drops sources into `raw/` (their layer, never edit it). You distill knowledge into `wiki/` pages (your layer). Maintain `wiki/index.md` and `wiki/log.md` on every operation.

## Operation: ingest

Trigger: "ingest (file or topic)" or after inbox-triage routes something to raw/.

1. Read the source in `raw/`.
2. Decide: does this update existing pages, create new ones, or both? Check `wiki/index.md` first; prefer enriching an existing page over creating a near-duplicate.
3. Write or update pages. Every page gets:
   - YAML frontmatter: `type` (concept | person | tool | framework | synthesis), `tags`, `sources` (the raw/ file paths), `created`, `updated`
   - [[wikilinks]] to related pages; a link to a page that does not exist yet is fine, it marks future work
   - Distillation, not transcription: the page is what the source MEANS, a few paragraphs, not a copy
4. Update `wiki/index.md` (alphabetical within sections by type).
5. Append one line to `wiki/log.md`: date, operation, pages touched, source.

## Operation: query

Trigger: "what does the wiki say about X".

1. Read `wiki/index.md`, open the relevant pages, follow wikilinks one hop.
2. Answer from the pages, citing each page used. If the wiki has nothing, say so plainly; never invent coverage.

## Operation: lint

Trigger: "lint the wiki".

Report three lists: contradictions between pages, orphan pages (nothing links to them), and red links ([[wikilinks]] with no page) ranked by how often they are referenced. Offer to fix the top items.
