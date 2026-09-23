# Ingestion Log — Large Model Responses

This file tracks how huge model outputs were ingested WITHOUT flooding chat context.

## Workflow

1.  You (user) upload draft to a URL (Gist, Pastebin, Catbox, etc.) OR attach file
2.  You give intermediary agent the URL / filename
3.  Agent uses `fetch_page` or `read_file` to pull in chunks
4.  Agent cleans and commits to `drafts/`

## Log Entries

| Date | Chapter | Source URL / File | Word Count | Status | Commit |
|------|---------|-------------------|------------|--------|--------|
| 2026-09-22 | Index / Bible + Reasoning | https://gist.github.com/NomiSami/5dc16e7e75612fc3cb2d609005830208 (raw: https://gist.githubusercontent.com/NomiSami/5dc16e7e75612fc3cb2d609005830208/raw/e653b2833846097e81efce8340daf0f3d85873e3/gistfile1.txt) | ~25 chunks, ~20k thinking + ~4k final | Parsed into PROJECT_BIBLE, outline/*, lore/*, characters/*, prompts/system-prompt, meta/reasoning-distilled | 4a4b0cb |
| 2026-09-22 | Original Basic Outline (user seed) | https://gist.github.com/NomiSami/20103ea669af1e34617070d504abb98b (raw: https://gist.githubusercontent.com/NomiSami/20103ea669af1e34617070d504abb98b/raw/78ecab277e6607a7bb20307a1660c85d09872976/gistfile1.txt) | ~300 words | Saved verbatim to outline/original-basic-outline.md, cross-checked vs bible | 3660c3a |
| 2026-09-22 | User Notes — Outline + Chapter Index feedback | https://gist.github.com/NomiSami/4b2d8789299fddf5ec07690cb2f22286 (raw: https://gist.githubusercontent.com/NomiSami/4b2d8789299fddf5ec07690cb2f22286/raw/6745ec9b062a56f3788e9b394baeb427debec2b6/gistfile1.txt) | ~800 words | Parsed into PROJECT_BIBLE.md, lore/worldbuilding.md, characters/protagonists.md + new sheets west/plum/trip/arthur-expanded/red-eyed-pair, meta/user-notes.md, prompts/revision-guide.md, outline/overall-plot.md, prompts/system-prompt.md | Pending |
|  |  |  |  |  |  |

## Notes
- Gist contained massive thinking trace + final planning doc. Thinking distilled into meta/reasoning-distilled.md keeping whys, removing bulk.
- Final output (plan) parsed into scaffold as above.
- Attached files "CS Custom Initial User Request.txt" and "Petals of a Flower Basic Outline.txt" were not found in filesystem (/home/user/uploads missing) — need re-upload via Gist URL or file attachment retry.
- Next expected: Prologue + Chapter 1-2 prose drafts (mentioned in gist as part of first installment but not present in this gist file). Await second gist.

## Example Usage

User: "Ingest https://gist.github.com/... chapter 01 draft"
Agent: fetches, cleans, writes to drafts/chapter-01.md, logs here.
