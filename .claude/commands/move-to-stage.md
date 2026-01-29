Move a note to the next stage in the vault pipeline.

Pipeline: 00-inbox → 01-thinking/notes → 03-creating/drafts → 04-published → 05-archive

Usage: /move-to-stage <filepath> [target-stage]

Process:
1. Read the note at $ARGUMENTS (or ask which note if not specified)
2. Determine its current stage from the folder location or frontmatter
3. If no target stage specified, advance to the next stage in the pipeline
4. Move the file to the target folder
5. Update the `stage` field in frontmatter to match
6. Confirm the move with old and new paths

Rules:
- Reference notes (02-reference/) don't follow the pipeline — warn if user tries to move them
- If moving to 04-published, ask the user to confirm the note is ready
- If moving to 05-archive, ask for confirmation
- Update any daily review notes that reference the old path (if practical)
