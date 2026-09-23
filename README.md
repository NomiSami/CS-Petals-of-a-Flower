# CS - Petals of a Flower
### A Cave Story Fanfic Project (AI-Assisted Draft)

This repository is the **central brain** for drafting a custom Cave Story fanfic titled **"Petals of a Flower"**.

It is organized to be navigated by a high-end LLM (the writer) with a lower-end intermediary agent (this Arena agent) that structures, cleans, and commits outputs.

#### Repository Navigation for AI — READ IN ORDER

1. `outline/original-basic-outline.md` — User's original 7-bullet seed (source truth, verbatim)
2. `PROJECT_BIBLE.md` — Absolute canon, tone, rules, revised per user notes. **Read this first. Never contradict.**
3. `meta/user-notes.md` — User's personal notes while reading model response, verbatim + mapping
4. `prompts/revision-guide.md` — What to revise for next pass (1 chapter delivery, more Mimigas, etc.)
5. `outline/overall-plot.md` — Plot structure, 5 Petals, POV rotation, major threads (1 chapter per installment)
6. `outline/chapter-outline.md` — Chapter breakdown (42 sections, but flexible, opportunistic changes allowed)
7. `outline/timeline.md` — Timeline (thousands -> hundreds -> dozens)
8. `lore/worldbuilding.md` — Worldbuilding, expanded per user notes (tundra/marsh/lakeside, separate populations, flower multi-use)
9. `lore/mimiga-lore.md` — Mimiga culture, meal vs soul flowers
10. `lore/island-map.md` — Map, Cradle dozens not six, Old Village separate
11. `characters/protagonists.md` + `antagonists.md` + `character-sheets/` — Character sheets including West/Plum/Trip, red-eyed pair, Arthur expanded
12. `prompts/system-prompt.md` — System prompt + generation settings (1 chapter, avoid canon lines, found text optional, mysticism allowed)
13. `prompts/next-pass-context.md` — Copy-paste brain pack for fresh thread to avoid cutoff
14. `meta/reasoning-distilled.md` — Distilled whys from first massive thinking trace (old, but useful)
15. `drafts/` — Actual story chapters (final output, 1 per installment)
16. `meta/` — Todo, changelog, ingestion log

#### Workflow for Large Model Outputs — CURRENT RULES

**DO NOT paste 10k+ word responses directly into chat.** Instead:
1. **URL Fetch:** Upload draft to GitHub Gist / Pastebin and give URL. Agent uses `fetch_page` in chunks (no context flood)
2. **File Attachment:** Attach .md/.txt — agent reads via file

The agent will:
- Clean/format draft
- Place in `drafts/chapter-XX.md` (1 per installment now)
- Extract lore/character into appropriate files
- Update changelog/todo

**Delivery:** **1 chapter per installment** (user revision 2026-09-22) — 2 was too much for required internal reasoning. Focus revisions. Hefty work allowed to expand.

#### Current Status
- [x] Scaffold built
- [x] Index outline ingested + reasoning distilled
- [x] Original basic outline saved verbatim
- [x] User notes integrated (more Mimigas, separate populations, West/Plum/Trip, flower multi-use, etc.)
- [x] Consistency pass (this commit)
- [ ] Prologue draft (next pass, revised with expanded Arthur)
- [ ] Chapter 1 draft

#### Tone Target — Revised
Cave Story-like: melancholic, quiet hope, isolated wonder, gentle tragedy. Doukutsu Monogatari style.
- Mimiga dialogue short plain present-focused, avoid exact canon lines (context changed) — write new matching voice
- Found text optional (sign/note/log/song) — good but not needed if strong start or continues active scene
- Opportunistic changes allowed — outline can change if plotpoints reveal themselves, model can make up unverifiable high-potential info for mysticism
- Keep title and contents coherent, diverge more from original next pass

#### Key User Revisions (2026-09-22 gist 4b2d8789)
- Cradle dozens not six, Old Village separate population many buildings purposes
- Village numbers: before war thousands/lot, after hundreds, during Mugen+Doctor dozens Cradle
- King process more involved than cooking, 2 lesser red-eyed guy/gal + Sandaime lesser warrior without, Mugen rising intelligence
- Arthur expanded history/personality, Jack was Arthur's number two resourceful league above
- Flowers multi-use, simpler soul flowers energy/hunger/medicinal, rhyme disjointed revise/drop, Ume pupils, settlements exports soul flowers select villages
- Add tundra/marsh/lakeside settlements, hostile/support/friendly peoples moth people, caretaker Hozuki
- Add West/Plum/Trip, Hamachi liked
- Fates unknown reveal as write, gem=eye called gem by some
