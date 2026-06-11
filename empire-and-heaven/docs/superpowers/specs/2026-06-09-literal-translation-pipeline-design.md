# Empire and Heaven Literal Translation Pipeline Design

Date: 2026-06-09

## Goal

Build a separate English production path for a full direct translation of `제국과 천국` that preserves all material content while still reading naturally for American Christian readers.

## Why A Separate Path

The repository already contains `adaptation_en`, which mixes literal transfer and literary adaptation. That path is not a safe place for a no-omission translation program. The literal program therefore needs its own directories, its own review harness, and its own completion rules.

## Source Of Truth

- Primary source: `chapters/*.md`
- Secondary reference only: `glossary/*.md`, `styleguide/*.md`
- Not authoritative for content: `adaptation_en/**/*`

## Translation Standard

- No scene deletion
- No exposition compression
- No event reordering
- No theology dilution
- No character motive simplification
- Natural English phrasing is allowed
- American Christian readability is required
- Historical and biblical gravity should remain intact

## Delivery Structure

Literal work is stored under `translation_en_literal/` with dedicated planning, segment, draft, final, review, and harness subdirectories.

## Operating Model

- Coordinator: owns chapter queue, state, and final merge approval
- Planner: divides each chapter at paragraph boundaries into manageable segments
- Translator: produces direct English translation by segment
- Reviewer: checks omission, compression, theological drift, and continuity

## Segmentation Rule

Chapters stay the primary production unit. Segments only exist inside a chapter and are used to keep each translation pass small enough to execute reliably. Segment boundaries must follow paragraph boundaries and should avoid cutting through a continuous speech, a scene pivot, or a historical explanation block that must remain together.

## Completion Gate

A chapter is complete only when:

1. Every planned segment has a draft
2. The merged chapter is checked against the Korean source
3. No material omission is found
4. Reviewer notes are resolved or explicitly deferred
5. Final file is promoted from `draft/` to `final/`

## Initial Execution Scope

Set up the full pipeline and start live production with Volume I Chapter 1.
