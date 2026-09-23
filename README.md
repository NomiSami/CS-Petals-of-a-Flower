# CS - Petals of a Flower
### A Cave Story Fanfic Project (AI-Assisted Draft)

This repository is the **central brain** for drafting a custom Cave Story fanfic titled **"Petals of a Flower"**.

It is organized to be navigated by a high-end LLM (the writer) with a lower-end intermediary agent (this Arena agent) that structures, cleans, and commits outputs.

#### Repository Navigation for AI

- `PROJECT_BIBLE.md` — Absolute canon, tone, and rules. Read this first. Never contradict.
- `outline/` — Plot structure, chapter breakdown, timeline
- `lore/` — Worldbuilding, Mimiga lore, Island geography
- `characters/` — Character sheets and motivations
- `drafts/` — Actual story chapters (final output)
- `prompts/` — System prompts and per-chapter prompts used to generate drafts
- `meta/` — Todo, changelog, and ingestion log

#### Workflow for Large Model Outputs

**DO NOT paste 10k+ word responses directly into chat.** Instead use one of:

1.  **File Attachment:** Attach a `.md` or `.txt` file in Arena chat. The agent can read it as a file.
2.  **URL Fetch:** Upload the draft to a paste service (GitHub Gist, Pastebin, etc.) and give the agent the URL. Agent will use `fetch_page` to ingest it in chunks without flooding context.
3.  **Direct Path:** Place file in `incoming/` and tell agent to process it.

The intermediary agent will then:
- Clean and format the draft
- Place it in `drafts/chapter-XX.md`
- Extract new lore/character info into appropriate files
- Update `meta/changelog.md` and `meta/todo.md`

#### Current Status
- [ ] Project Bible defined
- [ ] Outline complete
- [ ] Chapter 1 draft
- [ ] ...

#### Tone Target
Cave Story-like: melancholic, quiet hope, isolated wonder, gentle tragedy. Doukutsu Monogatari style.
