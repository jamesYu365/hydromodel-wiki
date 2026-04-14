# Ingest Workflow

Use this procedure when adding a new source into the wiki.

## Before Ingest

1. Confirm the source is in the correct `raw/` subfolder.
2. Confirm the raw filename is stable and normalized.
3. Skim the source and identify its type: paper, article, book material, note, or supplement.

## Ingest Steps

1. Read the raw source.
2. Check `wiki/index.md` for existing related coverage.
3. Create or update a source page in `wiki/sources/`.
4. Update related topic pages in `wiki/topics/`.
5. Create or update entity pages only when they are clearly useful and likely to recur.
6. Add links between the affected pages.
7. Update `wiki/index.md`.
8. Move the ingested raw artifact into `raw/papers/ingested/` when the source lives under `raw/papers/`, and update the `sources` frontmatter path in the corresponding source page.
9. Append an entry to `wiki/log.md`.

## Source Page Expectations

- Capture the main contribution or purpose of the source.
- Record the key claims, methods, evidence, and caveats.
- Link to the most relevant topic and entity pages.
- Keep the summary concise and useful for later synthesis.
- Ensure the frontmatter `sources` list points to the current raw-file location after any post-ingest move.

## Decision Rules

- Prefer updating existing topic pages over creating near-duplicates.
- If a source is supplementary material, connect it to the main paper page.
- If a source contradicts existing wiki content, note the conflict explicitly.
- If confidence is low, preserve uncertainty instead of forcing a conclusion.
- If a new paper introduces a distinct methodological thread, prefer adding a durable topic page over forcing it into an existing but mismatched topic.
