# Review Workflow

## Roles

### Review Coordinator

- Owns the review queue
- Selects the next chapter for review
- Confirms the draft exists before review starts
- Confirms whether the chapter can be promoted to `final/`

### Source Reviewer

- Compares the Korean source line by line against the draft
- Checks omission, compression, translation drift, and broken speech boundaries
- Notes unclear source text, OCR damage, or ambiguous names

### Continuity Reviewer

- Checks term policy alignment across chapters
- Checks whether a name, title, or biblical reference has shifted
- Checks whether the chapter still fits the adjacent chapter flow

### Gatekeeper

- Decides whether the draft is promoted, revised, or held
- Confirms the review note matches the evidence
- Moves the chapter to `final/` only after both reviews are clear

## Review Order

1. Confirm draft exists
2. Compare against the Korean source
3. Run continuity and term-policy check
4. Write the review note
5. Mark the manifest status
6. Promote to `final/` only if clear

## Review Output

Every reviewed chapter must produce:

- A review note in `translation_en_literal/review/`
- A manifest status update
- A clear final decision: `approve`, `revise`, or `hold`

## Review Decision Rules

- `approve`: no major omission, no broken continuity, no unresolved source-risk that blocks publication
- `revise`: the chapter is mostly correct but needs a repair pass before promotion
- `hold`: the chapter cannot be safely judged yet because the source or draft is incomplete
