# Moody Dev v2 Implementation Plan

> **For agentic workers:** REQUIRED: Use superpowers:executing-plans to implement this plan. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Upgrade Moody Dev theme to v2 with Pixel/Lego separators and new informative segments.

**Architecture:** Update `moody-dev.omp.json` by replacing separators, adding new segments to the `blocks` array, and ensuring proper color palette usage.

**Tech Stack:** Oh My Posh (JSON configuration).

---

## Chunk 1: Visual Foundation (Pixel/Lego)

### Task 1: Update Powerline Separators
**Files:**
- Modify: `moody-dev.omp.json`

- [ ] **Step 1: Replace path separator**
  Update `blocks[0].segments[3].powerline_symbol` to `\ue0c6`.
- [ ] **Step 2: Replace git separator**
  Update `blocks[0].segments[4].powerline_symbol` to `\ue0c6`.
- [ ] **Step 3: Update closing text segment**
  Update `blocks[0].segments[5].properties.text` to `\ue0c6`.
- [ ] **Step 4: Verify visually**
  Run: `oh-my-posh debug --config moody-dev.omp.json`
  Expected: Separators show as  (Pixel style).
- [ ] **Step 5: Commit**
  `git add moody-dev.omp.json; git commit -m "feat: update separators to Pixel/Lego style"`

---

## Chunk 2: Language & Environment Expansion

### Task 2: Add Go, Rust, and Java Segments
**Files:**
- Modify: `moody-dev.omp.json`

- [ ] **Step 1: Add Go segment**
  Insert Go segment after Python segment.
- [ ] **Step 2: Add Rust segment**
  Insert Rust segment after Go segment.
- [ ] **Step 3: Add Java segment**
  Insert Java segment after Rust segment.
- [ ] **Step 4: Verify with debug**
  Run: `oh-my-posh debug --config moody-dev.omp.json`
- [ ] **Step 5: Commit**
  `git add moody-dev.omp.json; git commit -m "feat: add Go, Rust, and Java segments"`

---

## Chunk 3: Cloud & Network Segments

### Task 3: Add Azure, GCP, and Network Segments
**Files:**
- Modify: `moody-dev.omp.json`

- [ ] **Step 1: Add Azure segment**
  Insert Azure segment after AWS segment.
- [ ] **Step 2: Add GCP (Google Cloud) segment**
  Insert GCP segment after Azure segment.
- [ ] **Step 3: Add Network segment**
  Insert Network segment before Status segment.
- [ ] **Step 4: Verify with debug**
  Run: `oh-my-posh debug --config moody-dev.omp.json`
- [ ] **Step 5: Commit**
  `git add moody-dev.omp.json; git commit -m "feat: add Azure, GCP, and Network segments"`

---

## Chunk 4: System Information & Final Polish

### Task 4: Add CPU/RAM segments and final layout check
**Files:**
- Modify: `moody-dev.omp.json`

- [ ] **Step 1: Add CPU segment**
  Insert CPU segment after Network segment.
- [ ] **Step 2: Add RAM segment**
  Insert RAM segment after CPU segment.
- [ ] **Step 3: Final layout adjustment**
  Ensure all segments have consistent spacing and proper color palette references.
- [ ] **Step 4: Final verification**
  Run: `oh-my-posh debug --config moody-dev.omp.json`
- [ ] **Step 5: Commit**
  `git add moody-dev.omp.json; git commit -m "feat: add CPU/RAM segments and finalize v2 layout"`
