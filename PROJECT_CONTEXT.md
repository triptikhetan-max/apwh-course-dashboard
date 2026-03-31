# AP World History Course Build — Project Context

## What This Project Is
Building two courses for AP World History students at Alpha Schools on the Timeback LMS platform. Exam date: May 7, 2026.

**Course 1: Jackson's AP World History Review** (71 CED topics, all 9 units)
**Course 2: HIPP Document Analysis (B2)** (9 modules, source analysis skills)

## Who's Who
- **Tripti** — SME, instructional designer, content DRI. All content decisions go through her.
- **Akshit** — Engineer. Builds on Timeback, scrapes questions, sets up autograder. Executes the spec.
- **Eric/Hari** — Leadership. Need student assignment briefs and course status updates.
- **Soham** — QA. Validates post-build.

## Students
| Student | AP Score | Primary Problem | Intervention |
|---------|----------|----------------|--------------|
| Jackson Price | 3 | 17 weak topics, Unit MCQs below 50% on 7/9 units | Full review course (all 71 topics with diagnostic) |
| Emma Cotner | 2 | Skill 2 at 0% (can't source documents), Unit 8 = 0% | B2 HIPP course + targeted units |
| Saeed Tarawneh | 2 | Skill 3 at 49% (knows content, can't apply to sources), -22% drop | B2 HIPP course + minimal content |
| Ella Dietz | 3 | Skill 5 at 43% (can't make connections across periods) | Skill 5 intervention (separate spec) |

## Course 1: Jackson's Review — STATUS: READY FOR AKSHIT
Location: `/jackson_course/`

### Structure
1. **Diagnostic:** Princeton PT1 (55 MCQs + 10 supplementary) → scores per unit → skip/skim/full
2. **Per topic (71 total):** Video + Article (one node) → 6 MCQs
3. **27 FRQs** placed after groups of 2-3 related topics (not per-topic)
   - 14 SAQs, 8 LEQs, 5 Mini-DBQs
   - First time each type appears, Heimler strategy video shown before it
   - 23 from released College Board FRQs, 4 from Barron's 2024

### Per Topic Node on Timeback
- Embedded YouTube video (Heimler's History) at top
- Article content directly below (video + article = one node, not separate pages)
- Article has: learning goal, content with bolded key terms, note-taking prompts, key terms list
- Then 6 MCQs (stimulus-based, 4 choices)
- Source MCQs from: AP Classroom first, Barron's/Princeton as backup

### Key Files
| File | What It Is |
|------|-----------|
| `COURSE_SPEC.md` | Master spec — read first |
| `FRQ_PLACEMENT_MAP.md` | 27 FRQs — where, what type, exact source |
| `GCHAT_MESSAGE_FOR_AKSHIT.md` | Handoff message |
| `diagnostic_test_mapping.md` | Princeton PT1 answer key + unit mapping |
| `diagnostic_supplement_unit4_5_9.md` | 10 extra Qs for Units 4, 5, 9 |
| `unit_X/topic_X.X/article.md` | Article content for each topic |
| `unit_X/topic_X.X/topic_spec.md` | Build instructions per topic |
| `released_ap_docs/` | 22 PDFs (11 FRQ sets + 11 scoring guidelines, 2017-2025) |

### What's Done
- [x] 71 articles generated with Opus, QC'd, all fixes applied
- [x] All Heimler video URLs populated
- [x] 27 FRQs mapped with exact sources
- [x] 3 strategy videos (SAQ, LEQ, DBQ) placed at first occurrence
- [x] Princeton diagnostic + 10 supplementary Qs
- [x] Folder organized for Akshit handoff

### What's Pending
- [ ] Akshit builds on Timeback
- [ ] Tripti reviews Unit 1 build before batching rest
- [ ] Emma/Saeed/Ella courses (after Jackson's is validated)

---

## Course 2: HIPP (B2) — STATUS: SPECS DONE, NOT YET HANDED OFF
Location: `/hipp_course/`

### Structure
9 modules, scaffolded Me-We-You progression:

| Module | Focus | Items | Docs Used |
|--------|-------|-------|-----------|
| 1 | What is HIPP? (intro) | 10 | 2 worked examples |
| 2 | Historical Situation | 16 | 5 practice docs |
| 3 | Purpose | 16 | 5 practice docs |
| 4 | Intended Audience | 16 | 5 practice docs |
| 5 | Point of View (hardest) | 17 | 5 practice docs (extra scaffolding) |
| 6 | Full HIPP — Guided | 8 | 5 docs, per-element scoring |
| 7 | Full HIPP — Independent | 8 | 5 docs, no scaffolding |
| 8 | HIPP → DBQ Connection | 6 | Mini-DBQs (3 + 4 docs) |
| 9 | Full DBQ Practice | 5 | Full 7-doc DBQ (2024 Set 1) |

### Key Design Decisions
- **Videos:** Heimler "Three Secrets to a Perfect DBQ" for Modules 1 and 8-9. Modules 2-5 are article-driven (no per-element video — article IS the teaching).
- **Scaffolding:** Guided → Semi-guided → Independent within each module
- **Autograder:** AI/LLM-based, scores each HIPP element separately (H: ✅/❌, I: ✅/❌, P: ✅/❌, POV: ✅/❌)
- **Model answers:** Shown after submission via H5P Reveal
- **Historical context hints:** Provided with each practice document
- **Self-check checklist:** Before each submission
- **No document reused across modules**
- **H5P elements:** Reveal (model answers), Accordion (hints), Fill-in-blanks (sentence frames) — REQUIRED, not nice-to-have

### Key Files
| File | What It Is |
|------|-----------|
| `module_X_akshit_build_spec.md` | Item-by-item build spec per module |
| `module_2_historical_situation.md` | Full article content for Module 2 (prototype) |

### What's Done
- [x] All 9 module specs written (item-by-item, autograder rubrics, model answers)
- [x] 77 released DBQ documents cataloged
- [x] Module 2 prototype article written and dry-tested (7.5/10)
- [x] 3 fixes identified and applied (answer keys, context hints, self-check)

### What's Pending
- [ ] Write article content for Modules 1, 3-9 (Module 2 is the template)
- [ ] Tripti reviews HIPP specs before handoff to Akshit
- [ ] Akshit builds on Timeback

---

## Research Library
Location: `/research/`

### HIPP Research (3 files)
| File | Content |
|------|---------|
| `hipp/01_reddit_forums_student_teacher.md` | 655 lines — student struggles, teacher strategies, sentence frames, what 5-scorers do |
| `hipp/02_video_article_inventory.md` | 13 sections — Heimler, Fiveable, Khan Academy, Tom Richey, CrashCourse, free worksheets |
| `hipp/03_pedagogy_methods.md` | 570 lines — Wineburg, SHEG, DBQ Project, cognitive science, Chief Reader Reports |

### FRQ Pattern Analysis
- `frq_pattern_analysis.md` — All released FRQs 2017-2025, China/Russia frequency, theme patterns, time period distribution

---

## Student Data
Location: `/student_data/`
- `ap_world_history_s3_review.md` — Full S3 review with per-student analysis (CED skills, weak topics, FRQ feedback, intervention plans)
- Source CSV: `/Users/tripti/Downloads/Alpha_Work/AP_Reviews/S3_AP_Review_Project/01_source_data/ap_course_progress_item_level_for_tripti.csv`

---

## Source Data
Location: `/source_data/`
- `ced/` — 71 CED topic files + enriched JSON (learning objectives, essential knowledge, illustrative examples)
- `video/` — 7 Unit 1 transcripts + `all_units_video_map.md` (64 Heimler URLs)
- `external/` — Khan Academy + Fiveable URLs per topic
- `base_course/` — WORH23-v1 base course articles

### External Sources (not in this folder)
- Barron's 2024 EPUB: `/Users/tripri/Downloads/World History/John McCannon - AP World History...epub`
- Princeton 2024 EPUB: `/Users/tripti/Downloads/World History/The Princeton Review - Princeton Review AP World History...epub`
- AP Classroom: Login required — Akshit has access

---

## Key Decisions Made (DO NOT CHANGE WITHOUT TRIPTI)

1. **No topic-level diagnostic.** Princeton PT1 at unit level for Jackson. Other students get assigned units directly from S3 data.
2. **Video + Article = one node** on Timeback. Not separate pages.
3. **6 MCQs per topic.** Source from AP Classroom first, then Barron's/Princeton.
4. **FRQs club multiple topics** (27 total, not 71). Placed at natural breakpoints.
5. **First time each FRQ type appears, show Heimler strategy video** before it.
6. **5-choice questions = DELETE entirely.** Do not convert to 4 choices.
7. **HIPP modules are article-driven** for elements (Modules 2-5). No per-element videos.
8. **H5P elements are REQUIRED** for HIPP course (Reveal, Accordion, Fill-in-blanks). Nice-to-have for Jackson course.
9. **Autograder is AI/LLM-based.** Scores against rubrics with element-specific feedback.
10. **Note-taking prompts based on CED EK statements.** Not generic.
11. **Key terms list in every article.**
12. **Content decisions are Tripti's.** Akshit executes, does not improvise.

---

## How to Continue This Project

1. Open Claude Code in `/Users/tripti/Projects/apwh-course-build/`
2. This PROJECT_CONTEXT.md gives full context
3. Key next steps:
   - Jackson course: Akshit builds Unit 1, Tripti reviews, then batch rest
   - HIPP course: Tripti reviews specs, then handoff to Akshit
   - Other students: Build targeted courses after Jackson's is validated
   - Email draft for Eric/Hari: Course status + student assignments
