# HydroModel Wiki

An LLM-maintained research wiki for hydrology modeling.

This repository is an Obsidian-based knowledge vault focused on hydrological modeling, natural runoff and streamflow reconstruction, forcing uncertainty, river-flow connectivity in China, and newer interpretable physics-AI hydrology methods. Raw papers and supporting materials live under `raw/`. Codex reads those sources and incrementally builds a structured wiki under `wiki/`.

## Why This Exists

Typical RAG-style workflows re-read source documents every time. This repo uses a different pattern:

- keep raw sources immutable
- build persistent source pages and topic pages in markdown
- accumulate cross-links, caveats, and comparisons over time
- preserve useful analyses as part of the wiki instead of losing them in chat history

The result is a compounding research workspace rather than a pile of files.

## Scope

Current focus areas include:

- hydrological modeling in China
- natural runoff and streamflow reconstruction
- precipitation-forcing uncertainty and error propagation
- river-flow connectivity, intermittency, and water-withdrawal impacts
- interpretable physics-AI hydrology and parameter regionalization methods

## Repository Layout

```text
raw/         immutable source documents
wiki/        LLM-maintained source pages, topic pages, and syntheses
docs/        workflow notes and operating experience
templates/   page templates for the wiki
AGENTS.md    Codex operating contract for this vault
```

Important subfolders:

- `raw/papers/` for papers and supplementary files awaiting ingest
- `raw/papers/ingested/` for papers and supplements that have already been ingested into the wiki
- `wiki/sources/` for per-source notes
- `wiki/topics/` for cross-source synthesis by concept
- `wiki/syntheses/` for durable answers, comparisons, and analyses

## Workflow

1. Put a paper, supplement, or note into the correct `raw/` folder.
2. Normalize the filename before ingest when practical.
3. Ask Codex to ingest the source.
4. Review the created or updated pages in `wiki/`.
5. After ingest, the raw file is normally moved into `raw/papers/ingested/` and the source-page frontmatter path is updated.
6. Ask questions against the wiki and write back durable answers.

Detailed procedures live in:

- [docs/raw-source-naming.md](docs/raw-source-naming.md)
- [docs/ingest-workflow.md](docs/ingest-workflow.md)
- [docs/query-writeback.md](docs/query-writeback.md)
- [docs/future-features.md](docs/future-features.md)

## Tooling

- Obsidian for browsing and graph navigation
- Codex for source ingestion, synthesis, and wiki maintenance
- `pdftotext` in the `agent` conda environment for PDF extraction, typically invoked here after `conda activate agent`
- optional future search tooling such as `qmd` once the vault grows larger

## Current Status

The wiki has been scaffolded and seeded with an initial corpus including:

- `CNRD v1.0`
- `High-quality reconstruction of China's natural streamflow`
- its supplementary materials
- `A mass-conserving-perceptron for machine-learning-based modeling of geoscientific systems`
- the 2024 precipitation-error propagation paper
- the 2025 river-flow-connectivity paper and its supporting information
- `Distilling hydrological and land-surface model parameters from physio-geographical properties using text-generating AI`

## Notes

- `.obsidian/` is intentionally ignored in git.
- `raw/` files are source-of-truth inputs and should not be edited in place.
- `AGENTS.md` stays tight; detailed operational practice goes into `docs/`.
