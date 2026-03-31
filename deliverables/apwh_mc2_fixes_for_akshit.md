# AP World History MC2 (Russia) — Engineering Fix Doc

**For:** Akshit (engineer)
**Course ID:** `s4-r1r3-mc2-83cb26f8`
**Course Title:** AP World: Russia (Kievan Rus to Soviet)
**Pull Date:** 2026-03-19
**QC Date:** 2026-03-20
**Status:** `publishStatus: testing`

---

## 1. COURSE OVERVIEW

**Current state:** 232 MCQ across 12 topic quizzes + 1 Mini MCQ quiz + 3 FRQ (235 total items)

**VERDICT: Only 83 of 232 MCQ (35.8%) are Russia/Soviet-specific. Course needs structural rebuild.**

| Classification | Count | % |
|----------------|-------|---|
| KEEP (Russia-specific) | 83 | 35.8% |
| DELETE (wrong topic) | 121 | 52.2% |
| DELETE (old format / 5-choice) | 11 | 4.7% |
| DELETE (duplicate) | 12 | 5.2% |
| DELETE (FRQ — not Russia) | 3 | 1.3% |
| **Total** | **232 MC + 3 FRQ** | **100%** |

Two quizzes have **0% keepable questions** (Industrialization Spreads, Unresolved Tensions After WWI). Two quizzes are **95-100%** keepable (The Cold War, End of the Cold War).

---

## 2. TOPIC FLOW — CURRENT vs PROPOSED

### Current Structure (12 topics)

| # | Current Topic | Test ID | Qs | KEEP | Action |
|---|---------------|---------|-----|------|--------|
| 1 | Empires Expand (Unit 3) | `pcb-resource-729d5633d2c74682ab8761c0b9779bd7` | 18 | 3 | COMBINE with 3.2+3.3, filter Russia |
| 2 | Empires: Administration (Unit 3) | `pcb-resource-a5847f4d738e4ba1b7a8600f4d3eb330` | 21 | 2 | COMBINE with 3.1+3.3, filter Russia |
| 3 | Empires: Belief Systems (Unit 3) | `pcb-resource-6291f51f016d412cb82ead7562b09cb0` | 7 | 2 | DELETE topic, merge 2 Qs into combined 3.x |
| 4 | Industrialization Spreads (Unit 5) | `pcb-resource-51dbe45f058a4775b5bdc54c80fd93b7` | 16 | 0 | DELETE (0% Russia) — merge into combined 5.x |
| 5 | Ind: Gov't Role (Unit 5) | `pcb-resource-700785c088f349c9a7505f80e977bc68` | 26 | 6 | KEEP 6, combine into Topic 3 |
| 6 | Causes of WWI (Unit 7) | `pcb-resource-cf3daafe79674053add1bb42e1c22b51` | 19 | 7 | KEEP, filter Russia, becomes Topic 5 |
| 7 | Unresolved Tensions (Unit 7) | `pcb-resource-1f06c2d384104b8ab23a736b65df2a83` | 12 | 0 | DELETE (0% Russia) |
| 8 | Setting Stage CW (Unit 8) | `pcb-resource-4526e6d16ce1477796e869746fd9db7e` | 19 | 7 | KEEP, becomes Topic 6 (Soviet/Stalin) |
| 9 | The Cold War (Unit 8) | `pcb-resource-f9d28bfb5d614d6ea75fca9c5dc4c92c` | 19 | 18 | Split across Topics 6+7 |
| 10 | Effects of CW (Unit 8) | `pcb-resource-3513d67d3e354167837d588dc4373966` | 21 | 14 | Split across Topics 7+Mini MCQ |
| 11 | Spread of Communism (Unit 8) | `pcb-resource-7178ea54cf49496d9022dd669f52afb1` | 16 | 5 | Merge Soviet Qs into Topic 7 |
| 12 | End of Cold War (Unit 8) | `pcb-resource-3916af733cec480b921543dda17d7393` | 13 | 13 | KEEP as Topic 8 |
| -- | Mini MCQ | `pcb-resource-3644c663ac044b00b745e1d79a890eaa` | 25 | 6 | REBUILD from scratch |
| -- | FRQ/SAQ | `2ce28f90-438d-402a-b340-05156fe801ae` | 3 | 0 | DELETE all 3 |

### PROPOSED STRUCTURE (8 topics + Mini MCQ + FRQ)

The new topic flow tells the story of Russia: frontier state → Mongol subjugation → imperial expansion → modernization → revolution → Soviet superpower → Cold War → collapse.

| New # | Title | CED | Period | Source |
|-------|-------|-----|--------|--------|
| **1** | Kievan Rus & Mongol Yoke | 1.8/2.2 | 1200-1450 | **NEW** — source 10 Qs from prep books + AP Classroom |
| **2** | Russian Empire & Tsardom | 3.1-3.2 | 1450-1750 | 7 KEEP from 3.1+3.2+3.3, add 3 from prep books |
| **3** | Russian Industrialization | 5.4/5.6 | 1750-1900 | 6 KEEP from 5.6, add 4 from prep books |
| **4** | Russian Reform & 1905 Revolution | 5.3/6.3 | 1860-1910 | **NEW** — source 10 Qs from prep books + AP Classroom |
| **5** | WWI & Russian Revolution | 7.2/7.5 | 1914-1922 | 7 KEEP from 7.2, add 3 from prep books |
| **6** | Soviet Union & Stalin | 8.1 | 1922-1945 | 7 KEEP from 8.1, add 3 from prep books |
| **7** | Cold War Soviet Union | 8.2/8.3/8.4 | 1945-1985 | 10 best from 37 KEEP across 8.2+8.3+8.4 |
| **8** | Fall of USSR & End of Cold War | 8.8 | 1985-1991 | 10 KEEP from 8.8 (trim 3) |
| -- | SAQ (×8) | per topic | per topic | **NEW** — 1 SAQ after each topic |
| -- | Mini MCQ Practice Quiz | all | all | REBUILD: 24 Qs, 3 per topic, mixed topics |
| -- | LEQ | cumulative | all | **NEW** — Russia-specific prompt from prep book |
| -- | DBQ | cumulative | 20th c. | **NEW** — Russia-specific prompt from prep book |

### Topics DELETED from current course

| Current Topic | Test ID | Why |
|---------------|---------|-----|
| 3.3 Empires: Belief Systems | `pcb-resource-6291f51f016d412cb82ead7562b09cb0` | 2 of 7 Russia. Merge those 2 into Topic 2, delete rest |
| 5.4 Industrialization Spreads | `pcb-resource-51dbe45f058a4775b5bdc54c80fd93b7` | 0% Russia. All Japan/India/generic |
| 7.5 Unresolved Tensions | `pcb-resource-1f06c2d384104b8ab23a736b65df2a83` | 0% Russia. All Japan/Ethiopia/Africa |

### New topics to ADD — SOURCE FROM PREP BOOKS + AP CLASSROOM

**Do NOT source from base course.** Source replacement questions from the prep books listed below. Akshit to scrape the questions from the prep book EPUBs. For any gaps, source from AP Classroom.

**Prep book locations:**
- Barron's 2024: `/tmp/apwh_prep/World History/John McCannon - AP World History_ Modern Premium, 2024...epub`
- Princeton 2024: `/tmp/apwh_prep/World History/The Princeton Review - Princeton Review AP World History...epub`

| New Topic | Prep Book Sources | AP Classroom Backup |
|-----------|-------------------|---------------------|
| **Topic 1: Kievan Rus & Mongol Yoke** | Barron's: Ch 1 Q10-Q12 (Song/Yuan — Mongol context), Ch 2 Q13-Q14 (neo-Confucianism/mandate of heaven — cross-cultural comparison with Russian Orthodox), Ch 6 Q17 (Black Death spread via Mongol routes). Princeton: PT4 Q7, Q10-Q11 (Mongol/Marco Polo — Mongol Empire context), PT5 Q19 (Mongol control Russia vs China), PT6 Q1 (Mongols invading central Asia), Q19 (Mongol rule Russia vs China). **~8-10 Qs with Russia/Mongol relevance.** | Source 2-4 more from AP Classroom CED 1.8/2.2 — Russia/Mongol specific |
| **Topic 4: Russian Reform & 1905 Revolution** | Barron's: Ch 15 (Governance 1750-1900) — search for Russia/reform questions, Ch 17 (Social 1750-1900) — search for Russian emancipation/serfs. Princeton: Ch 8 (Period 3 review) — Russian industrialization/reform content. PT3 Q28 (Japan defeated China — comparison context for Russo-Japanese War). | Source 6-8 from AP Classroom CED 5.3/6.3 — 1905 Revolution, Bloody Sunday, Stolypin reforms |

### DEDUPLICATION WITH MC1 (China)

These resources are **identical** between MC1 and MC2. Students taking both courses see duplicate content.

| Resource ID | Type | MC1 Topic | MC2 Topic |
|-------------|------|-----------|-----------|
| `WORH23-r103868-v1` | Video | 3.1 Empires Expand | 3.1 Empires Expand |
| `WORH23-r103869-v1` | Article | 3.1 Empires Expand | 3.1 Empires Expand |
| `WORH23-r103871-v1` | Video | 3.2 Empires Admin | 3.2 Empires Admin |
| `WORH23-r103872-v1` | Article | 3.2 Empires Admin | 3.2 Empires Admin |
| `WORH23-r103874-v1` | Video | 3.3 Belief Systems | 3.3 Belief Systems |
| `WORH23-r103875-v1` | Article | 3.3 Belief Systems | 3.3 Belief Systems |
| `WORH23-r104003-v1` | Video | 8.2 The Cold War | 8.2 The Cold War |
| `WORH23-r104004-v1` | Article | 8.2 The Cold War | 8.2 The Cold War |
| `d75cdd8b-08bf-4f52-b3c4-cdb3fdcb2196` | Video | 8.3 Effects of CW | 8.3 Effects of CW |
| `454dce3b-2f24-4bf8-a1bf-45b36d2b9df0` | Article | 8.3 Effects of CW | 8.3 Effects of CW |
| `WORH23-r104009-v1` | Video | 8.4 Spread of Communism | 8.4 Spread of Communism |
| `WORH23-r104010-v1` | Article | 8.4 Spread of Communism | 8.4 Spread of Communism |

**Resolution:** After rebuild, MC1 gets China-specific videos/articles, MC2 gets Russia-specific ones. No student should see the same content in both courses.

---

## 3. PER-QUIZ ACTION TABLE — FINAL QUIZ COMPOSITIONS

Every item ID below uses the `pcb-item-` prefix. Listed as short UUIDs for readability.

### TOPIC 1: Kievan Rus & Mongol Yoke (NEW — CED 1.8/2.2)
**Action:** Create new topic node. New test ID needed.
**Video + Article:** Source Russia-specific content on Kievan Rus, Byzantine influence, Mongol Golden Horde, Moscow's rise.
**Target: 10 MCQ + 1 SAQ**

**ALL 10 ITEMS — source from prep books + AP Classroom:**

| # | Source | Book | Location | Topic |
|---|--------|------|----------|-------|
| 1 | Princeton 2024 | Practice Test 5 (p06-c03) | Q19 | Mongol control comparison — Russia vs China |
| 2 | Princeton 2024 | Practice Test 6 (p06-c04) | Q1 | Mongols invading central Asia — mentions Russia |
| 3 | Princeton 2024 | Practice Test 6 (p06-c04) | Q19 | Mongol rule of Russia vs China |
| 4 | Princeton 2024 | Practice Test 4 (p06-c02) | Q7 | Mongol/Marco Polo — Mongol Empire context |
| 5 | Princeton 2024 | Practice Test 4 (p06-c02) | Q10 | Mongol Empire — political structures |
| 6 | Princeton 2024 | Practice Test 4 (p06-c02) | Q11 | Mongol Empire — cultural exchange |
| 7 | Barron's 2024 | Practice Test 2 (54_Practice02-01.xhtml) | Q21 | Mongol expansion map — political outcomes |
| 8 | Barron's 2024 | Practice Test 2 (54_Practice02-01.xhtml) | Q22 | Mongol expansion — Confucianism/Islam/Orthodox spread |
| 9 | AP Classroom | Unit 1 topic bank | CED 1.8 | Source 1 Q on Kievan Rus / Byzantine influence on Russia |
| 10 | AP Classroom | Unit 1 topic bank | CED 1.8 | Source 1 Q on Orthodox Christianity in Russia |

**SAQ:** AP Classroom — SAQ on Byzantine/Mongol influence on Russian political development (CED 1.8/2.2)

---

### TOPIC 2: Russian Empire & Tsardom (Combined from 3.1 + 3.2 + 3.3)
**Use Test ID from 3.1:** `pcb-resource-729d5633d2c74682ab8761c0b9779bd7` (repurpose)
**Current KEEP: 3 (3.1) + 2 (3.2) + 2 (3.3) = 7 → add 3 from prep books to reach 10**

**FINAL 10 ITEMS IN MCQ PRACTICE:**

**7 KEEP items from current quizzes:**

| # | Item ID | From | Stem (first 80 chars) |
|---|---------|------|-----------------------|
| 1 | `62885142` | 3.1 | Cossack communities — map of Russian frontiers |
| 2 | `b3f3bec0` | 3.1 | Russia's "possession of Baltic shore" — defeat of Sweden |
| 3 | `cbe66584` | 3.1 | Consequence of events in passage — birth of Russian Empire |
| 4 | `1000324e` | 3.2 | Russia 1450-1750 Source 1 — Peter the Great military/centralization |
| 5 | `3f6f5f4f` | 3.2 | Period 1450-1750 passage — Russia, growing absolute monarchy |
| 6 | `a545c715` | 3.3 | Beard policy Source 1 and 2 — Westernize Russia (Peter the Great) |
| 7 | `e3286635` | 3.3 | Peter the Great style of rule — absolute monarchy |

**3 NEW items — source from prep books:**

| # | Source | Book | Location | Topic |
|---|--------|------|----------|-------|
| 8 | Barron's 2024 | Ch 7 (Governance 1450-1750) | Search for Russia Q | Peter the Great / Russian expansion |
| 9 | Barron's 2024 | Ch 11 (Social 1450-1750) | Search for Russia Q | Serfdom / social hierarchy in Russia |
| 10 | Barron's 2024 | Ch 11 (Social 1450-1750) | Q17 | Qing/Manchu race-based hierarchy — compare with Russian serfdom |

**DELETE everything else from 3.1, 3.2, 3.3:**
- 3.1: DELETE 13 items (`b01798fe`, `ce96cff3`, `c3c7ef8b`, `68db220d`, `2e7476cf`, `2fd32f16`, `c436e1e1`, `24e37f90`, `168ab43a`, `840636e2`, `986a7e48`, `fdbea1f0`, `fe1dadfb`, `8cfa3dfc`, `47f8604b`) — 2 are old format, rest wrong topic
- 3.2: DELETE 18 items (`a72069a2`, `4ea25634`, `32bc05b8`, `d3a5c65b`, `544e18ef`, `7778d0d6`, `0661f660`, `98f24ad4`, `c4ddd3b4`, `6bd16da6`, `7341c0b7`, `bff23160`, `0c5e7fe0`, `55bcc53b`, `cb902bc5`, `76824f18`, `d3db294f`, `8d2adf65`, `634121c8`) — 1 old format, rest wrong topic
- 3.3: DELETE 5 items (`87c01fe0`, `f36b41f6`, `4ba58ef8`, `d6a6da11`, `d6fb515d`) — all wrong topic

**DELETE topic nodes:**
- `pcb-resource-a5847f4d738e4ba1b7a8600f4d3eb330` (3.2 Empires Admin) — items relocated
- `pcb-resource-6291f51f016d412cb82ead7562b09cb0` (3.3 Belief Systems) — items relocated

---

### TOPIC 3: Russian Industrialization (from 5.4 + 5.6)
**Use Test ID from 5.6:** `pcb-resource-700785c088f349c9a7505f80e977bc68` (repurpose)
**Current KEEP: 0 (5.4) + 6 (5.6) = 6 → add 4 from prep books to reach 10**

**FINAL 10 ITEMS IN MCQ PRACTICE:**

**6 KEEP items from Quiz 5.6:**

| # | Item ID | Stem (first 80 chars) |
|---|---------|----------------------|
| 1 | `c71f4453` | Japan Meiji and Soviet Union 1920s-30s industrialization comparison |
| 2 | `5bf3461c` | Russia industrialization 19c resembled Japan Meiji |
| 3 | `34b13ea9` | Russia 19c economic development pattern — passage |
| 4 | `2c950b54` | Russia 1890s rapid industrial output growth — Meiji Japan |
| 5 | `1fcf4741` | Russian Empire industrialization — new social classes |
| 6 | `c40d1999` | Japan vs Russia economic development comparison — state role |

**4 NEW items — source from prep books:**

| # | Source | Book | Location | Topic |
|---|--------|------|----------|-------|
| 7 | Barron's 2024 | Ch 15 (Governance 1750-1900) | Search for Russia Q | Crimean War / emancipation of serfs (1861) |
| 8 | Barron's 2024 | Ch 15 (Governance 1750-1900) | Search for Russia Q | Alexander II reforms / Witte industrialization |
| 9 | Barron's 2024 | Ch 17 (Social 1750-1900) | Search for Russia Q | Trans-Siberian Railway / labor conditions |
| 10 | Princeton 2024 | Ch 8 (Period 3 review) | Search for Russia Q | Russian industrialization under Witte |

**DELETE entire Quiz 5.4** (0 KEEP): all 16 items (`0652fefb`, `869ed6de`, `54e3b55b`, `cd78f1f9`, `66998d68`, `9c183976`, `91ab7149`, `c05621fa`, `40819d7d`, `437567c5`, `cf4c87f7`, `a650ca1f`, `b8ce35c9`, `8a592e81`, `b247d1ab`, `aefeaba9`)

**DELETE 20 wrong-topic items from Quiz 5.6:** `c89ea488`, `64d557c1`, `c89e92b8`, `49e4c0bb`, `3a01d51e`, `990f50f7`, `8932420c`, `5f64c61a`, `5dc16a40`, `33272e89`, `fb5e5f0b`, `c83d9d5d`, `20dba24e`, `afe29b9b`, `120fa38c`, `478ab1e7`, `664169ad`, `8e500851`, `17e22222`, `a4ff9cc6`

**DELETE topic node:** `pcb-resource-51dbe45f058a4775b5bdc54c80fd93b7` (5.4 Industrialization Spreads)

---

### TOPIC 4: Russian Reform & 1905 Revolution (NEW — CED 5.3/6.3)
**Action:** Create new topic node. New test ID needed.
**Video + Article:** Source Russia-specific content on populist movements, Russo-Japanese War, Bloody Sunday, 1905 Revolution, October Manifesto, Duma.
**Target: 10 MCQ + 1 SAQ**

**ALL 10 ITEMS — source from prep books + AP Classroom:**

| # | Source | Book | Location | Topic |
|---|--------|------|----------|-------|
| 1 | Barron's 2024 | Ch 15 (Governance 1750-1900) | Search for Russia Q | Populist movements / Narodniks |
| 2 | Barron's 2024 | Ch 15 (Governance 1750-1900) | Search for Russia Q | Russo-Japanese War consequences |
| 3 | Barron's 2024 | Ch 17 (Social 1750-1900) | Search for Russia Q | Russian peasant emancipation / social tensions |
| 4 | Barron's 2024 | Ch 19 (Governance 1900-1945) | Search for Russia Q | Pre-revolution reform attempts |
| 5 | Princeton 2024 | Ch 8 (Period 3 review) | Search for Russia Q | 1905 Revolution context |
| 6 | Princeton 2024 | Practice Test 3 (p06-c01) | Q28 | Japan defeated China — Russo-Japanese War comparison |
| 7 | Princeton 2024 | Practice Test 7 (p06-c05) | Q24 | Zamindars — compare with Russian serfdom/reform |
| 8 | AP Classroom | Unit 5 topic bank | CED 5.3 | Source 1 Q on Bloody Sunday / 1905 Revolution |
| 9 | AP Classroom | Unit 5 topic bank | CED 5.3 | Source 1 Q on October Manifesto / Duma |
| 10 | AP Classroom | Unit 6 topic bank | CED 6.3 | Source 1 Q on Alexander II reforms |

**SAQ:** AP Classroom — SAQ on causes of 1905 Revolution or Alexander II's reform legacy (CED 5.3/6.3)

---

### TOPIC 5: WWI & Russian Revolution (from Quiz 7.2)
**Use Test ID:** `pcb-resource-cf3daafe79674053add1bb42e1c22b51` (repurpose)
**Current KEEP: 7 (7.2) + 0 (7.5) = 7 → add 3 from prep books to reach 10**

**FINAL 10 ITEMS IN MCQ PRACTICE:**

**7 KEEP items from Quiz 7.2:**

| # | Item ID | Stem (first 80 chars) |
|---|---------|----------------------|
| 1 | `9503774d` | Most directly led to start of WWI — nationalist competition |
| 2 | `26713f13` | Soviet poster — communism as political/economic system |
| 3 | `ce1c7051` | Soviet Union's view of nationalism vs Marx's communism |
| 4 | `dc716179` | Giolitti — Balkans consequences, European military alliances |
| 5 | `8ae20bce` | Russian troops mobilized against Austria-Hungary — Serbia |
| 6 | `c16f3a92` | Passage — role of rival great power alliances in WWI |
| 7 | `9b42eb09` | Wilhelm II assurances to Russia — nationalism fueled by media |

**3 NEW items — source from prep books:**

| # | Source | Book | Location | Topic |
|---|--------|------|----------|-------|
| 8 | Barron's 2024 | Ch 19 (Governance 1900-1945) | Search for Russia Q | February Revolution / abdication of Tsar |
| 9 | Barron's 2024 | Ch 19 (Governance 1900-1945) | Search for Russia Q | October Revolution / Bolsheviks / Lenin |
| 10 | Barron's 2024 | Ch 19 (Governance 1900-1945) | Search for Russia Q | Treaty of Brest-Litovsk |

**DELETE 12 wrong-topic items from Quiz 7.2:** `308ced79`, `40e24ce7`, `ed76af15`, `16c7024d`, `44a179d1`, `f60568b1`, `96e8feea`, `26bf4fa6`, `5c80e6d5`, `4289022e`, `fe0c7d45`, `a50040d9`

**DELETE entire Quiz 7.5** (0 KEEP): all 12 items (`80a3802f`, `cb583b97`, `e5c36a2f`, `571cc949`, `5c0220f8`, `f4463784`, `727088a0`, `1f9021b3`, `f91f756e`, `2a8e78a4`, `2ab0c65f`, `6e9a20dc`)

**DELETE topic node:** `pcb-resource-1f06c2d384104b8ab23a736b65df2a83` (7.5 Unresolved Tensions)

---

### TOPIC 6: Soviet Union & Stalin (from Quiz 8.1)
**Use Test ID:** `pcb-resource-4526e6d16ce1477796e869746fd9db7e` (repurpose)
**Current KEEP: 7 (8.1) → add 3 from prep books to reach 10**

**FINAL 10 ITEMS IN MCQ PRACTICE:**

**7 KEEP items from Quiz 8.1:**

| # | Item ID | Stem (first 80 chars) |
|---|---------|----------------------|
| 1 | `d333f921` | Soviet image central purpose — Five Year Plan, women liberation |
| 2 | `e3fe1c5b` | Image context — collectivization of farms (Soviet) |
| 3 | `9832982e` | Image contrasts Soviet policy — Five Year Plan resistance |
| 4 | `0ed0deb9` | Soviet advertising — rise as major technological power |
| 5 | `71f6a765` | WWII photograph connected to Cold War — Soviet/US |
| 6 | `1796ff2d` | Image WWII and Cold War — ideological differences |
| 7 | `b62bf12e` | Image — shift in global balance of power (WWII/Cold War) |

**3 NEW items — source from prep books:**

| # | Source | Book | Location | Topic |
|---|--------|------|----------|-------|
| 8 | Barron's 2024 | Ch 19 (Governance 1900-1945) | Search for Russia Q | Stalin's rise / purges |
| 9 | Barron's 2024 | Ch 23 (Economics) | Q16 | Trade agreements with Russia/China |
| 10 | Barron's 2024 | Ch 25 (Environment) | Q16 | Famines from gov't policy — China and USSR |

**DELETE 10 wrong-topic items from Quiz 8.1:** `a0fe9049` (5-choice), `9f99a82d`, `2b7500f8`, `75613a8d`, `c55e5b14`, `641f4405`, `51f727c4`, `1c35cd43`, `4e5e21e8` (5-choice), `2d75e572`, `a90dfebb`, `29464651`

---

### TOPIC 7: Cold War Soviet Union (from 8.2 + 8.3 + 8.4)
**Use Test ID from 8.2:** `pcb-resource-f9d28bfb5d614d6ea75fca9c5dc4c92c` (repurpose)
**Current KEEP: 18 (8.2) + 14 (8.3) + 5 (8.4) = 37 → select best 10, move overflow to Mini MCQ**

**FINAL 10 ITEMS IN MCQ PRACTICE:**

| # | Item ID | From | Stem (first 80 chars) |
|---|---------|------|-----------------------|
| 1 | `200314bf` | 8.2 | Principal cause of Cold War — conflicting ideologies |
| 2 | `53c46bad` | 8.2 | Cold War rivalry — ideology and economic structure |
| 3 | `761138f4` | 8.2 | Khrushchev "two social-political systems" — dem cap vs communism |
| 4 | `a5a10004` | 8.2 | Kennan recommendation — Soviet ideological dominance |
| 5 | `dd09ef2e` | 8.2 | Kennan passage purpose — influence US containment policy |
| 6 | `a204c50d` | 8.2 | Stalin vs Khrushchev mode of rule — contrast |
| 7 | `4a0ec231` | 8.2 | Khrushchev document — thaw in Soviet social/political life |
| 8 | `5fc9357d` | 8.3 | NATO established 1949 — counter Soviet threat |
| 9 | `34ac1902` | 8.3 | Angolan Civil War — Cold War proxy conflicts |
| 10 | `3dcc0d59` | 8.3 | Soviet Union motivation in Congo — expand influence |

**MOVE TO MINI MCQ (14 items — overflow from 37):**

| Item ID | From | Stem snippet |
|---------|------|-------------|
| `8af2a8e0` | 8.4 | Chart — state-directed modernization campaigns (Soviet) |
| `062b0cc6` | 8.4 | "Cruel repression" — secret police, summary trials (Soviet) |
| `5070c5be` | 8.2 | Soviet undertaking projects — keeping pace |
| `971da32f` | 8.2 | US and Soviet emerged as superpowers |
| `0a7e21a1` | 8.2 | NATO — prevent spread of communism |
| `42ebf21b` | 8.2 | Kennan historical circumstances — Soviet defeat of Nazis |
| `02f4d778` | 8.2 | Kennedy and Khrushchev — nuclear war devastating |
| `c8780cb2` | 8.2 | Cold War 1950s — Soviet rocket technology |
| `1b95e354` | 8.3 | Total war not rational — nuclear weapons, proxy wars |
| `82d035ee` | 8.3 | Nuclear powers military capabilities — limitations |
| `1523b3c3` | 8.3 | Confrontation photographs — NATO and Warsaw Pact |
| `7e97c447` | 8.3 | Nuclear weapons 1945-1985 — Western vs communist |
| `d6288fa9` | 8.4 | Russian/Soviet literacy rates — rural peasantry benefited |
| `fb756ce4` | 8.4 | Soviet communism chart — revolution improved literacy |

**DELETE remaining items from 8.2, 8.3, 8.4 (not selected for quiz or Mini MCQ):**

From 8.2: `5975bfef`, `f7c34d7e`, `57806d4b`, `0394d190`, `9b201ea0`, `55e1fa95`
From 8.3: `cef70de8`, `fc212637`, `56fcd372`, `75cc7477`, `e5e97881`, `16126a63`, `15dbb6e2`, `66ed922b`, `e8103130`, `1a271ef5`, `3fc2ef5a`, `0b90939d`, `f6d5b3c8`, `186759fe`
From 8.4: `38a79d51`, `928603c9`, `da1f0bbc`, `ef128f84`, `00177f2b`, `5d67f1ae`, `c89704fb`, `7e1a7daf`, `8d86f576`, `6fce88f8`, `100d660d`, `0449573e`

**DELETE topic nodes:**
- `pcb-resource-3513d67d3e354167837d588dc4373966` (8.3 Effects of CW) — items relocated
- `pcb-resource-7178ea54cf49496d9022dd669f52afb1` (8.4 Spread of Communism) — items relocated

---

### TOPIC 8: Fall of USSR & End of Cold War (from Quiz 8.8)
**Use Test ID:** `pcb-resource-3916af733cec480b921543dda17d7393`
**Current KEEP: 13 → trim to 10**

**FINAL 10 ITEMS IN MCQ PRACTICE:**

| # | Item ID | Stem (first 80 chars) |
|---|---------|----------------------|
| 1 | `1bbe757e` | Author POV — collapse of communism in Eastern Europe |
| 2 | `087933ef` | Major change 1980s-90s — reduction communist vs capitalist |
| 3 | `2642d7c6` | End of political order on map — Soviet military/economic |
| 4 | `eea5fa81` | Passage 1970s-80s — liberalization of Soviet politics |
| 5 | `6bb1c558` | Havel — grassroots citizens organizations, communist bloc |
| 6 | `aed74e3e` | End of Cold War hastened by — EXCEPT arms control treaties |
| 7 | `a927ba1d` | Soviet Union images — rising public discontent |
| 8 | `a99562ef` | Soviet trucks Image 2 — free-market reforms failing |
| 9 | `d2c02cdc` | Soviet leaders power display — Afghanistan expensive failure |
| 10 | `6d3ce256` | US vs Russia CO2 trends 1990-2000 — Soviet economic collapse |

**MOVE TO MINI MCQ (3 items):**
- `e643b93b` — Collapse of Soviet communist regime — end of Cold War
- `5b10b6d9` — Expensive military competition — collapse of Soviet Union
- `c941586a` — Long-term cause collapse Soviet Union — cost of arms race

---

### MINI MCQ PRACTICE QUIZ — FULL REBUILD
**Current Test ID:** `pcb-resource-3644c663ac044b00b745e1d79a890eaa`
**Current: 25 items (11 duplicates, 7 wrong topic, 6 KEEP) → DELETE ALL 25, rebuild from scratch**

**DELETE all 25 current items:**
`b91e520c`, `d04b8d7a`, `1889a62f`, `f7aabed7`, `60a7efb9`, `1115891c`, `9e1206a6`, `afcc1c54`, `f9a8d0af`, `08a8543e`, `e4d2d7e6`, `f1bf4899`, `fabd9c95`, `a8c6d763`, `0146d850`, `480bf7ed`, `6e7fadec`, `2300cb72`, `46851162`, `b816e54e`, `d742f8a5`, `8eb7c6e0`, `e7f1d917`, `c0ee770a`, `551e887b`

**NEW 24-item end-of-course Mini MCQ — 3 items per topic (mixed review):**

> **Note:** The Mini MCQ below is for cumulative mixed-topic review at end of course. The per-topic MCQ Practice (10 Qs each) is the main assessment per topic.


| Topic | Item Source | Details |
|-------|------------|---------|
| **T1: Kievan Rus** (3) | Source from Barron's PT2 Q42-Q43 (mandate of heaven — cross-cultural); AP Classroom CED 2.2 ×1 | Mongol impact on Russia |
| **T2: Russian Empire** (3) | `b91e520c` (Europe map nationalist unification), `1889a62f` (Moscow Orthodox center), source 1 from Barron's Ch 7 | Peter the Great / Catherine |
| **T3: Industrialization** (3) | Source from Barron's Ch 23 Q19 (free-market reforms China vs Soviet); Princeton PT5 Q15 (Industrial Rev textile); AP Classroom CED 5.4 ×1 | Russian industrial development |
| **T4: 1905 Revolution** (3) | Source from AP Classroom CED 5.3 ×2, CED 6.3 ×1 | Reform movements / Bloody Sunday |
| **T5: WWI & Revolution** (3) | `d04b8d7a` (WWI troops collapse), `f9a8d0af` (Soviet poster), source 1 from Barron's Ch 19 | Russian Revolution |
| **T6: Soviet/Stalin** (3) | `e4d2d7e6` (Soviet collectivization), `a8c6d763` (Chinese vs Soviet programs), source 1 from Barron's Ch 24 Q2 (China/Russia post-Cold War) | Five-Year Plans / collectivization |
| **T7: Cold War** (3) | `5070c5be` (Soviet projects), `02f4d778` (Kennedy/Khrushchev nuclear), `82d035ee` (nuclear capabilities) | From Topic 7 overflow |
| **T8: Fall of USSR** (3) | `c941586a` (arms race cost), source 2 from Barron's Ch 23 Q16 (trade agreements), Princeton Ch 9 Q4 | Gorbachev / dissolution |

**Spec:** All 24 must be 4-choice, all stimulus-based, no duplicates with topic quizzes.
**Difficulty mix:** ~5 easy (20%), ~12 medium (50%), ~7 hard (30%).

---

### FRQ / SAQ PRACTICE — DELETE ALL CURRENT, REBUILD
**Current Test ID:** `2ce28f90-438d-402a-b340-05156fe801ae`
**DELETE all 3 current items:** `qti-item-01`, `qti-item-02`, `qti-item-03` — none are Russia-specific.

---

## 4. 5-CHOICE QUESTIONS — DELETE ALL 11

These are old pre-2011 AP format. Action: DELETE the question entirely (not "remove 5th choice"). Source a 4-choice replacement from AP Classroom for the same CED topic.

| # | Item ID (full) | Current Quiz | Stem (first 80 chars) |
|---|----------------|--------------|----------------------|
| 1 | `pcb-item-2e7476cf` | 3.1 Empires Expand | States that dominated Mediterranean trade 16th century |
| 2 | `pcb-item-24e37f90` | 3.1 Empires Expand | Russia emerging as expanding Eurasian power 1450-1750 |
| 3 | `pcb-item-7341c0b7` | 3.2 Empires Admin | St. Petersburg cityscape — Westernization |
| 4 | `pcb-item-cd78f1f9` | 5.4 Ind. Spreads | European predominance world economy 19c (dup of `54e3b55b`) |
| 5 | `pcb-item-91ab7149` | 5.4 Ind. Spreads | Japanese women during industrialization |
| 6 | `pcb-item-c89ea488` | 5.6 Gov't Role | Meiji reformers policies in Japan |
| 7 | `pcb-item-3a01d51e` | 5.6 Gov't Role | Societies resisting foreign penetration 1650-1850 |
| 8 | `pcb-item-8e500851` | 5.6 Gov't Role | Russia and Japan by 1914 — state-sponsored |
| 9 | `pcb-item-a0fe9049` | 8.1 Setting Stage | Rapid economic growth during WWII |
| 10 | `pcb-item-4e5e21e8` | 8.1 Setting Stage | NOT a consequence of WWII |
| 11 | `pcb-item-8d86f576` | 8.4 Spread of Communism | Chinese peasant women 1940s-50s — Maoist policies |

**Note:** Items `24e37f90` and `8e500851` are Russia-relevant but old format. DELETE them and source 4-choice replacements covering the same content from AP Classroom.

---

## 5. FRQ RESTRUCTURE

### DELETE current 3 FRQs

| Item ID | Problem |
|---------|---------|
| `qti-item-01` | Generic SAQ — not Russia-specific |
| `qti-item-02` | Generic SAQ — not Russia-specific |
| `qti-item-03` | Ethnic divisions in empires — generic, not Russia |

**Delete test:** `2ce28f90-438d-402a-b340-05156fe801ae`

### ADD: New FRQ structure

| Type | Placement | Count | Source |
|------|-----------|-------|--------|
| **SAQ** | After EACH topic MCQ Practice | 8 total (1 per topic) | AP Classroom released SAQs matching each topic's CED |
| **LEQ** | End of course | 1 (2-3 prompt choices) | See sourcing below |
| **DBQ** | End of course | 1 | See sourcing below |

### LEQ Sourcing — pick ONE or offer 2-3 as prompt choices:

| Option | Prompt | Period | Source |
|--------|--------|--------|--------|
| A | "Evaluate the extent to which Russian rulers' attempts to modernize Russia changed Russian society in the period 1700-1917." | Units 3-6 | Compose based on released AP exam LEQ format |
| B | "In the period 1750 to 1900, economic globalization widened the scope of migration... Evaluate how industrialization transformed Russian and Japanese societies." | Units 5-6 | Adapted from Barron's 2024 PT1 Q3 (Chinese/Indian migration) — swap for Russia/Japan focus |
| C | "In the period 1900-present, communist revolutions transformed multiple societies. Evaluate the extent to which the Russian Revolution achieved its stated goals." | Units 7-8 | Compose based on released AP exam LEQ format |

**Recommendation:** Use Option C (covers Units 7-8, directly relevant to student gaps — Jackson U7: 50%, U8: 49%).

### DBQ Sourcing:

| Option | Prompt | Period | Source |
|--------|--------|--------|--------|
| A | "Evaluate the extent to which Soviet economic policies transformed Russian society in the period 1917-1945." (7 documents) | Units 7-8 | Compose using primary sources from Five-Year Plans, collectivization, purges |
| B | "Evaluate the causes and consequences of the Russian Revolution of 1917." (7 documents) | Unit 7 | AP Classroom / released exam DBQ bank |

**Recommendation:** Use Option B — Russian Revolution is the most tested Russia topic on AP exams.

### SAQ sourcing per topic:

| Topic | SAQ Source | CED |
|-------|-----------|-----|
| T1: Kievan Rus | AP Classroom SAQ bank, CED 1.8/2.2 | Byzantine/Mongol influence |
| T2: Russian Empire | AP Classroom SAQ bank, CED 3.1/3.2 | Peter the Great reforms |
| T3: Industrialization | AP Classroom SAQ bank, CED 5.4/5.6 | State-led industrialization |
| T4: 1905 Revolution | AP Classroom SAQ bank, CED 5.3/6.3 | Reform movements |
| T5: WWI & Revolution | Barron's 2024 PT1 SAQ (adapted for Russia) | 7.2/7.5 |
| T6: Soviet/Stalin | AP Classroom SAQ bank, CED 8.1 | Five-Year Plans |
| T7: Cold War | AP Classroom SAQ bank, CED 8.2/8.3 | Arms race / proxy wars |
| T8: Fall of USSR | AP Classroom SAQ bank, CED 8.8 | Gorbachev / dissolution |

### Target course structure per topic

```
Topic X: Video → Article → MCQ Practice (10 MCQ) → SAQ (1-2 questions)
```

### End of course

```
Mini MCQ Practice Quiz (24 Qs, 3 per topic, even distribution)
LEQ Practice (2-3 prompt choices spanning different periods)
DBQ Practice (7 docs, full AP format, Russia-specific)
```

---

## 6. ENGINEERING FIXES

### E-1: PP100 → Regular Quiz

All test IDs below need PP100 flag removed and converted to regular quiz format:

| Test ID | Current Topic |
|---------|-------------|
| `pcb-resource-729d5633d2c74682ab8761c0b9779bd7` | 3.1 Empires Expand |
| `pcb-resource-a5847f4d738e4ba1b7a8600f4d3eb330` | 3.2 Empires Admin |
| `pcb-resource-6291f51f016d412cb82ead7562b09cb0` | 3.3 Belief Systems |
| `pcb-resource-51dbe45f058a4775b5bdc54c80fd93b7` | 5.4 Ind. Spreads |
| `pcb-resource-700785c088f349c9a7505f80e977bc68` | 5.6 Gov't Role |
| `pcb-resource-cf3daafe79674053add1bb42e1c22b51` | 7.2 Causes of WWI |
| `pcb-resource-1f06c2d384104b8ab23a736b65df2a83` | 7.5 Unresolved Tensions |
| `pcb-resource-4526e6d16ce1477796e869746fd9db7e` | 8.1 Setting Stage |
| `pcb-resource-f9d28bfb5d614d6ea75fca9c5dc4c92c` | 8.2 The Cold War |
| `pcb-resource-3513d67d3e354167837d588dc4373966` | 8.3 Effects of CW |
| `pcb-resource-7178ea54cf49496d9022dd669f52afb1` | 8.4 Spread of Communism |
| `pcb-resource-3916af733cec480b921543dda17d7393` | 8.8 End of Cold War |
| `pcb-resource-3644c663ac044b00b745e1d79a890eaa` | Mini MCQ |
| `2ce28f90-438d-402a-b340-05156fe801ae` | FRQ/SAQ |

### E-2: Missing Stimuli

1 KEEP item has a stimulus concern. Verify on live platform.

| Item ID (full) | Quiz | Issue |
|-----------------|------|-------|
| `pcb-item-1b95e354` | Effects of CW | Passage embedded in stem (no `stimulus_id`) — verify renders correctly |

(4 other items with missing stimuli are all being deleted for wrong topic.)

### E-3: Duplicates

12 items in Mini MCQ are exact duplicates. All resolved by Mini MCQ full rebuild (all 25 current items deleted).

| Duplicate (Mini MCQ) | Original (Topic Quiz) |
|----------------------|----------------------|
| `480bf7ed` | `a545c715` |
| `cd78f1f9` | `54e3b55b` |
| `6e7fadec` | `66998d68` |
| `2300cb72` | `34b13ea9` |
| `c0ee770a` | `2c950b54` |
| `551e887b` | `1fcf4741` |
| `46851162` | `8ae20bce` |
| `b816e54e` | `f91f756e` |
| `e7f1d917` | `e3fe1c5b` |
| `d742f8a5` | `75cc7477` |
| `08a8543e` | `e8103130` |
| `8eb7c6e0` | `6bb1c558` |

---

## 7. PRIORITY ORDER

### Phase 1: Immediate Engineering Fixes (~2 hours)

| # | Task | Items Affected | Time |
|---|------|----------------|------|
| 1a | DELETE 11 five-choice questions (see Section 4) | 11 items | 20 min |
| 1b | PP100 → regular quiz for all 14 test IDs (see E-1) | 14 tests | 30 min |
| 1c | DELETE 3 FRQs from test `2ce28f90-438d-402a-b340-05156fe801ae` | 3 items | 10 min |
| 1d | DELETE all 25 Mini MCQ items (duplicates + wrong topic) | 25 items | 20 min |
| 1e | Verify 1 stimulus item (`1b95e354`) on live | 1 item | 5 min |

### Phase 2: Topic Cleanup (~4 hours)

| # | Task | Items Affected | Time |
|---|------|----------------|------|
| 2a | DELETE wrong-topic items from all 12 quizzes | 121 items | 2 hrs |
| 2b | COMBINE 3.1+3.2+3.3 into Topic 2, relocate 7 KEEP items | 7 KEEP + 36 DELETE | 1 hr |
| 2c | COMBINE 5.4+5.6 into Topic 3, relocate 6 KEEP items | 6 KEEP + 36 DELETE | 30 min |
| 2d | Filter 8.2+8.3+8.4 into Topic 7, select 12, move 12 to Mini MCQ | 12 quiz + 12 Mini MCQ | 30 min |
| 2e | DELETE topic nodes 3.2, 3.3, 5.4, 7.5, 8.3, 8.4 | 6 topics | 15 min |

### Phase 3: Structural Rebuild — Source from Prep Books (~8 hours)

**Prep book EPUBs location:** `/tmp/apwh_prep/World History/`
**AP Classroom:** Use topic banks for gaps

| # | Task | Source | Qs to Scrape | Time |
|---|------|--------|-------------|------|
| 3a | BUILD Topic 1: Kievan Rus (Video + Article + 10 MCQ + SAQ) | Princeton PT4-6 (Mongol Qs), Barron's PT2, AP Classroom ×2 | 10 Qs | 2 hrs |
| 3b | ADD 3 new Qs to Topic 2 (Russian Empire) | Barron's Ch 7, Ch 11 | 3 Qs | 15 min |
| 3c | ADD 4 new Qs to Topic 3 (Industrialization) | Barron's Ch 15, Ch 17; Princeton Ch 8 | 4 Qs | 20 min |
| 3d | BUILD Topic 4: 1905 Revolution (Video + Article + 10 MCQ + SAQ) | Barron's Ch 15, Ch 17, Ch 19; Princeton Ch 8, PT3 Q28; AP Classroom ×3 | 10 Qs | 2 hrs |
| 3e | ADD 3 new Qs to Topic 5 (WWI & Revolution) | Barron's Ch 19 | 3 Qs | 15 min |
| 3f | ADD 3 new Qs to Topic 6 (Soviet/Stalin) | Barron's Ch 19, Ch 23, Ch 25 | 3 Qs | 15 min |
| 3g | ADD SAQs after all 8 topic quizzes | AP Classroom SAQ bank per CED topic | 8 SAQs | 1 hr |
| 3h | Replace 12 shared resource IDs with Russia-specific video/article content | New Russia-specific content | 12 resources | 1 hr |

### Phase 4: Mini MCQ & FRQ

| # | Task | Source |
|---|------|--------|
| 4a | REBUILD Mini MCQ (24 Qs, 3 per topic, mixed) | Overflow from topic MCQ Practice + prep books |
| 4b | ADD LEQ at end of course | Compose Russia-specific or adapt from released exam |
| 4c | ADD DBQ at end of course (Russian Revolution or Soviet economic policy) | AP Classroom / released exam DBQ bank |

### Total estimated time: ~17 hours across 4 phases

**Phase 1 is unblocked — start immediately.**
Phase 2 can start after Phase 1.
Phase 3 requires scraping prep book EPUBs at `/tmp/apwh_prep/World History/` and AP Classroom access.
Phase 4 depends on Phase 3 (Mini MCQ needs topic quiz items finalized first).

---

## 8. REBUILT COURSE SUMMARY

| Component | Items | Source |
|-----------|-------|--------|
| Topic 1: Kievan Rus & Mongol Yoke ★ | 10 MCQ Practice + 1 SAQ | 8 from Princeton/Barron's + 2 AP Classroom |
| Topic 2: Russian Empire & Tsardom | 10 MCQ Practice + 1 SAQ | 7 existing + 3 from prep books |
| Topic 3: Russian Industrialization | 10 MCQ Practice + 1 SAQ | 6 existing + 4 from prep books |
| Topic 4: Russian Reform & 1905 Revolution ★ | 10 MCQ Practice + 1 SAQ | 7 from prep books + 3 AP Classroom |
| Topic 5: WWI & Russian Revolution | 10 MCQ Practice + 1 SAQ | 7 existing + 3 from prep books |
| Topic 6: Soviet Union & Stalin | 10 MCQ Practice + 1 SAQ | 7 existing + 3 from prep books |
| Topic 7: Cold War Soviet Union | 10 MCQ Practice + 1 SAQ | 10 existing (best from 37 KEEP) |
| Topic 8: Fall of USSR | 10 MCQ Practice + 1 SAQ | 10 existing (from 13 KEEP) |
| Mini MCQ Practice Quiz (end of course) | 24 MCQ | 3 per topic, mixed review |
| LEQ | 1 prompt | Compose Russia-specific |
| DBQ | 1 prompt (7 docs) | AP Classroom / released exam |
| **TOTAL** | **80 MCQ Practice + 24 Mini MCQ + 8 SAQ + 1 LEQ + 1 DBQ = 114 items** | |

★ = New topic (needs video + article + MCQ practice + SAQ)

**Net change:** 235 items → 114 items. Leaner, 100% Russia/Soviet-specific.

---

*Generated 2026-03-20. Source data: `question_classification.md`, `02_course_tree.json`, `russia_questions_available.md`, plan `piped-kindling-falcon.md`.*
