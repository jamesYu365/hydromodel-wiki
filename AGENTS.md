# LLM Wiki Operating Schema

## Purpose

This repository is a research-focused LLM wiki maintained by Codex.

The wiki is the working knowledge base. Raw sources are the source of truth. Codex reads raw sources, synthesizes their contents into the wiki, maintains cross-links, and keeps the wiki coherent over time.

## Repository Structure

- `raw/`: immutable source materials
- `raw/assets/`: downloaded images and attachments associated with sources
- `wiki/`: maintained markdown knowledge base
- `wiki/sources/`: per-source summary pages
- `wiki/topics/`: concept and topic pages
- `wiki/entities/`: people, organizations, products, places, papers, or other named entities when needed
- `wiki/syntheses/`: higher-level analyses, comparisons, and answers worth preserving
- `templates/`: canonical page templates

## Environment

- Use the `agent` conda environment by default for repo commands and tooling.
- On this machine, prefer `conda activate agent` and then run the command, instead of `conda run`, because the current console is typically `gbk` encoded and `conda run` can break on Unicode-heavy output.
- `pdftotext` is installed in the `agent` environment and should be used there for PDF text extraction.
- If a command fails outside `agent`, retry it inside `agent` before assuming the tool is unavailable.
- On Windows, assume the terminal may default to `gbk`. For Python commands that print extracted document text, prefer UTF-8-safe execution such as `python -X utf8 ...` or emit ASCII-safe / escaped output when needed.

## Raw Source Naming

- Follow [docs/raw-source-naming.md](H:\myprj\LLM_Wiki\docs\raw-source-naming.md) as the source of truth for naming and placement rules.
- Once a source has been ingested and recorded in `wiki/index.md`, move its raw file from `raw/papers/` into `raw/papers/ingested/` by default and update the corresponding `wiki/sources/` frontmatter path at the same time.

## Global Rules

1. Never modify files under `raw/`.
2. Prefer updating the existing wiki over creating duplicate pages.
3. Use Obsidian-style markdown links such as `[[overview]]` and `[[topics/example-topic]]`.
4. Keep page names stable once created.
5. Every meaningful page should be linked from at least one other page and listed in `wiki/index.md`.
6. Record every ingest, major query writeback, and lint pass in `wiki/log.md`.
7. When new evidence conflicts with older claims, update the affected pages and note the conflict explicitly instead of silently overwriting meaning.
8. Do not invent facts. Mark uncertainty, ambiguity, and open questions clearly.

## Required Frontmatter

All pages in `wiki/` should begin with YAML frontmatter using only these fields unless the user asks for more:

```yaml
---
title: ""
type: ""
status: active
created: YYYY-MM-DD
updated: YYYY-MM-DD
sources: []
---
```

## Ingest Workflow

Follow [docs/ingest-workflow.md](H:\myprj\LLM_Wiki\docs\ingest-workflow.md).

Additional default:

- After completing an ingest and updating `wiki/index.md`, move the ingested raw source artifact into `raw/papers/ingested/` unless the user explicitly wants a different placement.

## Query Workflow

Follow [docs/query-writeback.md](H:\myprj\LLM_Wiki\docs\query-writeback.md).

## Future Tooling

- Follow [docs/future-features.md](H:\myprj\LLM_Wiki\docs\future-features.md) for deferred tooling such as `qmd`.

## Lint Workflow

Check for stale claims, conflicts, orphan pages, missing cross-links, thin summaries, and duplicate concepts. Log each lint pass in `wiki/log.md`.

## Naming Conventions

- Use lowercase kebab-case filenames.
- Prefer short, stable names.
- Avoid near-duplicate topic names.

## Default Operating Assumptions

- The user curates the source collection manually.
- Markdown and PDF are first-class source types.
- The wiki is optimized for Obsidian browsing.
- No external search infrastructure is required in v1.
