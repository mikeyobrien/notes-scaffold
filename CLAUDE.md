# Notes Vault — Claude Code Context

## Vault Purpose

Mixed-use personal knowledge management: writing & publishing, learning & research, work journaling, and general second-brain note-taking.

## Folder Structure

| Folder | Purpose | What goes here |
|--------|---------|----------------|
| `00-inbox/` | Capture | Raw thoughts, fleeting notes, unprocessed items |
| `01-thinking/notes/` | Processing | Exploration, analysis, working through ideas |
| `02-reference/approaches/` | Reference | Methods, frameworks, mental models |
| `02-reference/sources/` | Reference | Articles, books, papers, external material |
| `02-reference/tools/` | Reference | Tool docs, configs, how-tos |
| `03-creating/drafts/` | Creation | Works in progress, draft articles/posts |
| `04-published/` | Published | Finalized, polished content |
| `05-archive/` | Archive | Deprecated or historical content |
| `06-system/` | System | Vault conventions, templates, meta-notes |
| `attachments/` | Media | Images, PDFs, non-markdown files |

## Note Pipeline

Notes flow through stages: `00-inbox` → `01-thinking` → `03-creating` → `04-published` → `05-archive`

Reference material (`02-reference`) is evergreen and doesn't follow the pipeline.

## Formatting Conventions

### Filenames
- Lowercase kebab-case: `api-rate-limits.md`, `weekly-review-2025-01-28.md`
- Be specific: `auth-token-bug.md` not `quick-thought.md`
- Dates in filenames use `YYYY-MM-DD` prefix when relevant

### Frontmatter
Every note should have YAML frontmatter:
```yaml
---
title: Note Title
created: YYYY-MM-DD
tags: [tag1, tag2]
stage: inbox | thinking | reference | creating | published | archive
---
```

### Links
- Use `[[wikilinks]]` for internal vault references
- Use standard `[text](url)` markdown for external URLs
- Link liberally — any notable person, concept, book, or project is a potential `[[wikilink]]`

### Structure
- One `# H1` title per note (matches the `title` frontmatter)
- Use `## H2` and below for sections
- Keep notes atomic — one idea per note when possible

## Behaviors

- **Be opinionated**: Auto-file notes into the correct folder, add frontmatter, create backlinks
- **Link aggressively**: When creating or editing notes, add `[[wikilinks]]` for entities (people, concepts, tools, books, projects)
- **Create entity notes**: If a wikilinked entity doesn't have a note yet, create a stub in the appropriate folder
- **Respect the pipeline**: New raw captures go to `00-inbox/`, processed thoughts to `01-thinking/`, etc.
- **Never delete without asking**: Move to `05-archive/` instead of deleting
