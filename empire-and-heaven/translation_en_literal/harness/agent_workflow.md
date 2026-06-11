# Agent Workflow

## Roles

### Coordinator

- Owns the chapter queue
- Decides which chapter moves next
- Confirms draft, review, and final status
- Prevents cross-contamination with `adaptation_en`

### Planner

- Reads the Korean chapter
- Splits only at paragraph boundaries
- Keeps speeches and scene pivots intact
- Records target segment count in the planning manifest

### Translator

- Translates from Korean source only
- Produces full content for the assigned segment or full draft
- Keeps proper nouns and historical terms consistent
- Flags uncertain terms in the review note instead of silently guessing

### Reviewer

- Compares English against the Korean source
- Checks for omission, compression, and theological drift
- Checks readability for American Christian readers
- Approves promotion to `final/` only after coverage is secure

### Review Coordinator

- Owns the review queue after translation is complete
- Assigns source review and continuity review in order
- Records the final decision in the manifest
- Ensures no chapter is promoted before the review note is complete

## Working Order

1. Coordinator selects chapter
2. Planner confirms segment count
3. Translator produces draft
4. Review Coordinator starts review
5. Source Reviewer checks the draft against the Korean source
6. Continuity Reviewer checks terms and adjacent-chapter flow
7. Reviewer writes the review note and decision
8. Coordinator promotes cleared output to `final/`

## Merge Rule

When a chapter is translated in segments, the merged chapter must be reviewed as a whole chapter before final promotion.
