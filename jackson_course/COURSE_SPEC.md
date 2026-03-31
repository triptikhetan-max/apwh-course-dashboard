# Jackson's AP World History Review — Course Spec

## What This Is
A full AP World History review course (71 CED topics across 9 units) designed for Jackson Price. Personalized path based on Princeton PT1 diagnostic results.

## Course Structure
1. **Diagnostic:** Princeton Practice Test 1 (55 MCQs + 10 supplementary)
   - Source: Princeton 2024 EPUB + diagnostic_supplement_unit4_5_9.md
   - Scoring per unit: 80%+ = SKIP unit, 50-79% = SKIM (video + article only), below 50% = FULL (video + article + MCQ + essay)
2. **Per topic (71 total):** Video → Article → MCQ Practice (6)
3. **FRQs (27 total):** Placed after groups of 2-3 related topics, NOT per-topic. See `FRQ_PLACEMENT_MAP.md` for exact placements.
   - 14 SAQs, 8 LEQs, 5 Mini-DBQs
   - First time each type appears, a Heimler strategy video is shown before it
   - 23 sourced from released College Board FRQs, 4 from Barron's 2024

## Unit Overview
| Unit | Topics | CED Period | Exam Weight |
|------|--------|------------|-------------|
| 1 | 1.1-1.7 (7 topics) | 1200-1450 | 8-10% |
| 2 | 2.1-2.7 (7 topics) | 1200-1450 | 8-10% |
| 3 | 3.1-3.4 (4 topics) | 1450-1750 | 12-15% |
| 4 | 4.1-4.8 (8 topics) | 1450-1750 | 12-15% |
| 5 | 5.1-5.10 (10 topics) | 1750-1900 | 12-15% |
| 6 | 6.1-6.8 (8 topics) | 1750-1900 | 12-15% |
| 7 | 7.1-7.9 (9 topics) | 1900-present | 8-10% |
| 8 | 8.1-8.9 (9 topics) | 1900-present | 8-10% |
| 9 | 9.1-9.9 (9 topics) | 1900-present | 8-10% |

## Folder Structure
Each unit has its own folder. Each topic has:
- article.md — the content (video URL, article text, key terms, note prompts)
- topic_spec.md — build instructions (how to embed, what MCQs to source, FRQ if applicable)

Top-level files:
- COURSE_SPEC.md — this file (course overview)
- FRQ_PLACEMENT_MAP.md — where each FRQ goes, what it covers, exact source
- GCHAT_MESSAGE_FOR_AKSHIT.md — handoff message

## MCQ Sourcing Priority
1. AP Classroom topic question bank
2. Barron's AP World History 2024
3. Princeton Review AP World History 2024

## FRQ Structure
- **27 FRQs** placed after groups of 2-3 related topics (not per-topic)
- **14 SAQs** (3 pts each), **8 LEQs** (6 pts each), **5 Mini-DBQs** (4 pts each)
- Full placement details: `FRQ_PLACEMENT_MAP.md`
- **Strategy videos** (Heimler) before first SAQ, first LEQ, first DBQ
- Each topic_spec.md says whether an FRQ goes after that topic or not

## Styling
- Video: YouTube iframe, 100% width, 16:9
- Article: max-width 720px, clean font, bold key terms
- Callout boxes: light blue for "College Board wants you to know"
- MCQ: stimulus card + radio buttons + per-choice feedback
- FRQ: text area + autograder + model answer reveal
- H5P (nice-to-have): accordion for key terms, flashcards for review

## Build Priority
1. Diagnostic (Princeton PT1)
2. Unit 1 (topics 1.1-1.7) — build and show Tripti for review
3. Then batch remaining units

## DRI
- **Content/Design:** Tripti (all content decisions go through her)
- **Engineering:** Akshit (builds on Timeback, scrapes questions, sets up autograder)

## Questions?
Ask Tripti. Don't improvise on content.
