# Raw Source Naming

Use this procedure when organizing files under `raw/`.

## Principles

- Treat the raw file itself as the source of truth, not the incoming filename.
- Normalize names before ingestion whenever practical.
- Prefer manual judgment over brittle automation when the title page is noisy.
- Keep filenames stable after ingestion.

## Folder Placement

- Put research papers and supplements in `raw/papers/`.
- Put clipped articles in `raw/articles/`.
- Put books or book chapters in `raw/books/`.
- Put personal notes or ad hoc materials in `raw/notes/`.
- Use `raw/inbox/` only as a temporary landing zone.
- Keep attachments in `raw/assets/`.

## Filename Format

- Use lowercase kebab-case.
- Use `year-title-slug.ext` when a publication year is clear.
- Remove author prefixes, journal names, issue numbers, tracking IDs, and noisy suffixes.
- Use ASCII only in filenames.

Examples:

- `2022-high-quality-reconstruction-of-chinas-natural-streamflow.pdf`
- `2025-warming-climate-and-water-withdrawals-threaten-river-flow-connectivity-in-china.pdf`
- `2025-warming-climate-and-water-withdrawals-threaten-river-flow-connectivity-in-china-supporting-information.pdf`

## PDF Renaming Procedure

1. Extract the first page text in the `agent` environment with `pdftotext`.
2. Read the title block from the extracted text.
3. Ignore journal headers, section labels, DOI lines, citation blocks, and author affiliations.
4. Choose the actual paper title, even if it spans multiple lines.
5. Derive the normalized filename from the publication year and title.
6. Move the file into the correct `raw/` subfolder.

Example command:

```powershell
& 'D:\miniconda3\shell\condabin\conda-hook.ps1'; conda activate agent; pdftotext -f 1 -l 1 -layout ".\raw\papers\example.pdf" -
```

Windows terminal note:

- When using Python to print extracted text on this machine, prefer `python -X utf8 ...`.
- If output may still contain problematic characters, print escaped/ASCII-safe text rather than raw Unicode.

## Common Failure Patterns

- `RESEARCH ARTICLE`, `Article`, `Research papers`, and similar labels are not the title.
- Journal issue lines such as `Journal of X 632 (2024) 130906` are not the title.
- Supplement files often start with `Supporting Information for` or `Supplementary materials for`; keep that meaning in the final filename.
- Some title pages mix the title with callout boxes like `Key Points` or `Significance`; ignore those blocks.
- If the first page is still ambiguous, inspect the next page or choose manually.

## Default Decision Rule

If the extracted text does not make the title obvious, stop automatic handling and rename manually.
