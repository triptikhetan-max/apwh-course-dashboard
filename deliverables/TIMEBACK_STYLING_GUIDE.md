# Timeback Content & Styling Guide

**From:** Tripti (Content DRI / Instructional Designer)
**To:** Akshit (Engineering)
**Date:** March 23, 2026
**Purpose:** Exactly how to take our article markdown files and build them into polished course content on Timeback

---

## How to Use This Guide

This document tells you how every section in our `article.md` files maps to a Timeback content block, what styling to apply, and how to handle interactive elements (H5P, MCQs, FRQs). Use this as your single reference when building both the Jackson Remediation Course (71 topics) and the HIPP B2 Course (9 modules).

Read this alongside `MESSAGE_FOR_AKSHIT.md` (the build instructions) and the Module 2 build spec (the item-by-item prototype).

---

## 1. Article Structure on Timeback

Every `article.md` file follows the same section structure. Here is exactly how each section maps to a Timeback content block:

```
MD FILE SECTION                  ->  TIMEBACK BLOCK
----------------------------------------------------------------------
## EMBEDDED VIDEO                ->  Video Block
                                     - Embed YouTube iframe
                                     - Title above: "Watch: [Title]"
                                     - Duration note below video

## LEARNING GOAL                 ->  Text Block (styled as callout/banner)
                                     - Background color: light blue
                                     - One sentence, bold

## LEARNING OUTCOMES             ->  Text Block (styled as numbered list)
                                     - "By the end of this topic, you will
                                       be able to:"
                                     - Numbered list from CED

## STUDENT INSTRUCTIONS          ->  Text Block (styled as info box)
                                     - Background: light gray
                                     - Icons for each step
                                     - Time estimate

## ARTICLE CONTENT               ->  Rich Text Block (the main teaching)
                                     - H2 headings for sections
                                     - Bold key terms on first use
                                     - College Board callout boxes
                                     - Short paragraphs (3-5 sentences)

## KEY TERMS                     ->  Accordion Block (H5P) or Table
                                     - Term: Definition format
                                     - Collapsible if H5P available
                                     - Two-column table as fallback

## NOTE-TAKING PROMPTS           ->  Accordion Block (H5P) or List
                                     - 5 prompts, each collapsible
                                     - Prompt 5 is always the bridge to
                                       the next topic
                                     - Styled numbered list as fallback
```

### Building Each Block — Step by Step

**Video Block:**
1. Find the `## EMBEDDED VIDEO` section in the article.md
2. Extract the YouTube URL
3. Create a Video embed block (see Section 2 below for iframe details)
4. Place it as the FIRST content block the student sees

**Learning Goal Banner:**
1. Find the `## LEARNING GOAL` section
2. Create a Text Block
3. Apply the blue banner styling (see Section 3)
4. The content is always one sentence, displayed in bold
5. Place it directly below the video

**Learning Outcomes:**
1. Find the `## LEARNING OUTCOMES` section
2. Create a Text Block with a numbered list
3. Prefix with: "By the end of this topic, you will be able to:"
4. Each bullet from the article becomes a numbered item
5. Place directly below the Learning Goal banner

**Student Instructions:**
1. Find the `## STUDENT INSTRUCTIONS` section
2. Create a Text Block with the gray info-box styling
3. Preserve the step icons from the markdown (the watch/read/notes icons)
4. Include the time estimate line
5. Place below the Learning Outcomes

**Article Content (the main teaching text):**
1. Find the `## ARTICLE CONTENT` section
2. Create a Rich Text Block
3. Use H2 headings for any subsections within the article
4. Bold all key terms on their FIRST appearance in the text (they will already be bolded in the markdown with `**term**`)
5. Any sentence or paragraph that starts with or contains "College Board wants you to know" or references what College Board tests should be placed inside a styled callout box (amber/gold — see Section 3)
6. Keep paragraphs short. If a paragraph exceeds 5 sentences, it is already split in the markdown — preserve those breaks
7. This is the largest block. Place it after Student Instructions.

**Key Terms:**
1. Find the `## KEY TERMS` section
2. Each line has the format: `- **Term** -- Definition`
3. If H5P Accordion is available: create a collapsible accordion where each panel header is the term and the body is the definition
4. If H5P is not available: create a two-column table (Term | Definition) with the green background styling
5. Place after the Article Content block

**Note-Taking Prompts:**
1. Find the `## NOTE-TAKING PROMPTS` section
2. There are always 5 prompts, numbered 1-5
3. Prompt 5 always begins with "Connection:" and bridges to the next topic
4. If H5P Accordion is available: each prompt is a collapsible panel (prompt text visible, students can expand to write notes)
5. If no H5P: display as a styled numbered list with the pink background
6. Place as the LAST block in the article

---

## 2. Video Embedding

### Standard YouTube Embed (Jackson Course)

Every Jackson course article has a Heimler's History video. Here is how to embed it.

**Step 1:** Find the YouTube URL in the article. It will appear in one of two formats:

```
- URL: https://www.youtube.com/watch?v=HfIWZhXt7fY
```
or
```
**Video:** [Heimler's History - Title](https://www.youtube.com/watch?v=hFCnwYlWPJc)
```

**Step 2:** Extract the VIDEO_ID. This is the string after `watch?v=` in the URL.

Examples:
- URL: `https://www.youtube.com/watch?v=HfIWZhXt7fY` -> VIDEO_ID = `HfIWZhXt7fY`
- URL: `https://www.youtube.com/watch?v=hFCnwYlWPJc` -> VIDEO_ID = `hFCnwYlWPJc`

**Step 3:** Build the iframe:

```html
<iframe
  width="100%"
  height="400"
  src="https://www.youtube.com/embed/VIDEO_ID"
  frameborder="0"
  allowfullscreen>
</iframe>
```

**Step 4:** Add the title ABOVE the video:

```
Watch: Heimler's History -- [Topic Title]
```

Use the title from the article's `## EMBEDDED VIDEO` section. For example, Topic 1.1 has:
- Title: "Developments in EAST ASIA [AP World Review -- Unit 1 Topic 1]"
- Display as: "Watch: Heimler's History -- Developments in East Asia"

**Step 5:** Add a text note BELOW the video:

```
Duration: ~X minutes. Take notes as you watch.
```

The duration is listed in the article (e.g., "Duration: 11:36" becomes "Duration: ~12 minutes").

### Timestamp Embedding (HIPP Course)

Some HIPP modules use only a segment of a video. When you see a timestamp instruction like:

```
- Cue to timestamp: 13:10
```

Add the start parameter to the embed URL:

```html
<iframe
  width="100%"
  height="400"
  src="https://www.youtube.com/embed/VIDEO_ID?start=790"
  frameborder="0"
  allowfullscreen>
</iframe>
```

Convert the timestamp to seconds: 13:10 = 13 * 60 + 10 = 790 seconds.

Update the duration note to reflect the segment length:

```
Duration: ~2.5 minutes (starting at 13:10). Watch to the end of the video.
```

### No Video Embed (HIPP Modules 2-7)

Most HIPP modules are article-driven and do NOT have a video embed. If the build spec says "No video embed needed" or "article-driven," skip the video block entirely. Some modules have a text reference to what students watched in Module 1 — build that as a regular Text Block, not a Video Block.

---

## 3. Styling Guide

### Color Palette

Use these exact colors for each block type. Every styled block should have a subtle left border (4px) in addition to the background color.

| Block Type | Background | Text Color | Left Border | Usage |
|---|---|---|---|---|
| Learning Goal banner | `#EFF6FF` | `#1D4ED8` | `#1D4ED8` | One sentence learning goal at top |
| College Board callout | `#FEF3C7` | `#92400E` | `#D97706` | "College Board wants you to know..." |
| Student Instructions | `#F3F4F6` | `#374151` | `#9CA3AF` | Step-by-step instructions box |
| Key Terms | `#F0FDF4` | `#166534` | `#16A34A` | Term definitions section |
| Note-Taking Prompts | `#FDF2F8` | `#9D174D` | `#DB2777` | 5 prompts at end of article |
| Document Card | `#F9FAFB` | `#111827` | `#D1D5DB` | Primary source documents (HIPP) |
| Good example | `#F0FDF4` | `#166534` | `#16A34A` | "Earns the point" examples |
| Bad example | `#FEF2F2` | `#991B1B` | `#EF4444` | "0 points" examples |

### Typography

| Element | Size | Weight | Line Height | Notes |
|---|---|---|---|---|
| Article headings (H2) | 18-20px | Bold | 1.4 | Used for major sections within article content |
| Article subheadings (H3) | 16-18px | Bold | 1.4 | Used for subsections |
| Body text | 14-16px | Normal | 1.6 | Standard paragraph text |
| Key terms (first use) | 14-16px | **Bold** | 1.6 | Bold on first appearance in body text |
| Callout text | 14px | Italic | 1.5 | Inside College Board callout boxes |
| Source line (documents) | 14px | Italic | 1.5 | Italicized attribution above document text |
| Block quote text | 14-16px | Normal | 1.6 | Student example responses, model answers |

### Layout

| Property | Value | Notes |
|---|---|---|
| Max content width | 720px | Keeps line length readable (50-75 characters per line) |
| Content padding | 20px all sides | Inside each content block |
| Spacing between sections | 24px | Gap between consecutive blocks |
| Spacing between paragraphs | 12px | Within article content |
| Video width | 100% of content area | Fills the 720px max width |
| Video height | 400px | Standard 16:9 embed height |
| Styled block padding | 16px all sides | Inside callout boxes, banners, etc. |
| Styled block border-radius | 8px | Rounded corners on all styled blocks |
| Left border width | 4px | On all colored callout blocks |

### Styled Callout Boxes — How to Build Them

When you encounter text in the article that references College Board specifically (phrases like "College Board loves testing," "College Board wants you to know," "College Board frequently tests"), wrap that sentence or paragraph in a callout box:

```
+------------------------------------------------------------------+
|  [amber background #FEF3C7]                                      |
|  [4px left border #D97706]                                       |
|                                                                  |
|  College Board Tip                                               |
|  [italic text in #92400E]                                        |
|  "College Board frequently tests these different responses to    |
|  Chinese influence -- remember that each country adapted Chinese |
|  culture differently based on their own needs."                  |
|                                                                  |
+------------------------------------------------------------------+
```

For the Learning Goal banner:

```
+------------------------------------------------------------------+
|  [blue background #EFF6FF]                                       |
|  [4px left border #1D4ED8]                                       |
|                                                                  |
|  Learning Goal                                                   |
|  [bold text in #1D4ED8]                                          |
|  "Explain how Song China used traditional methods while          |
|  innovating economically, and analyze how Chinese culture        |
|  influenced East Asia."                                          |
|                                                                  |
+------------------------------------------------------------------+
```

---

## 4. H5P Elements

H5P elements fall into two categories:
- **Jackson Course:** Nice-to-have (accordion for key terms and note-taking prompts, flashcards for review). Do not block launch on these.
- **HIPP Course:** Required. These are core to the instructional design.

### Accordion (Both Courses)

**Purpose:** Collapsible sections that reveal content on click.

**Where used:**
- Key Terms (both courses): Each panel header = the term in bold. Panel body = the definition. Student clicks to expand.
- Note-Taking Prompts (both courses): Each panel header = "Prompt 1", "Prompt 2", etc. Panel body = the full prompt text.
- "Need help?" hints (HIPP course): A single collapsible panel with historical context hints for practice documents.

**How to build:**
1. Create an H5P Accordion element
2. For Key Terms: one panel per term. Header text is the term name. Body text is the definition.
3. For Note-Taking Prompts: one panel per prompt (5 total). Header is "Prompt 1: [short label]". Body is the full prompt text.
4. For hints: one panel labeled "Need help? Click for historical context." Body contains the hint text from the build spec.
5. All panels start COLLAPSED. Student clicks to expand.

**Fallback (if H5P not available):**
- Key Terms: two-column table with green background (`#F0FDF4`)
- Note-Taking Prompts: styled numbered list with pink background (`#FDF2F8`)
- Hints: regular text block with gray background, prefixed with "Hint:"

### Reveal (HIPP Course Only — Required)

**Purpose:** Shows a model answer AFTER the student submits their own response.

**Where used:** Every FRQ/writing practice item in the HIPP course. After the student submits their Historical Situation (or Purpose, Audience, POV) analysis, a "Show Model Answer" button appears. Clicking it reveals the exemplar response.

**How to build:**
1. Student sees the document + prompt + text area
2. Student types and clicks "Submit"
3. Autograder scores the response (Score 0 or Score 1) and shows feedback
4. A "Show Model Answer" button appears below the feedback
5. Clicking the button reveals the model answer in a styled box (green background `#F0FDF4`, green left border `#16A34A`)
6. The model answer text comes from the build spec's "Model Answer" field for that item
7. Below the model answer, add a note: "Compare your response to this model. Did you include the 'and that matters because' clause?"

### Fill-in-the-Blanks (HIPP Course Only — Required)

**Purpose:** Interactive sentence frame practice where students type into blank fields within a pre-written sentence structure.

**Where used:** Guided practice documents in the HIPP course (Docs 1-2 in each module), where students complete a sentence frame rather than writing from scratch.

**How to build:**
1. Display the sentence frame with blank input fields where the underscores are
2. Example from Module 2, Practice Doc 1:

```
"During this time period, the Mauryan Empire was
[___________________________________],
and that matters because
[___________________________________]."
```

3. Each blank is a text input field (minimum width 300px)
4. After the student fills in the blanks and submits, show the complete model answer via Reveal (see above)
5. The fill-in-the-blanks format is used for Practice Docs 1-2 (guided). Docs 3-5 use a full text area (open response) with decreasing scaffolding.

---

## 5. MCQ Formatting

MCQs appear in two places:
- **Jackson Course:** Diagnostic (3 per topic) and MCQ Practice (6 per topic, FULL path only). Questions and answer keys are in `apwh_full_course_spec.md`.
- **HIPP Course:** Discrimination practice (3 MCQs per module). Questions are in each module's build spec.

### MCQ Layout

**Stimulus / Document Card:**
- Many MCQs are stimulus-based (a primary source excerpt, chart, or passage is shown above the question)
- Display the stimulus in a Document Card (see Section 7 below for Document Card styling)
- The source line goes at the TOP of the card, in italic
- The document text goes below the source line

**Question Stem:**
- Displayed below the stimulus card
- Regular body text (14-16px)
- Starts with "Which of the following..." or similar AP-style phrasing

**Answer Choices:**
- 4 choices, always labeled (A), (B), (C), (D)
- Radio buttons (single select)
- Each choice on its own line with adequate spacing (12px between choices)
- Choice text wraps naturally — do not truncate

**After Submission:**
- Highlight the student's selected answer:
  - Correct: green background (`#F0FDF4`) with green left border
  - Incorrect: red background (`#FEF2F2`) with red left border
- Show the correct answer if the student got it wrong
- Show explanation text for EVERY choice (not just the one they picked). The explanations are in the build spec / course spec, formatted as:
  - **(A)** "Explanation of why A is right/wrong..."
  - **(B)** "Explanation of why B is right/wrong..."
  - etc.
- Students should see all four explanations so they understand the reasoning behind each option

### MCQ Display Template

```
+------------------------------------------------------------------+
|  STIMULUS CARD (if applicable)                                   |
|  [Document Card styling - see Section 7]                         |
|  Source: [italic source line]                                    |
|  [document text]                                                 |
+------------------------------------------------------------------+

Question: Which of the following is the best Historical Situation
analysis for this document?

  ( ) (A) "This was written in Africa during the 1800s."
  ( ) (B) "This was written during European imperialism in Africa."
  ( ) (C) "The Temne leaders were angry about the hut tax..."
  (x) (D) "This letter was written during the Scramble for Africa..."

[SUBMIT]

--- After submission ---

Correct! You selected (D).

(A) Too vague. "Africa during the 1800s" covers an entire continent
    across an entire century. 0 points.
(B) Better -- names a specific development. But no explanation of
    why it matters to this document. 0 points.
(C) Not Historical Situation -- describes document content. 0 points.
(D) CORRECT. Identifies Scramble for Africa + colonial administration.
    Explains why it matters. Earns the point.
```

---

## 6. FRQ / Essay Formatting

FRQs appear in two places:
- **Jackson Course:** Essay practice (SAQ, LEQ, or mini-DBQ per topic, FULL path only). Prompts and rubrics are in `apwh_full_course_spec.md`.
- **HIPP Course:** Writing practice (5 practice documents per module with decreasing scaffolding). Prompts, rubrics, model answers, and feedback are in each module's build spec.

### FRQ Layout

**Prompt Card:**
- Display the essay prompt in a styled card similar to the MCQ stimulus
- Background: `#F9FAFB`, border: 1px solid `#E5E7EB`, border-radius: 8px
- For HIPP practice: include the Document Card (source line + document text) above the writing prompt

**Response Area:**
- Large text area for student response
- Minimum height: 200px
- Placeholder text: "Type your response here..."
- Allow the text area to expand as the student types

**Submit Button:**
- Below the text area
- Standard button styling
- Label: "Submit"

**After Submission — Scoring and Feedback:**

The autograder evaluates the response against the rubric criteria in the build spec.

For HIPP single-element practice (Modules 2-5):
```
+------------------------------------------------------------------+
|  Score: 1/1                                                      |
|  [green background if Score 1, red if Score 0]                   |
|                                                                  |
|  Feedback:                                                       |
|  "Strong work! You identified [specific development] and         |
|  explained why it matters to the document. Your 'and that        |
|  matters because' clause connects context to content."           |
+------------------------------------------------------------------+
```

For full HIPP analysis (Modules 6-7):
```
+------------------------------------------------------------------+
|  Score: 3/4                                                      |
|                                                                  |
|  H (Historical Situation): 1/1                                   |
|  I (Intended Audience):    1/1                                   |
|  P (Purpose):              1/1                                   |
|  POV (Point of View):      0/1                                   |
|                                                                  |
|  Feedback for POV:                                               |
|  "You identified the author's point of view but did not explain  |
|  why the author holds that perspective. Add the 'and that        |
|  matters because' clause."                                       |
+------------------------------------------------------------------+
```

**After Scoring — Model Answer (via H5P Reveal):**
- A "Show Model Answer" button appears below the feedback
- Clicking reveals the exemplar response from the build spec
- Model answer displayed in a green-styled box (`#F0FDF4` background)
- Below the model answer: "Compare your response to this model. What did you include that the model has? What did you miss?"

### FRQ Display Template

```
+------------------------------------------------------------------+
|  DOCUMENT CARD (for HIPP practice)                               |
|  Source: [italic source line at TOP]                             |
|  [document text]                                                 |
+------------------------------------------------------------------+

Prompt: Write a Historical Situation analysis for this document.
Remember to use the "and that matters because" clause.

+------------------------------------------------------------------+
|  [text area - min 200px height]                                  |
|  Type your response here...                                      |
|                                                                  |
|                                                                  |
+------------------------------------------------------------------+
                                                        [Submit]

--- After submission ---

+------------------------------------------------------------------+
|  Score: 1/1                                                      |
|  [feedback message from build spec]                              |
+------------------------------------------------------------------+

                                         [Show Model Answer]

--- After clicking Show Model Answer ---

+------------------------------------------------------------------+
|  Model Answer                                [green background]  |
|  "The historical situation was British colonial expansion in     |
|  India during the mid-19th century, when the Raj was building    |
|  extensive railroad networks using Indian labor and capital.     |
|  This matters because the petitioners, as elite Indians          |
|  operating within the colonial system, had a direct economic     |
|  stake in how railroad development affected Indian interests..." |
+------------------------------------------------------------------+
|  Compare your response to this model. Did you include the        |
|  "and that matters because" clause?                              |
+------------------------------------------------------------------+
```

---

## 7. Document Cards (for HIPP Practice)

When displaying a primary source document for student analysis, use a distinct Document Card style that visually separates the source material from instructional text.

### Document Card Styling

| Property | Value |
|---|---|
| Background | `#F9FAFB` |
| Border | 1px solid `#D1D5DB` |
| Border-radius | 8px |
| Padding | 20px |
| Left border | 4px solid `#D1D5DB` |
| Max width | Same as content area (720px) |

### Document Card Structure

```
+------------------------------------------------------------------+
|  [4px left border #D1D5DB]                                       |
|  [background #F9FAFB]                                            |
|                                                                  |
|  Source: Chanakya, political advisor to the Mauryan emperor,     |
|  Arthashastra (a political treatise on statecraft and wealth),   |
|  c. 250 BCE                                                      |
|  [italic, 14px]                                                  |
|                                                                  |
|  ---  (thin horizontal rule separating source from text)         |
|                                                                  |
|  [Document text in a slightly different font]                    |
|  "The king shall maintain contact with frontier officers and     |
|  neighboring rulers through communication and trade..."          |
|  [regular weight, 14-16px]                                       |
|                                                                  |
+------------------------------------------------------------------+
```

### Critical Rules for Document Cards

1. **Source line goes at the TOP.** This is non-negotiable. Students must read the source line FIRST because it contains the author, date, and context they need for HIPP analysis. The entire pedagogical approach depends on students seeing the source line before the document text.

2. **Use a thin horizontal rule** (1px, `#E5E7EB`) to separate the source line from the document body.

3. **Font differentiation:** Use a serif font (like Georgia or Times New Roman) or a slightly different font weight for the document text to visually distinguish the primary source from instructional text. This helps students recognize "this is the source I'm analyzing" versus "this is the article teaching me."

4. **Preserve original formatting.** If the source document has line breaks, paragraph breaks, or italics, preserve them exactly as they appear in the released AP exam PDFs. These documents come from `/reports/hipp_research/released_ap_docs/frq_sets/` — the build spec tells you exactly which PDF and which document number to extract.

5. **No truncation.** Show the COMPLETE document text. Students need the full text for analysis.

---

## 8. Course Navigation

### Sequential Unlock (Both Courses)

Students progress through content in a fixed order. Each item must be completed before the next one unlocks.

**Jackson Course sequence per topic:**
1. Embedded Video (must watch / mark complete)
2. Article (must scroll to bottom / mark complete)
3. MCQ Practice — 6 questions (FULL path only)
4. Essay (FULL path only)

**HIPP Course sequence per module (using Module 2 as template):**
1. Video Reference note (Item 1)
2. Article: "What is Historical Situation?" (Item 2)
3. Article: "The Golden Rule" (Item 3)
4. Article: Sentence Frames (Item 4)
5. Worked Example 1 — Teacher think-aloud (Item 5)
6. Worked Example 2 — Good vs. Bad (Item 6)
7. Common Mistakes (Item 7)
8. MCQ 1 (Item 8)
9. MCQ 2 (Item 9)
10. MCQ 3 (Item 10)
11. Practice Doc 1 — Guided FRQ (Item 11)
12. Practice Doc 2 — Guided FRQ (Item 12)
13. Practice Doc 3 — Semi-Guided FRQ (Item 13)
14. Practice Doc 4 — Independent FRQ (Item 14)
15. Practice Doc 5 — Independent FRQ (Item 15)
16. Reflection (Item 16)

### Progress Bar

- Display a progress bar at the top of each topic/module showing completion percentage
- Format: "3 of 16 items complete" or a visual bar
- The bar updates as the student completes each item

### Diagnostic Gating (Jackson Course Only)

The Jackson course has a diagnostic at the start (Princeton Practice Test 1, 55 MCQs). The diagnostic score per unit determines the student's path:

| Unit Score | Path | What the Student Sees |
|---|---|---|
| 80%+ correct | SKIP | Unit is grayed out with a checkmark. Student moves to next unit. |
| 50-79% | SKIM | Student gets Video + Article only. No MCQ practice, no essay. |
| Below 50% | FULL | Student gets Video + Article + 6 MCQs + Essay for every topic. |

After the diagnostic, display a "Your Path" summary:

```
Your Diagnostic Results:
  Unit 1 (East Asia): 40% -- FULL PRACTICE
  Unit 2 (Networks): 80% -- SKIP
  Unit 3 (Land Empires): 60% -- SKIM (video + article)
  ...
```

**Path B students (Emma, Saeed, Ella):** These students do NOT take the diagnostic. They go straight into their assigned units. Tripti will provide per-student unit assignments separately.

### Module Progress (HIPP Course)

Display module progress as: "Module 2 of 9" with a visual indicator showing which modules are complete, current, and locked.

```
[1 done] [2 current] [3 locked] [4 locked] ... [9 locked]
```

---

## 9. Quick Reference: Article.md to Timeback Mapping

Use this table as a cheat sheet when building any article.

| Article.md Section | Timeback Block Type | Styling | Priority | Notes |
|---|---|---|---|---|
| `## EMBEDDED VIDEO` | Video embed (YouTube iframe) | Full width, title above, duration below | Required | Extract VIDEO_ID from URL |
| `## LEARNING GOAL` | Banner/callout block | Blue: `#EFF6FF` bg, `#1D4ED8` text | Required | One sentence, bold |
| `## LEARNING OUTCOMES` | Numbered list | Below learning goal, normal styling | Required | Prefixed with "By the end of this topic..." |
| `## STUDENT INSTRUCTIONS` | Info box | Gray: `#F3F4F6` bg, `#374151` text | Required | Preserve step icons and time estimate |
| `## ARTICLE CONTENT` | Rich text | Bold key terms, CB callout boxes in amber | Required | Largest block. Short paragraphs. |
| `## KEY TERMS` | Accordion (H5P) or two-column table | Green: `#F0FDF4` bg, `#166534` text | Required (accordion is nice-to-have for Jackson, required for HIPP) | Term = panel header, definition = body |
| `## NOTE-TAKING PROMPTS` | Accordion (H5P) or numbered list | Pink: `#FDF2F8` bg, `#9D174D` text | Required (accordion is nice-to-have for Jackson, required for HIPP) | 5 prompts. #5 = bridge to next topic. |
| Diagnostic (3 MCQs) | Quiz block | Standard MCQ layout | Required | From `apwh_full_course_spec.md`, NOT from article |
| MCQ Practice (6 Qs) | Quiz block | Standard MCQ layout | Required (FULL path only) | From `apwh_full_course_spec.md`, NOT from article |
| Essay | FRQ block | Document card + text area + autograder | Required (FULL path only) | From `apwh_full_course_spec.md`, NOT from article |

---

## 10. HIPP Course vs. Jackson Course — Key Differences

Some elements work differently between the two courses. Here is a summary so you do not mix them up.

| Feature | Jackson Course (Remediation) | HIPP Course (B2) |
|---|---|---|
| H5P Accordion | Nice-to-have (use table/list fallback if needed) | Required |
| H5P Reveal | Not used | Required (model answers after FRQs) |
| H5P Fill-in-Blanks | Not used | Required (guided practice docs) |
| Video | Every topic has a Heimler video embed | Only Modules 1, 8, 9 have video. Modules 2-7 are article-driven. |
| MCQ source | `apwh_full_course_spec.md` (Sections 8-9 per topic) | Each module's build spec |
| FRQ source | `apwh_full_course_spec.md` (Sections 10-11 per topic) | Each module's build spec |
| Autograder | Rubric criteria in course spec per essay | Detailed rubric per practice doc in build spec (Score 0 criteria, Score 1 criteria, keywords, differentiated feedback) |
| Document Cards | Not typically used (MCQ stimuli are shorter excerpts) | Used extensively for practice documents |
| Diagnostic gating | Yes (Princeton Practice Test 1) | No |
| Paths (Skip/Skim/Full) | Yes | No — all students do all items |

---

## 11. File Locations Reference

When building, here is where to find everything:

| What You Need | Where to Find It |
|---|---|
| Jackson course article content | `01_jackson_course/articles/topic_X.X/article.md` |
| Video URLs | Inside each article file (look for `## EMBEDDED VIDEO`) |
| Video URL backup | `01_jackson_course/source_data/video/all_units_video_map.md` |
| Diagnostic questions (3 per topic) | `04_course_specs/apwh_full_course_spec.md` -- Section 8 per topic |
| MCQ practice (6 per topic) | `04_course_specs/apwh_full_course_spec.md` -- Section 9 per topic |
| Essay prompts + rubrics | `04_course_specs/apwh_full_course_spec.md` -- Sections 10-11 per topic |
| Units 8-9 expanded content | `04_course_specs/apwh_units_8_9_expanded.md` |
| CED learning objectives | `01_jackson_course/source_data/ced/topic_X.X_ced.md` |
| HIPP Module 2 article | `02_hipp_course/module_2_historical_situation.md` |
| HIPP Module 2 build spec | `02_hipp_course/module_2_akshit_build_spec.md` |
| Released AP exam PDFs (for document scraping) | `03_hipp_research/released_ap_docs/frq_sets/` |
| Document catalog (which doc from which year) | `03_hipp_research/04_released_dbq_document_catalog.md` |
| Scoring guidelines | `03_hipp_research/released_ap_docs/scoring_guidelines/` |

---

## 12. Checklist: Building One Jackson Course Topic

Use this checklist for each of the 71 topics:

- [ ] Open `topic_X.X/article.md`
- [ ] Create Video Block: extract YouTube URL, build iframe, add title + duration
- [ ] Create Learning Goal banner (blue styling)
- [ ] Create Learning Outcomes list
- [ ] Create Student Instructions box (gray styling)
- [ ] Create Article Content block: bold key terms, extract College Board callouts into amber boxes
- [ ] Create Key Terms block: accordion (if H5P) or green table
- [ ] Create Note-Taking Prompts block: accordion (if H5P) or pink list
- [ ] Open `apwh_full_course_spec.md`, find this topic's section
- [ ] Build Diagnostic (3 MCQs) with answer explanations
- [ ] Build MCQ Practice (6 questions) with answer explanations
- [ ] Build Essay prompt with autograder rubric
- [ ] Set sequential unlock order
- [ ] Test: video plays, all blocks render, MCQ scoring works, essay submission + feedback works

## 13. Checklist: Building One HIPP Module

Use this checklist for each of the 9 HIPP modules (Module 2 is the template):

- [ ] Open the module's build spec (e.g., `module_2_akshit_build_spec.md`)
- [ ] Build each item in order (Item 1 through Item 16)
- [ ] For article items: copy content from build spec, apply styling per this guide
- [ ] For MCQ items: build with stimulus card, 4 choices, per-choice feedback
- [ ] For FRQ items: build document card + prompt + text area + autograder
- [ ] Set up autograder with Score 0 / Score 1 criteria and keywords from build spec
- [ ] Set up differentiated feedback (different messages for Score 0 vs Score 1)
- [ ] Build H5P Reveal for model answers on all FRQ items
- [ ] Build H5P Accordion for hints on guided practice docs
- [ ] Build H5P Fill-in-Blanks for sentence frame practice (guided docs only)
- [ ] For document scraping: open the correct PDF from `released_ap_docs/frq_sets/`, find the correct document number, extract source line + full text verbatim
- [ ] Set sequential unlock (Item 1 -> 2 -> ... -> 16)
- [ ] Test: all items render, MCQ scoring works, FRQ autograder scores correctly, Reveal shows model answer, Accordion expands/collapses

---

## Questions?

If anything in this guide conflicts with what Timeback can actually do, flag it. Do not improvise on content or styling decisions — ask Tripti. You build what the spec says; Tripti reviews before it goes live.
