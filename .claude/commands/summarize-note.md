Create a concise summary of the note at $ARGUMENTS.

Process:
1. Read the full note
2. Generate a 2-4 sentence summary capturing the core idea, key points, and any action items
3. Present the summary to the user
4. Ask if they want the summary:
   a. Added to the note's frontmatter as a `summary` field
   b. Displayed only (no changes to the note)

Rules:
- Preserve the author's voice and intent — summarize, don't editorialize
- If the note has existing tags, use them as context for what matters
- For long notes (>500 words), also list the 3-5 most important takeaways as bullets
- If no argument is provided, ask which note to summarize
