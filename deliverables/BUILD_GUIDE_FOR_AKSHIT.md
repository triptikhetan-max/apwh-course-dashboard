# Build Guide for Akshit

---

## COURSE 1: Jackson's AP World History Review Course

**Structure:** Princeton PT1 diagnostic (65 MCQs) --> 71 topic modules

### Diagnostic (before the course starts)

- Scrape from Princeton 2024 EPUB at `/Users/tripti/Downloads/World History/`
- Supplementary Qs: `diagnostic_supplement_unit4_5_9.md`
- Scoring per unit: 80%+ = skip, 50-79% = skim, below 50% = full

### Each of the 71 topics has 4 items. Build them in this order:

**1. VIDEO**
- Open `jackson_course/topic_X.X/article.md`
- First line has the YouTube URL
- Embed as iframe, 100% width, 16:9 aspect ratio

**2. ARTICLE**
- Same `article.md` file. Copy these sections in order:
  - Learning Goal
  - Learning Outcomes
  - Student Instructions
  - Article Content
  - Key Terms
  - Note-Taking Prompts
- Key terms as H5P accordion (nice-to-have, not required)
- Note-taking prompts as collapsible sections (nice-to-have)

**3. MCQ PRACTICE (6 questions)**
- 6 stimulus-based MCQs, 4 choices (A-D), all related to the CED topic of that article
- Source priority:
  1. **AP Classroom** — first choice, pull from the topic question bank for that CED topic
  2. **Barron's 2024** — if AP Classroom doesn't have enough, pull from Barron's (EPUB at `/Users/tripti/Downloads/World History/`)
  3. **Princeton 2024** — same location, use if still short

**4. ESSAY (1 prompt)**
- Essay type per topic:
  - **SAQ** — most topics (short answer, 2-3 parts)
  - **LEQ** — every 3rd-4th topic (long essay with thesis)
  - **Mini-DBQ** — once per unit (2-3 docs, thesis + body paragraph)
- Source: AP Classroom topic bank or released AP exam FRQs
- Autograder scores against AP rubric (thesis, evidence, analysis)

### Where to find everything

| What | Path |
|------|------|
| 71 article files | `jackson_course/topic_X.X/article.md` |
| Princeton diagnostic | Princeton EPUB at `/Users/tripti/Downloads/World History/` |
| Diagnostic supplement | `diagnostic_supplement_unit4_5_9.md` |

All paths relative to `/Users/tripti/Downloads/final_pdfs/qc_pipeline/reports/` unless noted.

---

## COURSE 2: HIPP Document Analysis (B2)

**Structure:** 9 modules, each has an item-by-item build spec.

### How to build

1. Open the module spec: `hipp_course/module_X_akshit_build_spec.md`
2. Follow it item by item. Each item tells you:
   - Content type (video / article / MCQ / FRQ)
   - Exact source (which PDF, which page, which document number)
   - Scrape instructions
   - For FRQs: autograder rubric, model answer, feedback text
   - H5P elements tagged where needed (Reveal for model answers, Accordion for hints)
3. Documents to scrape from released AP exams at: `hipp_research/released_ap_docs/frq_sets/`

### Where to find everything

| What | Path |
|------|------|
| Module specs (9 files) | `hipp_course/module_X_akshit_build_spec.md` |
| Practice doc PDFs | `hipp_research/released_ap_docs/frq_sets/` |

---

## STYLING (both courses)

**Video:** YouTube iframe, 100% width, 16:9 aspect ratio

**Article:** max-width 720px, clean readable font, bold key terms on first use

**Callout boxes:** light blue background for "College Board wants you to know" tips

**MCQ:** stimulus card above, radio buttons below, show per-choice feedback after submit

**FRQ:** text area, submit button, autograder feedback + model answer reveal after submit

---

## Start here

1. Build Topic 1.1 + HIPP Module 2
2. Show Tripti for review
3. Then batch the rest

**Don't improvise on content. If something is unclear, ask Tripti.**
