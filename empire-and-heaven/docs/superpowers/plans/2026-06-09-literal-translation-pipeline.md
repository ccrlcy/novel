# Literal Translation Pipeline Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Create a separate literal translation production path and begin translating the novel without mixing it into the adaptation workflow.

**Architecture:** The Korean chapter files remain the only authoritative content source. A dedicated literal pipeline stores planning manifests, segment work units, draft chapters, final chapters, review notes, and harness rules under a separate directory tree.

**Tech Stack:** Markdown files, repository file structure, Codex sub-agents, harness review documents

---

### Task 1: Create literal pipeline structure and rules

**Files:**
- Create: `translation_en_literal/README.md`
- Create: `translation_en_literal/harness/literal_translation_rules.md`
- Create: `translation_en_literal/harness/chapter_completion_checklist.md`
- Create: `translation_en_literal/harness/agent_workflow.md`

- [ ] Define the literal path and rules
- [ ] Define chapter completion checks
- [ ] Define agent responsibilities

### Task 2: Create chapter inventory and segmentation manifest

**Files:**
- Create: `translation_en_literal/planning/chapter_manifest.md`

- [ ] Inventory all chapters
- [ ] Assign canonical output filenames
- [ ] Assign per-chapter segment counts

### Task 3: Create reusable empty production directories

**Files:**
- Create: `translation_en_literal/segments/.gitkeep`
- Create: `translation_en_literal/draft/.gitkeep`
- Create: `translation_en_literal/final/.gitkeep`
- Create: `translation_en_literal/review/.gitkeep`

- [ ] Create empty working directories

### Task 4: Produce first literal chapter draft

**Files:**
- Create: `translation_en_literal/draft/v1_ch01.en.literal.md`
- Create: `translation_en_literal/review/v1_ch01.review.md`

- [ ] Translate Chapter 1 without compression
- [ ] Add review note for unresolved terminology or continuity risks

### Task 5: Verify outputs and prepare next batch

**Files:**
- Modify: `translation_en_literal/planning/chapter_manifest.md`

- [ ] Mark Chapter 1 state accurately
- [ ] Confirm the next queued chapters
