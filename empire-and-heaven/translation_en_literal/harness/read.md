# Empire And Heaven Literal Translation Agent

This document captures the working pattern used in the `translation_en_literal` program so the same process can be repeated without re-deriving it.

## Mission

- Translate the Korean source into a full literal English version.
- Preserve meaning, sequence, theology, and historical texture.
- Avoid adaptation, compression, or omission.
- Keep the translation readable for an American Christian audience without loosening the source.

## Operating Principles

- Translate from the Korean source only.
- Do not import content from adaptation paths.
- Keep every paragraph, speech block, and scene transition intact.
- If a term is uncertain, document it in the review note instead of silently normalizing it.
- Review the chapter as a whole before promoting it to `final/`.

## Role Split

### Coordinator

- Tracks the chapter queue.
- Confirms whether a chapter is still in draft, under review, or finalized.
- Prevents cross-contamination with any other translation path.

### Planner

- Reads the Korean chapter and checks the chapter boundary.
- Confirms whether the chapter can be handled as a whole unit.
- Keeps the chapter flow intact.

### Translator

- Produces the literal English draft from the Korean source.
- Keeps names, titles, and historical references consistent with the term policy.
- Maintains full coverage without summarizing.

### Reviewer

- Compares the Korean source and the English draft line by line.
- Checks for omission, compression, doctrinal drift, and continuity breaks.
- Approves finalization only when the chapter is safe for publication handling.

## Term Control

- Use the canonical forms in `term_policy.md`.
- Use the glossary in `glossary.md` for recurring names and titles.
- Keep `Christianus`, `Christiani`, and `Christiana` distinct when the source requires it.
- Use `my lord` for direct honorific address when the context is dialogue.
- Keep `master` only where it is a literal title, office, or household relation.

## Chapter Workflow

1. Confirm the chapter source.
2. Confirm the draft exists.
3. Read the review note and the manifest row.
4. Check source coverage against the Korean chapter.
5. Check continuity with neighboring chapters.
6. Normalize terminology only when the source supports it.
7. Update the review note status.
8. Update the manifest status.
9. Copy the draft into `final/`.
10. Verify that review, manifest, and final file match.

## Final Gate

A chapter is complete only when:

- the draft exists,
- the review note exists,
- source coverage has been checked,
- no major omission remains open,
- the final file exists in `final/`,
- the manifest is marked `finalized`.

## Notes From This Run

- The full program reached `v2_ch12`.
- The glossary and term policy were added first.
- Review note language was normalized across all 22 chapters.
- The final directory contains 22 completed chapters.
- The manifest is finalized through chapter 22.

