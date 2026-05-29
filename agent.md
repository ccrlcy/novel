# Empire and Heaven Translation Agent Notes

## Current Mission

Translate the Korean novel `Empire and Heaven` into English as a faithful literary translation.

This is not an adaptation, rewrite, modernization, summary, or retelling project.

## Non-Negotiable Rules

1. Never add content not present in the source text.
2. Never remove content from the source text.
3. Never summarize.
4. Never paraphrase entire scenes.
5. Never invent dialogue.
6. Never invent emotions.
7. Never invent transitions.
8. Never infer missing chapters.
9. Never continue from assumptions.
10. If source is unavailable, stop immediately and report: `Source verification required.`

## Translation Goal

Target style:

- Faithful translation
- Literary English
- NIV readability
- Historical novel tone
- Preserve the author's intent

Priority order:

1. Accuracy
2. Completeness
3. Consistency
4. Readability
5. Style

Style must never override accuracy.

## Repository Paths

Source chapters:

- `empire-and-heaven/chapters`

English final files:

- `empire-and-heaven/adaptation_en/final`

## Completion Definition

A chapter is complete only when all of the following are done:

1. Source chapter identified
2. Translation finished
3. QA passed
4. Git committed
5. Commit hash reported

Without a commit hash, status is not complete.

## Completed Work

### Chapter 1

- Source: `empire-and-heaven/chapters/상_01_스며드는_바람.md`
- Target: `empire-and-heaven/adaptation_en/final/ch01_the_encroaching_wind.en.final.md`
- Commit: `f751a733718a828fdc8f61d3ac57f99efe35ea01`
- Status: COMPLETE

### Chapter 2

- Source: `empire-and-heaven/chapters/상_02_낯선_사람들.md`
- Target: `empire-and-heaven/adaptation_en/final/ch02_strangers.en.final.md`
- Commit: `e3a4af4d5f58016a58b8003f2bc966dd9022fab9`
- Status: COMPLETE

### Chapter 3

- Source: `empire-and-heaven/chapters/상_03_어둠을_헤치고.md`
- Target: `empire-and-heaven/adaptation_en/final/ch03_through_the_darkness.en.final.md`
- Commit: `30309bd5c7a715fff98292ba43f82d79519333fe`
- Status: COMPLETE

### Chapter 4

- Source: `empire-and-heaven/chapters/상_04_얻는_자와_잃은_자.md`
- Target: `empire-and-heaven/adaptation_en/final/ch04_the_one_who_gains_and_the_one_who_loses.en.final.md`
- Commit: `04650e7b1fa6e6a10ad32391a1c848fc1a2354b3`
- Latest file SHA after update: `443b7a425b4fd2f65c210d838182025df1443e`
- Verified file size: `30821`
- Status: COMPLETE

### Chapter 5

- Source: `empire-and-heaven/chapters/상_05_심야의_파수대.md`
- Target: `empire-and-heaven/adaptation_en/final/ch05_the_midnight_watch.en.final.md`
- Commit: `6b281b32d352a74ed7fdfbc8145349103f2ad1d7`
- Latest file SHA after update: `cb1073305056be639135405c89bf3257d2268069`
- Verified file size: `50712`
- Status: COMPLETE

## Next Chapter

Next source chapter:

- `empire-and-heaven/chapters/상_06_잃어버린_좌표.md`

Expected target file:

- `empire-and-heaven/adaptation_en/final/ch06_lost_coordinates.en.final.md`

## Working Notes

- User requested Korean responses.
- User requested minimal usage; keep chat output concise and avoid pasting full translations unless explicitly asked.
- Existing English files may contain adaptation or compression. Replace with faithful translation when source comparison shows mismatch.
- Preserve source oddities or unclear markers rather than inventing missing material.
- Use GitHub contents API for file creation/update when working directly in the repository.
