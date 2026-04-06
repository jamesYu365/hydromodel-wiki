# Query Writeback

Use this procedure when answering questions against the wiki.

## Default Query Path

1. Read `wiki/index.md`.
2. Open the most relevant wiki pages.
3. Synthesize the answer from wiki content first.
4. Only return to raw files when the wiki is missing coverage or the user asks for source-level verification.

## When To Write Back

Write the result into `wiki/syntheses/` when the answer has durable value, such as:

- comparisons between papers or methods
- a timeline or trend summary
- a reusable concept explanation
- a decision memo
- a synthesis that connects multiple source or topic pages

## When Not To Write Back

Do not create a synthesis page for:

- trivial factual lookups
- one-off housekeeping answers
- questions already fully answered by an existing wiki page

## Writeback Steps

1. Create or update a page in `wiki/syntheses/`.
2. Link it to the relevant source, topic, and entity pages.
3. Update `wiki/index.md`.
4. Append a log entry to `wiki/log.md` if the writeback is substantial.

## Quality Bar

- Keep the synthesis tighter than chat output.
- Make the page understandable without the original conversation.
- Preserve uncertainty and disagreements where relevant.
