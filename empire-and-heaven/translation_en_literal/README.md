# Empire and Heaven Literal Translation Program

This directory contains the direct English translation workflow for `제국과 천국`.

## Standard

- Translate the full book
- Do not mix this path with `adaptation_en`
- Preserve all material content from `chapters/*.md`
- Allow natural English phrasing
- Do not summarize, reduce, or reframe scenes
- Keep American Christian readability without flattening theology or history

## Directory Map

- `planning/`: chapter inventory, queue, and segmentation decisions
- `segments/`: optional segment work units for chapter-internal translation passes
- `draft/`: merged literal chapter drafts
- `final/`: reviewer-cleared literal chapter files
- `review/`: chapter review notes and issue lists
- `harness/`: rules, workflow, and completion gates

## Review Stage

The review stage is separate from translation.

- Drafts stay in `draft/`
- Review notes stay in `review/`
- Promotion happens only after the review note and manifest status agree
- `final/` is reserved for chapters that pass the review gate

## File Naming

- Draft chapter: `v1_ch01.en.literal.md`
- Final chapter: `v1_ch01.en.literal.final.md`
- Review note: `v1_ch01.review.md`
- Segment file if needed later: `v1_ch01_s01.ko.md` or `v1_ch01_s01.en.md`

## Source Priority

1. `chapters/*.md`
2. `glossary/*.md`
3. `styleguide/*.md`

`adaptation_en` may be consulted for naming continuity, but it is never the source of truth for literal content.

## Review Harness

- `harness/review_standards.md`
- `harness/review_workflow.md`
- `harness/review_checklist.md`
- `harness/final_gate.md`
