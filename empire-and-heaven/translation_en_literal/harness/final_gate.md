# Final Gate

## Purpose

This gate prevents a chapter from being treated as publication-ready until translation, review, and continuity checks are complete.

## Required Inputs

- Korean source chapter
- English literal draft
- Review note
- Manifest row

## Final Conditions

A chapter may move into `final/` only if all of the following are true:

1. The draft exists
2. The review note exists
3. The review note does not leave a major omission unresolved
4. The manifest status is aligned with the review decision
5. The chapter does not violate the term policy
6. The chapter does not borrow from `adaptation_en`

## Final Actions

- If approved, create the final file in `final/`
- If revision is needed, keep the chapter in `draft/` and record the issue in `review/`
- If the source or draft is incomplete, mark it `hold`
