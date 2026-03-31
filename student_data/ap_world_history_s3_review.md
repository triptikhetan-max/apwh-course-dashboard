# AP World History: Modern - S3 Review & AP Practice Exam Analysis

## Data Sources
- **Practice test scores:** `AP Practice Tests - Feb 2026.xlsx` > `Results` sheet (columns: student, course, test, final_mcq_accuracy, final_frq_accuracy, ap_score)
- **FRQ grading & feedback:** `FRQ Grading.xlsx` > `paper_test_frq_grading` sheet (columns: Test Name, Student, Question Number, score, feedback, FRQ_score)
- **Timeback learning data:** `Alpha High School - Mid Term Report Data - Academics Copy.xlsx` > `ap_learning_data` sheet (columns: completion_percent, course_accuracy, tb_course_mcq_accuracy, tb_course_frq_accuracy)
- **SSD accommodations:** same sheet > `approved_ssd_accommodations` column
- **AP course registrations:** same sheet > `course_registered`, `priority` columns
- **Topic-level course progress:** `ap_course_progress_item_level_for_tripti.csv` (columns: student, course_name, unit_title, item_title, test_type, accuracy, totalQuestions, correctQuestions). test_type values: `topic_test`, `unit_mcq_test`, `unit_frq_test`

## 1. Overall S3 Results

### Enrollment
- **Total students registered:** ~14 (across Alpha Austin, Alpha Miami)
- **Students who completed practice exam:** 6
- **Students deferred to Session 4:** Kavin Lingham, Stella Cole (both have Timeback data)
- **Students barely started or not enrolled:** Aoife Huey (not enrolled), Artemis Schiettecatte (2% completion), Liam Lenhardt (not enrolled), Mollie McDougald (2% completion), Ju Orloff (16% completion)
- **Exam date:** May 7, 2026
- **All tested students are Priority 1**
- **Test source:** Barron's; Final exam (paper-based) for all 6 tested students

### Practice Exam Score Distribution (6 students)
- **Score of 5:** 1 student (17%) - Michael Cai
- **Score of 4:** 1 student (17%) - Stella Grams
- **Score of 3:** 2 students (33%) - Ella Dietz, Jackson Price
- **Score of 2:** 2 students (33%) - Emma Cotner, Saeed Tarawneh
- **Score of 1:** 0 students

### Averages (6 tested students)
- **Average MCQ accuracy:** 66.0%
- **Average FRQ accuracy:** 57.8%
- **Average AP Score:** 3.2

---

## 2. Insights

### MCQ vs. FRQ Performance Gap
- FRQ accuracy (57.8%) trails MCQ (66.0%) by ~8 percentage points
- However, the FRQ gap is driven by specific question types (see below)
- MCQ is critically low for Emma (53%) and Saeed (58%) - both need content-level remediation

### FRQ Question-Type Breakdown (all 6 tested students)
| Student | SAQ 1 | SAQ 2 | SAQ 3/4 | DBQ (out of 7) | LEQ (out of 6) | Total FRQ |
|---------|-------|-------|---------|----------------|----------------|-----------|
| Emma Cotner | 2/3 | 1/3 | 2/3 | **1/7** | 2/6 | 43% |
| Saeed Tarawneh | 1/3 | 1/3 | 2/3 | **2/7** | 2/6 | 39% |
| Ella Dietz | 3/3 | 2/3 | 2/3 | **2/7** | 3/6 | 63% |
| Jackson Price | 3/3 | 2/3 | 1/3 | **2/7** | 3/6 | 56% |
| Stella Grams | 1/3 | 2/3 | 2/3 | **5/7** | 3/6 | 58% |
| Michael Cai | - | - | - | - | - | 88% |

**The DBQ is the single biggest weakness:**
- 4 of 5 students who took the Final scored 1-2 out of 7 on the DBQ
- Only Stella Grams earned a respectable 5/7
- The DBQ is worth 25% of the exam score, making this gap critical

### Common DBQ Weaknesses (from FRQ feedback)
1. **Thesis/Claim:** Emma (not earned), Saeed (not earned), Ella (not earned). Students either restate the prompt, make factually inaccurate claims (Emma referenced "Confucian ideals" for the USSR), or fail to identify both continuity AND change
2. **Contextualization:** Emma (not earned), Saeed (not earned), Ella (not earned). Students either provide irrelevant context (Emma: US-USSR Cold War; Saeed: Meiji Restoration) or skip it entirely
3. **Document usage:** Most students used only 3-5 documents when 6-7 are needed for full credit (Saeed used 6+, others used 3-5). Students describe documents rather than using them as evidence for an argument
4. **Sourcing/HIPP:** Almost no students performed HIPP analysis (Historical context, Intended audience, Purpose, Point of view) on documents

### Common LEQ Weaknesses
1. **Thesis construction:** Saeed (not earned - wrote about wrong option, labeled Option 2 but answered Option 3). Emma (not earned - focused on European actions rather than responses of African/American societies)
2. **Comparison skill:** Jackson and Ella showed basic comparison ability but lacked sophistication. Students describe each region separately rather than making integrated comparisons

### Timeback Course Data vs. Practice Test Performance
| Student | TB Completion | TB Accuracy | TB MCQ | TB FRQ | Practice MCQ | Practice FRQ | AP Score |
|---------|-------------|-------------|--------|--------|-------------|-------------|----------|
| Emma Cotner | 93% | 76% | 83% | 74% | 53% | 43% | 2 |
| Saeed Tarawneh | 98% | 80% | 77% | 68% | 58% | 39% | 2 |
| Ella Dietz | 89% | 80% | 86% | 73% | 62% | 63% | 3 |
| Jackson Price | 100% | 54% | 46% | 15% | 78% | 56% | 3 |
| Stella Grams | 89% | 89% | 93% | 85% | 65% | 58% | 4 |
| Michael Cai | 48% | 68% | 65% | 51% | 80% | 88% | 5 |

**Key observations:**
- **Emma Cotner:** 93% completion with 76% accuracy in Timeback, but MCQ dropped from 83% (TB) to 53% (practice). This is one of the largest drops - suggests Timeback questions may not align well with exam-level difficulty, or she memorized answers rather than understanding concepts
- **Saeed Tarawneh:** Nearly identical pattern to Emma - 98% completion, 80% accuracy in TB, but practice test scores dropped significantly. TB FRQ (68%) -> practice FRQ (39%)
- **Jackson Price:** Unusual pattern - 100% completion but only 54% accuracy in Timeback (46% MCQ, 15% FRQ!), yet scored 78% MCQ on practice test. This suggests he may have rushed through Timeback content but learned from the process, OR the practice test happened to cover his stronger areas
- **Michael Cai:** Only 48% Timeback completion but scored 5. Strong natural aptitude or external preparation
- **Stella Grams:** Consistent performer - high TB accuracy (89%) translated to solid practice performance (4)

### Topic-Level Performance Analysis
*[Source: `ap_course_progress_item_level_for_tripti.csv` > AP World History: Modern - PP100]*

The item-level data reveals a critical **recognition-vs-retrieval gap** — topic quiz scores (recognition-based, within-context) diverge sharply from unit MCQ and FRQ scores (retrieval-based, mixed content) for several students:

| Student | Topic Quiz Avg | Unit MCQ Avg | Unit FRQ Avg | Topic→Unit MCQ Gap | Practice MCQ |
|---------|---------------|-------------|-------------|-------------------|-------------|
| Emma Cotner | 73.0% | 82.5% | 74.4% | -9.5 pts* | 53% |
| Saeed Tarawneh | 83.1% | 76.7% | 68.1% | +6.5 pts | 58% |
| Ella Dietz | 80.7% | 85.6% | 72.3% | -5.0 pts* | 62% |
| Jackson Price | 70.0% | **45.6%** | **15.5%** | **+24.4 pts** | 78% |
| Stella Grams | 89.4% | 93.1% | 82.0% | -3.7 pts | 65% |
| Michael Cai | 71.0% | 65.0% | 49.5% | +6.0 pts | 80% |

*Negative gaps for Emma and Ella suggest they performed better on unit MCQs than topic quizzes — this is unusual and may indicate they benefited from reviewing across topics rather than in isolation.

**Jackson Price stands out dramatically:** His topic quiz average (70%) drops to 45.6% on unit MCQs and 15.5% on unit FRQs. This is the most extreme recognition-vs-retrieval gap in the data. Yet his practice test MCQ was 78% — the highest among the underperformers. This paradox suggests he either crammed before the practice test or the Barron's MCQ format happened to favor his strengths. His unit-level data is a better predictor of sustained knowledge than either the topic quizzes or the single practice test.

**Weak topic concentration by student:**
- **Emma Cotner (11 topics below 60%):** Developments in Europe 1200-1450 (51.6%), Exploration Causes/Events (56.9%), East Asia 1200-1450 (55.6%), Unresolved Tensions After WWI (54.8%), Spread of Communism (57.7%), plus KO Dropbox gaps in Units 4, 6, 7, 8
- **Saeed Tarawneh (6 topics below 60%):** Empires: Administration (0%), Technological Innovations 1450-1750 (52.2%), Economy in the Interwar Period (56.8%), The Silk Roads (59.4%), plus KO Dropbox Unit 8 (57.1%)
- **Ella Dietz (2 topics below 60%):** KO Dropbox Unit 3 (0%), World History LEQ (16.7%). Remarkably few weak topics — her content knowledge is solid
- **Jackson Price (17 topics below 60%):** Industrial Revolution Begins (32.4%), Nationalism & Revolutions (47.8%), End of Cold War (47.9%), KO Dropboxes for Units 4/5/7/8/9 all below 50%, Continuity & Change in Globalized World (51.9%), and many more. Widespread gaps across Units 1, 4-9

### Student Trends
- **All tested students are Grade 10** at Alpha Austin campus
- **Honors students struggling:** Saeed (honors, score 2), Jackson (honors, score 3), Ella (honors, score 3)
- **High completion ≠ exam readiness:** Emma (93%) and Saeed (98%) both scored 2 despite near-complete Timeback courses. This aligns with the AP Repair & Revise BrainLift finding that the PP100 prediction model averages 14 points too optimistic.
- **DBQ is the universal weakness:** Even the score-4 student (Stella) only earned 5/7 on the DBQ, while the 4 others scored 1-2/7
- **Jackson Price is an outlier in every direction:** 100% completion, lowest Timeback accuracy (54%), highest practice MCQ (78%), but the worst unit-level FRQ scores (15.5% avg across 14 FRQ tests). His learning is inconsistent and unpredictable.
- **KO Dropbox scores are weak across the board:** Jackson (0% on Units 8, 9), Emma (0% on Unit 4, 50-57% on Units 6-8). KO Dropbox requires students to write in their own words — the weak scores confirm the AP Repair & Revise BrainLift observation that most students are not maintaining their Knowledge Organisers.

---

## 3. Improvements for S4 (Target: All Students Score 5)

### Priority Actions

#### A. DBQ Intensive (ALL students - this is the highest-leverage intervention)
The DBQ is worth 25% of the exam and is where students are losing the most points.

1. **Thesis formula practice:**
   - Teach the CCOT thesis template: "From [start date] to [end date], [topic] experienced continuity in [specific thing] while changing in [specific thing]"
   - Students practice writing thesis statements ONLY (no full essays) for 10 different DBQ prompts
   - Goal: every student can write a defensible thesis in under 3 minutes

2. **Contextualization drill:**
   - For each practice DBQ, students must write a 3-4 sentence contextualization paragraph BEFORE looking at documents
   - Focus on: What was happening in the world during this period? What broader trends led to the situation described in the prompt?
   - Common error to fix: Students provide irrelevant context (e.g., Emma wrote about US-USSR Cold War for a 1917-1953 USSR economy question)

3. **Document usage practice:**
   - Practice the "bucket" method: group documents into 2-3 categories that support different parts of the argument
   - Each body paragraph must reference at least 2 documents with specific quotes or content
   - Goal: use 6-7 documents minimum (students currently use 3-5)

4. **HIPP analysis:**
   - For every document, practice identifying at least one HIPP element
   - Create a HIPP template card students use during practice DBQs
   - Minimum requirement: 1 HIPP analysis per DBQ (for the sourcing point)

#### B. SAQ Precision (Emma, Saeed)
1. **Direct answer practice:** SAQ answers should be 2-3 sentences MAX per part. Practice the format: "[Claim sentence]. [Evidence sentence]. [Connection sentence]."
2. **Historically specific examples:** Both Emma and Saeed lost points for vague answers. Create flashcards with 5 specific examples for each major topic (e.g., negative tech impacts: Luddite movement, Great Smog of London, Bhopal disaster)

#### C. LEQ Structure (Saeed, Emma)
1. **Read the prompt carefully:** Saeed answered the wrong option (labeled Option 2, wrote about Option 3). Practice underlining key terms in prompts before writing
2. **Comparison structure:** Teach the "overlap" approach - don't write about Region A then Region B separately. Each paragraph should compare both regions on a specific theme
3. **Evidence depth:** Students need 2-3 specific examples per region (not just "Columbus" or "colonization")

#### D. MCQ Content Remediation (Emma at 53%, Saeed at 58%)
1. **Identify topic gaps:** Both students' Timeback data suggests decent MCQ in coursework but poor performance under exam conditions. Focus on:
   - Stimulus-based MCQ practice (reading passages, maps, charts in the AP format)
   - Timed practice: 55 MCQs in 55 minutes
2. **Content review:** Focus on Units 5-8 (Revolutions, Industrialization, Global Conflict, Cold War/Decolonization) which are heavily tested on the exam

#### E. Session 4 Students to Monitor
| Student | TB Completion | TB Accuracy | TB MCQ | TB FRQ | Risk Level |
|---------|-------------|-------------|--------|--------|-----------|
| Kavin Lingham | 85% | 73% | 74% | 54% | Medium - low FRQ |
| Stella Cole | 73% | 81% | 86% | 56% | Medium - no FRQs done on practice |
| Ju Orloff | 16% | 90% | 95% | 100% | Low completion but high accuracy |
| Artemis Schiettecatte | 2% | 55% | - | - | High risk - barely started |
| Aoife Huey | 0% | - | - | - | High risk - not enrolled |
| Liam Lenhardt | 0% | - | - | - | High risk - not enrolled |
| Mollie McDougald | 2% | - | - | - | High risk - barely started |

---

## 4. Individual Student Plans

### Emma Cotner (AP Score: 2 | MCQ: 53% | FRQ: 43%)

**SSD Accommodations:** None
**Full AP course load:** P1 AP World History: Modern (93% completion), P2 AP Computer Science A (0% completion), P3 AP Biology (28% completion, 85% accuracy)
*[Source: Mid Term Report > ap_learning_data > approved_ssd_accommodations, course_registered]*

**CED Skill Breakdown (from updated Student Analysis v2, Feb 25):**
| CED Skill | Score | Rating |
|-----------|-------|--------|
| Skill 1: Developments & Processes | 50% (3/6) | WEAK |
| **Skill 2: Sourcing & Situation** | **0% (0/2)** | **CRITICAL** |
| Skill 3: Claims & Evidence in Sources | 49% (18/37) | WEAK |
| Skill 4: Contextualization | 100% (3/3) | STRONG |
| Skill 5: Making Connections | 71% (5/7) | STRONG |
Course-to-exam drop: -20% (72% course → 53% exam).

**Key skill insight:** Emma's **Skill 2 (Sourcing & Situation) at 0%** is the most extreme weakness in the entire AP World cohort. She cannot source or situate documents at all. Combined with Skill 3 (Claims & Evidence) at 49%, she fundamentally cannot work with source-based questions — which make up 37 of 55 MCQ items (67% of the exam). This is a Layer 2 crisis, not just Layer 1.

**Zero-score practice test topics (4):** 8.5 Decolonization After 1900, 8.6 Newly Independent States, 8.7 Global Resistance to Established Order, 9.2 Technological Advances (Disease) — all in Units 8-9.

**Weakest units on practice test:** Unit 8 **0% (0/7) CRITICAL**, Unit 6 44% WEAK, Unit 9 50% WEAK.

**Current state:** Second-lowest score in the cohort. Despite 93% Timeback completion and 76% accuracy, practice test performance dropped dramatically — MCQ fell from 83% (TB) to 53% (practice), and FRQ from 74% (TB) to 43% (practice). The -20% course-to-exam drop is driven by her inability to work with source-based questions (Skills 2+3). Topic-level data shows 73.0% average across 80 topic tests, with 11 topics below 60% concentrated in Units 1, 4, 6, 7, 8. Unit 8 is a complete void on the practice test (0/7).

**Specific weaknesses from FRQ feedback:**
- SAQ 1 (2/3): Earned points for Great Smog of London and telephone examples, but misattributed smog primarily to automobiles instead of coal burning
- SAQ 2 (1/3): Earned Part A (religious fragmentation) but gave "borders of Holy Roman Empire" as a continuity in religious practice — that's political, not religious
- SAQ 3/4 (2/3): Earned similarity and difference for women's roles but used anachronistic terms ("not allowed to vote" for 1200-1450 period)
- **DBQ (1/7):** Referenced "Confucian ideals" for the USSR (fundamentally wrong), no defensible thesis, irrelevant contextualization (US-USSR Cold War for 1917-1953 economic question), minimal document usage
- LEQ (2/6): No thesis earned. Focused on European actions instead of African/American responses

#### Layer 1: Core Knowledge Gaps
*[Source: `ap_course_progress_item_level_for_tripti.csv`]*

Emma's 11 weak topics reveal gaps across multiple periods:
- **Unit 1 (The Global Tapestry):** Developments in Europe 1200-1450 (51.6%), East Asia 1200-1450 (55.6%)
- **Unit 4 (Transoceanic Interconnections):** Exploration Causes/Events (56.9%), KO Dropbox (0% — 0/11)
- **Unit 6 (Consequences of Industrialization):** KO Dropbox (50% — 4/8)
- **Unit 7 (Global Conflict):** Unresolved Tensions After WWI (54.8%), KO Dropbox (55.6%)
- **Unit 8 (Cold War/Decolonization):** Spread of Communism (57.7%), KO Dropbox (57.1%)
- **Unit 9 (Globalization):** Calls for Reform (0% — 0/1)

Her KO Dropbox scores (0-57% across Units 4, 6, 7, 8) confirm she is not encoding knowledge in her own words. Her strong areas (Columbian Exchange 100%, Newly Independent States 100%, Unit 5 KO 100%) show she *can* learn when she engages deeply.

Unit MCQ tests tell a different story: 95% on Unit 4, 90% on Unit 5, 80% on Units 3/7 — but she has not completed Unit MCQs for Units 1, 8, or 9. The high unit MCQ scores alongside low topic-level scores suggests she may be benefiting from repeated exposure rather than initial mastery.

**Layer 1 actions:**
1. Complete KO Dropbox entries for Units 4, 6, 7, 8 — these are the gaps where she hasn't encoded knowledge in her own words
2. Targeted retrieval on 11 weak topics: flashcard-based recall of key facts for each, then re-test
3. **Regional/civilization fundamentals:** The "Confucian ideals" for USSR error reveals a basic confusion about civilizations. Create and quiz on a one-page reference sheet per major civilization/region (Russia/USSR, China, Ottoman, Western Europe)

#### Layer 2: Disciplinary Moves
**CED skill data confirms Layer 2 is Emma's central crisis:** Skill 2 (Sourcing & Situation) at 0% and Skill 3 (Claims & Evidence) at 49% mean she cannot work with source-based questions in any form — FRQ or MCQ. Her strong Skill 4 (Contextualization, 100%) and Skill 5 (Making Connections, 71%) show she CAN think historically when questions don't require source analysis.

Emma's FRQ feedback reveals the same pattern from a different angle — multiple analytical skill gaps:
- **Conflates political and religious concepts** (SAQ 2: "borders of Holy Roman Empire" as religious practice)
- **Applies anachronistic frameworks** (SAQ 3/4: "not allowed to vote" in 1200-1450)
- **Cannot distinguish between European actions and indigenous responses** (LEQ: focused on colonizers rather than colonized)
- **Cross-civilization confusion** (DBQ: Confucian ideals applied to USSR)

**Layer 2 actions:**
1. **Source analysis fundamentals (Skill 2 — 0%, CRITICAL):** Emma needs to learn how to source documents from scratch. Drill the HIPP framework: Historical context, Intended audience, Purpose, Point of view. Practice on 3 documents per day — just identifying sourcing elements, not answering questions yet
2. **Claims & Evidence practice (Skill 3 — 49%, WEAK):** For each practice passage, write one claim that the evidence supports. Her 49% means she gets roughly half of source-based MCQs wrong — the single biggest area for improvement
3. Practice categorizing evidence as political, economic, social, or religious — quiz with 20 examples
4. Practice the "response" frame: for any prompt about how people responded to X, explicitly list actions taken BY the group in question, not actions done TO them
5. Precision vocabulary: create and drill "commonly confused" pairs (political vs. religious change, continuity vs. change, cause vs. effect, indigenous vs. colonial actions)

#### Layer 3: Exam Technique
Emma's extended writing is critically weak — DBQ 1/7, LEQ 2/6. Both lack defensible theses.
- **DBQ:** No thesis, irrelevant contextualization, minimal document usage (2-3 instead of 6-7), no HIPP
- **LEQ:** No thesis, answered the wrong frame (European actions vs. African/American responses)

**Layer 3 actions:**
1. **DBQ bootcamp (scaffolded):** Week 1: Given thesis + documents, write body paragraphs. Week 2: Given documents, write thesis + body. Week 3: Full timed DBQ
2. **Thesis writing daily practice:** Write one thesis per day. Must include both continuity AND change, or both comparison elements
3. **Contextualization drill:** For each practice DBQ, write 3-4 sentences about what was happening in the world during the period BEFORE looking at documents
4. **MCQ timed drills:** 20 stimulus-based MCQs, 3x per week. Target: 70%+

**Target:** Score 3+ on next practice test. DBQ from 1/7 to 3/7. MCQ from 53% to 65%+.

---

### Saeed Tarawneh (AP Score: 2 | MCQ: 58% | FRQ: 39%)

**SSD Accommodations:** None
**Full AP course load:** P1 AP World History: Modern (98% completion), P2 AP Psychology (12% completion, 95% accuracy), P3 AP Biology (0% completion, not started)
*[Source: Mid Term Report > ap_learning_data > approved_ssd_accommodations, course_registered]*

**CED Skill Breakdown (from updated Student Analysis v2, Feb 25):**
| CED Skill | Score | Rating |
|-----------|-------|--------|
| Skill 1: Developments & Processes | 83% (5/6) | STRONG |
| Skill 2: Sourcing & Situation | 50% (1/2) | WEAK |
| **Skill 3: Claims & Evidence in Sources** | **49% (18/37)** | **WEAK** |
| Skill 4: Contextualization | 100% (3/3) | STRONG |
| Skill 5: Making Connections | 71% (5/7) | STRONG |
Course-to-exam drop: **-22%** (80% course → 58% exam) — the BIGGEST drop in the AP World cohort.

**Key skill insight:** Saeed **knows the content** (Skill 1 at 83% STRONG) but **cannot apply it to source-based questions** (Skill 3 at 49% WEAK). This is a textbook recognition-vs-retrieval gap — his -22% course-to-exam drop is the largest in the cohort, and the CED data confirms it's driven by source analysis weakness, not content gaps.

**Zero-score practice test topics (5):** 4.3 Columbian Exchange, 4.4 Maritime Empires Established, 6.1 Rationales for Imperialism, 8.6 Newly Independent States, 9.2 Technological Advances (Disease) — scattered across Units 4, 6, 8, 9.

**Weakest units on practice test:** Unit 8 29% CRITICAL, Unit 1 33% WEAK, Unit 6 33% WEAK.

**Current state:** Lowest FRQ score in the cohort (39%). Despite 98% completion and 80% TB accuracy, practice performance dropped sharply — MCQ from 77% (TB) to 58%, FRQ from 68% (TB) to 39%. The -22% course-to-exam drop is now explained by CED skill data: Skill 3 (Claims & Evidence) at 49% means he gets roughly half of source-based MCQs wrong. Topic-level data shows 83.1% average across 80 topic tests with only 6 topics below 60%, confirming this is primarily a Layer 2 problem, not Layer 1.

**Specific weaknesses from FRQ feedback:**
- SAQ 1 (1/3): Too vague — did not name a specific technology or event for inequality claim
- SAQ 2 (1/3): Correctly identified Protestant Reformation but called religion a "tool for rebellion" — that's political, not religious practice
- SAQ 3/4 (2/3): Called the UN an NGO (it's an IGO). Focused on why organizations were created rather than their different impacts
- **DBQ (2/7):** No thesis (identified themes but didn't state continuity AND change). No contextualization (referenced Meiji Restoration and Cold War/USSR collapse — irrelevant to 1917-1953 Soviet economy). Weak document usage
- **LEQ (2/6):** Answered the wrong option (labeled Option 2 but wrote about Option 3). Conflated British colonial settler grievances with indigenous American responses

#### Layer 1: Core Knowledge Gaps
*[Source: `ap_course_progress_item_level_for_tripti.csv`]*

Saeed's topic-level data (83.1% average) is the strongest among the 4 underperforming students. Only 6 topics are below 60%:
- **Unit 3 (Land Based Empires):** Empires: Administration (0% — 0/1, likely incomplete)
- **Unit 4 (Transoceanic Interconnections):** Technological Innovations 1450-1750 (52.2%)
- **Unit 7 (Global Conflict):** Economy in the Interwar Period (56.8%)
- **Unit 2 (Networks of Exchange):** The Silk Roads (59.4%)
- **Unit 8:** KO Dropbox (57.1%)
- **Unit 1:** World History LEQ (50.0%)

His strong areas are extensive: 13 topics at 100% (East Asia, Mongol Empire, Nationalism, Industrialization Spreads, Rationales for Imperialism, multiple Unit 8-9 topics). His content knowledge foundation is solid.

Unit MCQ tests show consistent 65-85% across all 9 units, with the weakest being Unit 9 (60%) and Unit 5 (65%). No catastrophic gaps.

Unit FRQ tests reveal the real problem: Saeed scored 0% on Unit 5 LEQ, 0% on Unit 5 SAQ, 28.6% on Unit 4 DBQ, 33.3% on Unit 1 SAQ, and 40% on Unit 7 LEQ. His FRQ performance declines as the course progresses from structured (Unit 1-3) to analytical (Unit 5-9).

**Layer 1 actions:**
1. Targeted review of 4 genuinely weak topics: Technological Innovations 1450-1750, Economy in the Interwar Period, The Silk Roads, Empires Administration
2. Complete KO Dropbox Unit 8 properly — needs to encode Cold War/Decolonization knowledge in own words
3. Layer 1 is NOT Saeed's primary problem — he knows the content. Move quickly to Layers 2 and 3.

#### Layer 2: Disciplinary Moves
**CED skill data confirms Layer 2 is Saeed's central problem:** Skill 3 (Claims & Evidence) at 49% means he loses points on the majority of source-based MCQs (37 of 55 questions). His strong Skill 1 (83%) and weak Skill 3 (49%) create the classic "knows the content, can't work with sources" profile — exactly what his -22% course-to-exam drop predicted.

Saeed's FRQ feedback reveals a clear pattern: **he conflates related but distinct concepts and misreads what prompts are asking for.**
- **Political vs. religious:** religion as "tool for rebellion" is a political analysis, not religious practice
- **Cause vs. impact:** described why organizations were created instead of their different impacts
- **NGO vs. IGO:** factual precision error (UN is an IGO)
- **Wrong essay option:** labeled Option 2 but answered Option 3 — not reading prompts carefully
- **Irrelevant contextualization:** Meiji Restoration and Cold War collapse for a 1917-1953 question — cannot match context to time period

**Layer 2 actions:**
1. **Prompt-reading protocol (Immediate):** Before ANY response: underline key terms, write "The question is asking me to...", confirm option number for LEQ. Practice on 10 past prompts (just reading and restating, no writing)
2. **Precision vocabulary chart:** Create and quiz on commonly confused pairs — NGO vs. IGO, political vs. religious, cause vs. effect, continuity vs. change, creator vs. impact
3. **Historically specific examples bank:** For each AP World unit, list 5 specific, named examples with dates. Practice using in SAQ format. His current vagueness (e.g., "technology causing inequality" without naming anything) must be replaced with precision
4. **Period-matching drill:** Given a date range, list 3 relevant contextual events. This directly addresses his contextualization errors (citing events outside the prompt's time period)

#### Layer 3: Exam Technique
Saeed's DBQ (2/7) and LEQ (2/6) show he cannot construct exam-ready extended responses despite having content knowledge.
- **DBQ:** No thesis formula, no contextualization method, documents not grouped into argument structure
- **LEQ:** Wrong option selected, no defensible thesis even when writing about content he knows
- **SAQs:** Vague answers that don't earn points because they lack specific evidence

**Layer 3 actions:**
1. **DBQ structured practice (scaffolded):** Week 1: thesis + contextualization only. Week 2: add document grouping. Week 3: full timed DBQ
2. **SAQ precision drill:** Practice the format: [Claim sentence]. [Specific evidence with name/date]. [Connection to question]. 5 SAQs per week
3. **MCQ content review:** Focus on Units 5 and 9 (lowest unit MCQ scores: 65% and 60%). Stimulus-based timed practice
4. **Cross-subject note:** AP World exam is May 7, AP Psychology is May 12. Saeed should focus heavily on World History first, then pivot to Psych after May 7. His 95% accuracy in the little Psych he's done suggests he can learn it quickly.

**Target:** Score 3+ on next practice test. DBQ from 2/7 to 4/7. FRQ overall from 39% to 55%+.

---

### Ella Dietz (AP Score: 3 | MCQ: 62% | FRQ: 63%)

**SSD Accommodations:** None
**Full AP course load:** P1 AP World History: Modern (89% completion), P2 AP Chemistry (0% completion, not started)
*[Source: Mid Term Report > ap_learning_data > approved_ssd_accommodations, course_registered]*

**CED Skill Breakdown (from updated Student Analysis v2, Feb 25):**
| CED Skill | Score | Rating |
|-----------|-------|--------|
| **Skill 1: Developments & Processes** | **50% (3/6)** | **WEAK** |
| Skill 2: Sourcing & Situation | 100% (2/2) | STRONG |
| Skill 3: Claims & Evidence in Sources | 62% (23/37) | STRONG |
| Skill 4: Contextualization | 100% (3/3) | STRONG |
| **Skill 5: Making Connections** | **43% (3/7)** | **WEAK** |
Course-to-exam drop: -19% (80% course → 62% exam).

**Key skill insight:** Ella's profile is **INVERTED from Emma and Saeed** — she CAN do source work (Skill 2: 100%, Skill 3: 62%) but can't make cross-period connections (Skill 5: 43%) or recall core historical processes (Skill 1: 50%). Her weakness is synthesis and big-picture thinking, not document analysis.

**Zero-score practice test topics (1):** 4.1 Technological Innovations 1450-1750.

**Weakest units on practice test:** Unit 1 The Global Tapestry 33% WEAK, Unit 2 Networks of Exchange 45% WEAK, Unit 4 Transoceanic Interconnections 55% WEAK — all early-period content.

**Current state:** Moderate performance overall. Strong SAQs (7/9) but weak DBQ (2/7) is dragging her score down. CED skill data reveals her weakness is in early-period content and cross-period synthesis — NOT in source analysis. Her strong Skill 2/3/4 scores explain why her SAQs are good (source-based short answers) while her DBQ is weak (requires broader connections). Topic-level data is the strongest of the 4 underperformers: 80.7% average with only 2 topics below 60%. This is a Layer 1 (early periods) + Layer 2 (synthesis/connections) problem.

**Specific weaknesses from FRQ feedback:**
- SAQ 1 (3/3): Perfect score. Good use of industrialization examples
- SAQ 2 (2/3): Correctly identified Protestant Reformation and Catholic continuity. Missed Part C (couldn't explain a specific change from the map)
- SAQ 3/4 (2/3): Good similarity (patriarchal structures) but difference about women in trade was "not reliably accurate or clearly contrasted"
- **DBQ (2/7):** Thesis not earned (restated prompt rather than making a claim). Contextualization not earned. Demonstrated some document understanding but didn't use them as evidence for an argument. No HIPP/sourcing
- LEQ (3/6): Earned thesis, contextualization, and evidence. Missed on comparison depth and sophistication

#### Layer 1: Core Knowledge Gaps
*[Source: `ap_course_progress_item_level_for_tripti.csv`]*

Ella has remarkably few content gaps — only 2 topics below 60%:
- **Unit 3:** KO Dropbox (0% — 0/6). She did not complete the Knowledge Organiser for Land-Based Empires
- **Unit 1:** World History LEQ (16.7% — but this is an FRQ-type assessment, not a knowledge test)

Her topic quiz profile is strong across all 9 units. Unit MCQ tests range from 70% (Unit 7) to 95% (Unit 4), with 6 of 8 completed units at 85%+. She has NOT completed Unit 9 MCQ test.

**Layer 1 actions:**
1. Complete KO Dropbox Unit 3 (Land-Based Empires) — this is the only genuine content encoding gap
2. Complete Unit 9 content and MCQ test — she may have a gap in Globalization content
3. Review Unit 7 (Global Conflict) content where her MCQ was lowest at 70%
4. **Layer 1 is NOT Ella's primary problem.** She has the knowledge — move quickly to Layers 2 and 3

#### Layer 2: Disciplinary Moves
**CED skill data reframes Ella's Layer 2 diagnosis:** Her Skill 5 (Making Connections) at 43% is her weakest skill — she cannot connect events across periods, regions, or themes. This explains the SAQ-vs-DBQ gap: SAQs require applying knowledge to a specific source (Skills 2/3, which she's strong at), while DBQs require synthesizing across documents to build a broader argument (Skill 5, which she's weak at).

Her gap between SAQ performance (7/9) and DBQ performance (2/7) is now clearly explained by the skill data. She can recall and apply knowledge in short-form responses but cannot construct sustained historical arguments that connect broader patterns.

Specific disciplinary skill gaps:
- **Cannot construct a thesis FROM documents:** Restated the DBQ prompt instead of making a defensible claim. But she CAN write a thesis for LEQ (earned) — so the issue is specifically about synthesizing multiple documents into a claim
- **Cannot use documents as evidence for a CONNECTED argument:** She understands documents individually but cannot deploy them to support a cross-cutting argument. This maps to Skill 5 (Making Connections) at 43%
- **No HIPP analysis:** Did not attempt sourcing on any document
- **Early-period content weakness (Skill 1: 50%):** Units 1, 2, 4 are all below 55% on the practice test — she may struggle with DBQ/LEQ prompts set in pre-1750 periods

**Layer 2 actions:**
1. **Document-to-argument practice:** Take 3 documents and write a paragraph that uses them to support a specific claim (not describe them). 2x per week
2. **HIPP template:** For each practice document, write one sentence about Historical context, Intended audience, Purpose, OR Point of view. Drill until automatic
3. **SAQ Part C precision:** She consistently misses third parts of SAQs. Practice "connect to broader historical process" answers

#### Layer 3: Exam Technique
Ella's DBQ weakness is mechanical, not conceptual — she needs to learn the formula:
- **Thesis:** Make a claim, don't restate. She can do this for LEQ already — needs to transfer the skill to DBQ
- **Contextualization:** Write 3-4 sentences about the broader period BEFORE engaging documents. She doesn't attempt this
- **Document grouping:** Organize 7 documents into 2-3 categories that map to body paragraphs
- **Sourcing point:** One HIPP analysis per DBQ to earn the sourcing point

**Layer 3 actions:**
1. **Study 3 exemplar DBQ essays:** Annotate thesis, document usage, HIPP, and contextualization in each
2. **Write 1 full DBQ per week** with self-scoring against the AP rubric — focus on earning contextualization and sourcing points she currently miss
3. **MCQ improvement:** Push from 62% to 75%+ by reviewing Unit 7 (Global Conflict, 70%) and completing Unit 9 (Globalization, untested)
4. **Timed practice:** 55 MCQs in 55 minutes to build exam-condition fluency

**Target:** Score 4-5 on next practice test. DBQ from 2/7 to 5/7. Ella has the clearest path to a 5 among the underperformers alongside Jackson Price — her content knowledge is solid and her gaps are targeted and fixable.

---

### Jackson Price (AP Score: 3 | MCQ: 78% | FRQ: 56%)

**SSD Accommodations:** None
**Full AP course load:** P1 AP World History: Modern (100% completion), P2 AP Physics 1 (0% completion), P3 AP Computer Science A (35% completion, 57% accuracy), P4 AP Chemistry (0% completion)
*[Source: Mid Term Report > ap_learning_data > approved_ssd_accommodations, course_registered]*

**CED Skill Breakdown (from updated Student Analysis v2, Feb 25):**
| CED Skill | Score | Rating |
|-----------|-------|--------|
| Skill 1: Developments & Processes | 67% (4/6) | STRONG |
| Skill 2: Sourcing & Situation | 50% (1/2) | WEAK |
| Skill 3: Claims & Evidence in Sources | 78% (29/37) | STRONG |
| Skill 4: Contextualization | 67% (2/3) | STRONG |
| Skill 5: Making Connections | 100% (7/7) | STRONG |
Course-to-exam drop: **+15%** (63% course → 78% exam) — Jackson is the ONLY student who performed BETTER on the practice test than in coursework.

**Key skill insight:** Jackson's CED profile is nearly all STRONG — Skill 5 (Making Connections) at 100% is the highest in the cohort. Only Skill 2 (Sourcing & Situation) at 50% is WEAK, but tested on only 2 questions (low confidence). His reverse course-to-exam pattern (+15%) contradicts the recognition-vs-retrieval pattern seen in every other student. He may actually perform better under structured test conditions than day-to-day coursework.

**Zero-score practice test topics (2):** 4.3 Columbian Exchange, 8.6 Newly Independent States — only 2, minimal Layer 1 gaps.

**Weakest units on practice test:** Unit 2 Networks of Exchange 64%, Unit 9 Globalization 67%. All others above 70%.

**Current state:** The most paradoxical student in the dataset. Strongest practice MCQ (78%) in the underperforming group. His Timeback data tells a very different story: 100% completion with only 54% accuracy (46% MCQ, 15% FRQ in TB). But CED skill data suggests **the practice test may be more reliable than the Timeback data** — his +15% course-to-exam improvement and nearly all-STRONG skill profile indicate genuine competence that Timeback underestimates. His real problem is FRQ (56%), not MCQ.

**Specific weaknesses from FRQ feedback:**
- SAQ 1 (3/3): Perfect score. Excellent use of smartphone, automobile, and home computer as specific examples
- SAQ 2 (2/3): Correctly identified Protestant Reformation and Christian continuity. Small error: "93 Theses" instead of "95 Theses"
- SAQ 3/4 (1/3): Called the UN an NGO (it's an IGO). Claimed TNCs have "little to no impact" on conflict/politics — factually incorrect
- **DBQ (2/7):** Earned thesis (continuities: class hostility, state control; changes: greater enforcement/coercion). But no contextualization, weak document usage, no sourcing
- LEQ (3/6): Earned thesis, contextualization, and evidence. Missed comparison depth

#### Layer 1: Core Knowledge Gaps
*[Source: `ap_course_progress_item_level_for_tripti.csv`]*

Jackson has the most widespread topic-level gaps of any World History student — **17 topics below 60%** spanning Units 1, 4-9:
- **Unit 5 (Revolutions):** Industrial Revolution Begins (32.4%), Nationalism & Revolutions (47.8%), KO Dropbox (50.0%)
- **Unit 8 (Cold War/Decolonization):** End of Cold War (47.9%), KO Dropbox (0%), Decolonization (58.3%), Global Resistance (58.6%)
- **Unit 9 (Globalization):** KO Dropbox (0%), Continuity & Change (51.9%), Globalized Culture (57.7%)
- **Unit 7 (Global Conflict):** KO Dropbox (44.4%), Causation in Global Conflict (57.9%)
- **Unit 4 (Transoceanic Interconnections):** KO Dropbox (27.3%), Changing Social Hierarchies (58.6%)
- **Unit 1 (Global Tapestry):** East Asia 1200-1450 (55.0%), World History LEQ (0%)
- **Unit 6 (Consequences of Industrialization):** Causes of Migration (56.1%)

His KO Dropbox scores are catastrophic: 0% on Units 8 and 9, 27.3% on Unit 4, 44.4% on Unit 7, 50% on Unit 5. He is not encoding ANY knowledge in his own words for the later units.

**Unit MCQ tests confirm the pattern:** Unit 6 (15%), Unit 7 (25%), Unit 8 (30%), Unit 3 (45%), Unit 4 (45%), Unit 9 (45%). Only Unit 5 (85%) and Unit 1 (70%) are above 50%. His unit FRQ average of 15.5% across 14 tests is the worst in the entire World History cohort.

**How did he score 78% MCQ on the practice test?** The CED skill data provides a new explanation: his Skill 3 (Claims & Evidence) at 78% and Skill 5 (Making Connections) at 100% suggest he IS genuinely strong at AP-style analytical questions. The +15% course-to-exam improvement (unique in the dataset) may indicate that the Timeback course format underestimates his ability — he performs better when applying knowledge to passages than on isolated recall questions. **This changes the diagnosis: Layer 1 may be less of a crisis than Timeback data suggests, and FRQ technique (Layer 3) may be the primary barrier to a higher score.**

**Layer 1 actions:**
1. **Revised priority: Layer 1 is important but may NOT be Jackson's primary problem.** His practice test MCQ (78%) + CED skill profile (nearly all STRONG) suggest he retains more knowledge than Timeback indicates. Focus retrieval practice on the specific gaps, not broad remediation
2. Complete ALL KO Dropboxes for Units 4, 5, 7, 8, 9 — he must encode knowledge in his own words
3. Targeted flashcard-based retrieval on all 17 weak topics, with spaced repetition. Focus first on Units 5 and 8 (most topics below 60%)
4. Re-test on unit MCQs for Units 3, 4, 6, 7, 8, 9 after retrieval practice to verify whether knowledge is sticking

#### Layer 2: Disciplinary Moves
**CED data shows Jackson's analytical skills are largely strong** — Skill 5 (Making Connections) at 100% and Skill 3 (Claims & Evidence) at 78% are among the best in the underperforming group. His thesis-writing is decent (earned on both DBQ and LEQ), and his only WEAK skill (Skill 2: Sourcing, 50%) was tested on just 2 questions. His Layer 2 gaps are narrow and specific:
- **Terminology precision:** NGO vs. IGO confusion, incorrect claim about TNC impact on politics
- **Factual precision:** "93 Theses" instead of "95 Theses"
- **Comparison depth:** LEQ missed on comparison sophistication — describes each region separately rather than integrating

**Layer 2 actions:**
1. **Terminology precision chart:** NGO vs. IGO, TNC impacts, and other commonly confused political science/international relations terms
2. **Factual accuracy review:** Key dates, names, and numbers for high-frequency AP exam content (95 Theses, Treaty of Westphalia 1648, etc.)
3. **Comparison skill:** Practice the "overlap" approach — each paragraph compares both regions on a theme, rather than describing A then B

#### Layer 3: Exam Technique
Jackson's thesis is a strength (earned on DBQ and LEQ). His exam technique gaps are in the middle of essays:
- **DBQ:** No contextualization (despite earning it on LEQ — so he knows how, just didn't do it). Weak document usage. No HIPP/sourcing
- **LEQ:** Earned most elements but lacked comparison sophistication
- **SAQ:** Inconsistent — perfect on factual recall (SAQ 1) but weak on analytical application (SAQ 3/4)

**Layer 3 actions:**
1. **DBQ body paragraph practice:** His thesis is fine — focus on what comes after. Practice contextualization paragraphs, document grouping into argument categories, and HIPP analysis on individual documents
2. **Timed full DBQ practice:** 1 per week, self-scored against rubric. His contextualization skill exists (earned on LEQ) — he just needs to transfer it to DBQ format
3. **MCQ maintenance:** His 78% practice MCQ is encouraging but may not be reliable given unit MCQ data. Continue stimulus-based MCQ practice to build sustained accuracy

**Target:** Score 4+ on next practice test. DBQ from 2/7 to 4-5/7. **Updated assessment (with CED data):** Jackson's practice test MCQ (78%) and nearly all-STRONG CED skill profile suggest his true ability is closer to the practice test than the Timeback data. His +15% course-to-exam improvement is unique in the dataset and indicates genuine exam competence. The primary barrier to a 5 is FRQ (56%), specifically the DBQ (2/7). If DBQ improves, Jackson has the strongest path to a 5 among the four AP World underperformers.
