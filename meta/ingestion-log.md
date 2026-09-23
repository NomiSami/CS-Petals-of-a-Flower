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
|  |  |  |  |  |  |

## Example Usage

User: "Ingest https://gist.github.com/... chapter 01 draft"
Agent: fetches, cleans, writes to drafts/chapter-01.md, logs here.

## Notes
- Never paste 10k+ words directly — always use URL or file attachment.
- Agent will chunk-read via fetch_page if needed.
