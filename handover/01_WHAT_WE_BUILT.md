# What We Built — Detailed Breakdown

## Course 1: Jackson's AP World History Review

**Location:** `jackson_course/`
**Status:** READY FOR AKSHIT TO BUILD ON TIMEBACK

### Structure
1. **Diagnostic:** Princeton PT1 (55 MCQs + 10 supplementary) → scores per unit → 80%+ SKIP, 50-79% SKIM, below 50% FULL
2. **Per topic (71 total):** Heimler video → article → 6 MCQs (stimulus-based, 4 choices A-D)
3. **27 FRQs** clustered after groups of 2-3 related topics (not per-topic)
   - 14 SAQs, 8 LEQs, 5 Mini-DBQs
   - First time each type appears, Heimler strategy video plays
   - 23 from released CollegeBoard (2017-2025), 4 from Barron's 2024

### Key Files
- `COURSE_SPEC.md` — Master spec (read first)
- `FRQ_PLACEMENT_MAP.md` — 27 FRQs with placement, type, source, PDF path
- `GCHAT_MESSAGE_FOR_AKSHIT.md` — Handoff message
- `diagnostic_test_mapping.md` — Princeton PT1 answer key + unit mapping
- `diagnostic_supplement_unit4_5_9.md` — 10 extra questions
- `unit_X/topic_X.X/article.md` — Article content per topic (71 files)
- `unit_X/topic_X.X/topic_spec.md` — Build instructions per topic (71 files)
- `released_ap_docs/` — 22 PDFs (11 FRQ sets + 11 scoring guidelines, 2017-2025)

### Article Template (every article follows this)
1. Learning Goal (one sentence, CED-aligned)
2. Learning Outcomes (3-5 from CED)
3. Student Instructions (watch video, read article, take notes, ~15 min)
4. Article Content (400-600 words, bold key terms, College Board callout boxes)
5. Key Terms (12-20 with definitions)
6. Note-Taking Prompts (5 prompts, #5 always bridges to next topic)

---

## Course 2: B2 HIPP Document Analysis

**Location:** `hipp_course/`
**Status:** SPECS DONE, NOT YET HANDED OFF

### 9 Modules (Me-We-You Progression)

| Module | Focus | Items | Teaching Method |
|--------|-------|-------|----------------|
| 1 | What is HIPP? (intro) | 10 | Heimler video (0:00-6:25) |
| 2 | Historical Situation | 16 | Article-driven (PROTOTYPE DONE) |
| 3 | Purpose | 16 | Article-driven |
| 4 | Intended Audience | 16 | Article-driven |
| 5 | Point of View (hardest) | 17 | Article-driven + extra scaffolding |
| 6 | Full HIPP — Guided | 8 | Per-element scoring |
| 7 | Full HIPP — Independent | 8 | No scaffolding |
| 8 | HIPP → DBQ Connection | 6 | Mini-DBQs + Heimler (13:10-end) |
| 9 | Full DBQ Practice | 5 | Full 7-doc DBQ (2024 Set 1) |

### Key Design Decisions
- Videos only for Modules 1 and 8-9. Modules 2-5 are article-driven.
- AI/LLM autograder scores each HIPP element separately (H/I/P/POV: pass/fail)
- Model answers via H5P Reveal (REQUIRED, not nice-to-have)
- H5P Fill-in-Blanks for guided practice (Docs 1-2), open response for Docs 3-5
- No document reused across modules. 77 DBQ documents cataloged.

### What's Done vs Pending
- Done: All 9 module specs, Module 2 prototype (7.5/10), 77 DBQ docs cataloged, research (3 files)
- Pending: Article content for Modules 1, 3-9 (Module 2 is the template)

---

## Course 3: MC1 China (Han to Qing) — SCRAPPED

**Course ID:** `s4-r1r3-mc1-a120a364`
**Status:** Built by Akshit, QC failed, rebuild not happening

- 190 MCQ + 3 FRQ built
- QC found: only 72 MCQs (37%) are about China, 93 are wrong-topic
- All 3 FRQs wrong-topic (Mughal, Chile, generic)
- Missing Units 5, 6, 7 entirely
- Fix doc written: `deliverables/apwh_mc1_fixes_for_akshit.md` (~15 hrs rebuild)
- **Decision: Not rebuilding. Built Jackson's course instead.**

---

## Course 4: MC2 Russia (Kievan Rus to Soviet) — SCRAPPED

**Course ID:** `s4-r1r3-mc2-83cb26f8`
**Status:** Built by Akshit, QC failed, rebuild not happening

- 232 MCQ + 3 FRQ built
- QC found: only 83 MCQs (36%) are about Russia, 121 are wrong-topic
- All 3 FRQs generic, 0 about Russia
- Missing Units 1-2, 6. Two quizzes at 0% keepable.
- Fix doc written: `deliverables/apwh_mc2_fixes_for_akshit.md` (~17 hrs rebuild)
- **Decision: Not rebuilding. Built Jackson's course instead.**
