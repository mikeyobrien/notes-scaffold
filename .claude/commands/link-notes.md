Scan the note at $ARGUMENTS for entities (people, concepts, tools, books, projects, places) and add [[wikilinks]] throughout the text.

Rules:
- Only add wikilinks where they make semantic sense — don't link common words
- If the linked entity doesn't have a vault note yet, create a stub in the appropriate 02-reference/ subfolder with basic frontmatter
- Don't duplicate links — if an entity is mentioned multiple times, only link the first occurrence
- Preserve the original text — insert wikilinks around existing words, don't rephrase
- Show the user a summary of links added and any new stubs created

If no argument is provided, ask the user which note to process.
