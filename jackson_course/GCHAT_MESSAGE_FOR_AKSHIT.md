Hey Akshit — Jackson's AP World History Review course is ready to build.

**What it is:** A full 71-topic AP World History review course personalized for Jackson. He takes a diagnostic first, and based on how he scores per unit, he either skips, skims, or does the full module for each topic.

**Course structure:**
1. Princeton PT1 diagnostic (65 MCQs) → scores per unit → determines his path
2. 71 topic modules across 9 units. Each topic has: Video → Article → 6 MCQs
3. 27 FRQs placed after groups of related topics (not per-topic). See `FRQ_PLACEMENT_MAP.md`

**What I'm giving you:**

A folder called `jackson_course/` with everything organized:

```
jackson_course/
├── COURSE_SPEC.md          ← read this first — course overview, styling, build priority
├── FRQ_PLACEMENT_MAP.md    ← where each FRQ goes, what it covers, exact source
├── unit_1/
│   ├── topic_1.1/
│   │   ├── article.md      ← the content (video URL, article text, key terms, prompts)
│   │   └── topic_spec.md   ← build instructions for this topic
│   ├── topic_1.2/
│   │   ├── article.md
│   │   └── topic_spec.md
│   └── ... (7 topics)
├── unit_2/ through unit_9/  ← same structure, 71 topics total
```

**How to build one topic:**
1. Open `topic_spec.md` — it tells you everything
2. Embed the video (YouTube URL is in the spec)
3. Copy the article content from `article.md`
4. Add 6 MCQs — source from AP Classroom first (topic question bank for that CED topic). If not enough, use Barron's or Princeton (chapters listed in the spec)
5. Check `topic_spec.md` Section 4 — if an FRQ goes after this topic, add it. If not, move on.
6. FRQs club 2-3 topics together. Details (type, source, PDF, rubric) are in the topic spec AND in `FRQ_PLACEMENT_MAP.md`
7. First SAQ/LEQ/DBQ in the course has a Heimler strategy video before it — URLs in the topic spec

**Diagnostic:**
- Princeton Practice Test 1 — scrape from Princeton 2024 EPUB
- 10 supplementary Qs in `diagnostic_supplement_unit4_5_9.md`
- Scoring: 80%+ per unit = skip, 50-79% = skim (video + article only), below 50% = full

**Start here:**
1. Build the diagnostic
2. Build Unit 1 (topics 1.1-1.7)
3. Show me for review
4. Then batch the rest

**Content decisions are mine. If something is unclear, ask me — don't improvise.**
