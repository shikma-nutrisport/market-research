# CLAUDE.md: Koach Moach (כוח מוח) market research

This repository holds a market-research project for Koach Moach, a monthly employee-wellbeing program of short body-and-brain games that working parents play at home with their children aged 5-12.

This file is the single source of truth. PART 1 says how to run the research. PART 2, in Hebrew, is the research base: the product brief, hypotheses, starting competitor list, seed papers and starting keywords. Ignore README.md and any older brief or prompt in the repository.

---

# PART 1: HOW TO RUN

## Run mode

- Talk to me in Hebrew.
- Run the whole workflow below, step by step, through step 5. Start from the first step that PROGRESS.md does not mark as done, or from step 1 if PROGRESS.md does not exist.
- Work autonomously. Do not ask me questions, and do not stop between steps to ask whether to continue. Stop only when step 5 is done, or when you are truly blocked (see "If you are blocked").
- Work on one item at a time (one step, one competitor group, one paper) and save it to its file right away. Rely on the files, not on your memory of earlier steps.
- After every step, and after every single paper in step 4: update PROGRESS.md, commit and push. Use short English commit messages, like "Step 2A: competitors part 1".

## PROGRESS.md

Create it at the start if it does not exist. Keep it short:
- First line: the branch name you are pushing to.
- One line per step: step, status (done / partial / not started), files written, date.
- A short list of anything blocked, or marked "לא אומת", that needs my attention.

A new session reads this file first and continues from where the last one stopped.

## If you are blocked

- If websites are blocked by network restrictions (you cannot open PubMed, Europe PMC or company sites), write that at the top of PROGRESS.md, push, tell me in one Hebrew line to change this environment's network access to Full, and stop.
- If a single site, product or paper fails, mark it "לא אומת" and move on. Never stop the run for one item.

## Rules for every step

1. **Language:** write all analysis, summaries and tables in Hebrew. Keep company names, product names, paper titles and search terms in English.
2. **Verify with live sources.** Check every company, product, price, paper and number on the web. Put the source URL next to each fact. If you cannot verify something, write "לא אומת" next to it. Never guess, and never invent names, numbers, links, quotes or effect sizes.
3. **Keep three kinds of statements apart:** what you verified now (with a link), what comes from PART 2 of this file, and your own inference (mark it "הערכה").
4. **Numbers from papers come only from the paper itself.** If you could read only the abstract, say so, and do not add numbers that are not in it.
5. **Open access only.** Never bypass paywalls. If an open-access PDF downloads directly, save it to 04-papers/pdfs/Author_Year.pdf. If not, keep the link and move on; do not spend time on it.
6. **Short tables over long prose.**
7. **The Koach Moach column** in any comparison is filled only from PART 2. Do not add features that are not there.

---

## WORKFLOW

### STEP 1. KEYWORDS → 01-keywords/keywords.md
No web search in this step.
Start from the keyword list in section 12 of PART 2. It is a starting list of search terms, not instructions. Build 60-100 English search terms in four groups:
- A. Product and category (finding competitors)
- B. Employer side (finding B2B competitors)
- C. Science (finding papers), including MeSH terms
- D. Market (size and trends)

Add synonyms, MeSH terms and the product-category names that app stores and industry analysts actually use. Cover all three parts of the product: movement, the cognitive challenge, and the mental part (short pause, breathing, body awareness, mindful movement). Tag each term [competitors], [papers] or [market]. Mark MeSH terms "MeSH, to verify".
Then add:
- E. 10-15 Hebrew search terms for finding Israeli employee-wellbeing providers and family programs.
- F. 3 ready-to-use PubMed queries (Boolean, with field tags) for step 4, building on the sample query in section 12.

Format: a compact list per group, one term per line with its tag.

### STEP 2A. MARKET SCAN, PART 1 → 02-competitors/competitors-part1.md
Cover two groups:
1) family or parent-child movement games and apps
2) cognitive-motor or brain-body training for kids, including mindful-movement products for kids

Start with the relevant names in section 10 of PART 2, then use the [competitors] keywords from step 1 to find more. Aim for 12-16 products across the two groups. For each one, open its official site or app store page and check that it is active in 2026. If you cannot confirm that, keep it in the table and write "לא אומת".

One Markdown table with these columns:
Name | URL | Category (1/2) | Group (Direct / Indirect / Substitute) | What it does | Who pays | Ages | Price model | Parent-child co-play (Yes/Partial/No) | Cognitive challenge inside the movement (Yes/Partial/No) | Sold to employers (Yes/No) | Hebrew (Yes/No) | Source + date checked

Keep each cell short, up to 12 words.

### STEP 2B. MARKET SCAN, PART 2 → 02-competitors/competitors-part2.md and 02-competitors/summary.md
Cover two more groups:
3) employer-paid family or kids wellbeing programs, and corporate wellness challenge platforms (include Personify Health, YuMuuv, Vantage Fit and Mightier)
4) Israeli employee-wellbeing providers that serve families: digital platforms, workshop and lecture providers, family fun days, camps for employees' children. Search in Hebrew with the group E terms from step 1.

Aim for 10-14 more. Same columns and same verification rule as step 2A.

Then write 02-competitors/summary.md in Hebrew, 5-8 lines:
- The 3-4 closest competitors across both tables, and why.
- Does any of them combine all three: parent-child co-play, a cognitive challenge inside the movement, and sales to employers? Answer yes or no first, then the evidence. If yes, say what that means for our differentiation.
- One pattern in how Israeli employers buy family-facing wellbeing (price, budget source, timing). Mark it "הערכה" if it is an inference.

### STEP 3. DEEP COMPARISON → 03-comparison/comparison.md
Compare: Active Arcade, Nex Playground, Kid Motion Coach, GoNoodle, Mightier, and our product "Koach Moach".
Active Arcade and Nex Playground come from the same company (Nex). Treat them as two products with different business models. If step 2 found a closer competitor, swap one of the five for it and explain why in one line.
For each competitor use the official site, the app store page, and 2-3 user reviews from 2025-2026 (app store reviews, Trustpilot, Reddit or independent reviews).

One Markdown table, one column per product, with these rows:
1. Target user and children's ages
2. How parent and child play together
3. Cognitive challenge inside the movement
4. Session length
5. Equipment needed
6. Feedback on performance (camera / self-report / none)
7. Price and who pays
8. Sales channel (consumer / school / employer / health plan)
9. What they promise, and what evidence they cite
10. Children's privacy approach
11. Hebrew support
12. Top 3 strengths
13. Top 3 weaknesses, from user reviews
14. What Koach Moach does differently

Keep each cell up to 25 words. Put footnote numbers like [1] in the cells and list the source URLs under the table.

Below the table, in Hebrew:
- a. The market gap none of them covers (3-5 lines).
- b. One specific thing to copy or learn from each competitor.
- c. One strategic risk each competitor poses to Koach Moach.
- d. Three lines I can paste into a sales page under "במה אנחנו שונים", with no claim we cannot support.

### STEP 4A. EVIDENCE REVIEW, SEED PAPERS 1-6 → 04-papers/summaries/Author_Year.md
Work on ONE paper at a time, in this order, using the table in section 11 of PART 2:
1. Diamond & Lee 2011
2. Vazou et al. 2016/2019 (check whether 2016 and 2019 are the same paper)
3. Mao et al. 2024
4. Schmidt, Benzing & Kamer 2016
5. Egger et al. 2019
6. Benzing et al. 2016

Open the paper itself (PubMed, PubMed Central, Europe PMC, publisher open access). For each paper write, in Hebrew:
- Full citation, link, open access (yes/no)
- Research question
- Who: ages, number of participants, setting (school / home / lab)
- What was done: type of activity, minutes per session, sessions per week, number of weeks
- Compared to what
- Main results, with effect sizes as reported
- The bottom line in one sentence
- Limitations
- Evidence level (meta-analysis / systematic review / RCT / observational / pilot)
- Fit to Koach Moach: how far the ages, the setting and the dose are from a 10-minute parent-child session at home
- What Koach Moach MAY say in B2B marketing based on this paper (1-2 ready-to-use sentences)
- What Koach Moach may NOT say (1-2 examples)

Commit and push after each paper.

### STEP 4B. EVIDENCE REVIEW, SEED PAPERS 7-12 → 04-papers/summaries/Author_Year.md
Same format and the same one-paper-at-a-time rule as step 4A, for:
7. Brown et al. 2016
8. Flanders et al. 2009, plus the 5-year follow-up abstract linked in PART 2
9. Loy, O'Connor & Dishman 2013 (find the journal article, not only the dissertation)
10. Physical activity context and cognition across the lifespan, 2025 (check the authors, the number of studies and the number of participants)
11. Family Move parent-child app pilot (PART 2 has two links, one from EdUHK and one from HKU; check which institution it is and whether both records are the same study)
12. The 2023 Frontiers in Psychology article on energy and fatigue (check what it actually says about sessions shorter than about 6 minutes, and whether it is a research paper or an opinion piece)

### STEP 4C. NEW PAPERS → 04-papers/summaries/new-papers.md
Search PubMed, Europe PMC and Semantic Scholar with the [papers] keywords and the PubMed queries from step 1, for up to 10 more papers from 2010-2026 that the seed list does not cover. Prefer meta-analyses, systematic reviews and RCTs with children aged 5-12, or with parent-child pairs. Look especially for:
- short (under 15 minutes) cognitively engaging activity, at home and not only in school
- parent-child or family co-activity and children's self-regulation or emotion regulation
- the mental part of the product: short pauses, breathing, body awareness or mindful movement for children
- acute exercise and energy, mood or cognition in working adults

For each new paper write a short version: citation and link, design, ages and number, dose, main result, bottom line, what we may say and what we may not. Include only papers you actually opened. Leave out any paper you cannot link to.

### STEP 4D. EVIDENCE TABLE AND BOTTOM LINES → 04-papers/evidence-table.md and 04-papers/bottom-lines.md
Use only the papers summarized in steps 4A-4C.

1. 04-papers/evidence-table.md, one table:
Paper | Year | Design | Ages | Setting | Dose (minutes x times per week x weeks) | Outcome | Effect | Bottom line | Open access | Link

2. 04-papers/bottom-lines.md, in Hebrew, 5-7 sentences, covering:
- a. children's attention
- b. self-regulation and emotional regulation
- c. parents' energy and mental performance
- d. the minimum session length and frequency the evidence points to

Address directly the gap between the dose in the studies and our format (about 10 minutes, at home, parent and child together). Say clearly what a 10-minute format can rely on (for example, acute effects) and what it cannot claim (for example, lasting change in executive functions), based on the papers.

Then, in the same file, two short lists: 5 claims we may use in B2B marketing, each with its paper, and 5 claims we must not use.

### STEP 5. EXECUTIVE SUMMARY → 00-summary.md
One page in Hebrew, about 500 words, that pulls together steps 1-4:
1. The market opportunity, in 3-4 sentences.
2. The top 3 competitive threats, and whether anyone already covers our three-part differentiation.
3. The scientific blueprint: what the evidence supports, the recommended session length and frequency, and what we may and may not claim.
4. The six hypotheses in section 5 of PART 2: one line each, marked supported / contradicted / still open, and what will settle it. Desk research is done; whatever is still open goes to my interviews with wellbeing managers and to the family pilot.
5. Three concrete changes to the product, the message or the price model that come out of this research.

End with relative links to all the detailed files.

**When step 5 is done:** update PROGRESS.md, commit and push. Then show me the full text of 00-summary.md here in the chat, and tell me the name of the branch that holds all the files.

---

# PART 2: RESEARCH BASE (בעברית)

> מה שכתוב כאן הוא נקודת פתיחה והשערות, לא עובדות מאומתות. כל שם, מחיר, מספר ומאמר צריך אימות מול מקור חי לפני שהוא נכנס לתוצרים.

## 1. המוצר

כוח מוח היא תוכנית רווחה חודשית לארגונים. היא נותנת לעובדים ולילדים שלהם דרך נוחה ופרקטית להתמיד באימונים קצרים וחוויתיים עם משימות מוחיות. כל אימון משלב משימה גופנית, משימה קוגניטיבית ורכיב מנטלי: הפוגה קצרה מהיום שמייצרת הקשבה לגוף, תנועה, תרגול קשב, חיבור וזמן איכות. הורים וילדים משחקים יחד בבית, בתוך אתגר ארגוני חודשי שמחזיק את המשפחות לאורך החודש.

| | |
| --- | --- |
| פורמט | משחקים של 1 עד 3 דקות. מפגש של כ-10 דקות, שלושה-ארבעה משחקים ברצף |
| שלושת הרכיבים | גוף: תנועה. מוח: אתגר מחשבתי בתוך התנועה. מנטלי: עצירה, הקשבה לגוף, תרגול קשב |
| עטיפה ארגונית | אתגר חודשי לכל הארגון: ניקוד, טבלת צוותים ודוח מצטבר ל-HR בסוף החודש |
| כניסה | קישור וקוד ארגוני, בלי חיבור למערכות הארגון בשלב הראשון |
| ציוד | בלי ציוד מיוחד. כל משחק עובד עם שני משתתפים לפחות |
| פרטיות | הילד לא נרשם, אין וידאו, נשמר רק ניקוד. פרופיל משפחתי אחד שההורה מנהל |
| מי קונה | מנהלת רווחה או HR בארגון ישראלי של כמה מאות עד כמה אלפי עובדים |
| מי משתמש | העובד וילדיו בני 5 עד 12. אפשר לשחק גם עם בן או בת זוג, אחיין או שותף לדירה |
| מי עומדת מאחורי המוצר | המייסדת: דיאטנית קלינית ומאמנת כושר, שש שנים של עבודה עם ילדים בכוח מוח |

**הבעיה:** תנועה וזמן איכות משפחתי נעלמים מהשגרה של הורים עובדים, ותוכניות הרווחה של הארגון לא מגיעות אליהם הביתה ולא מחזיקות לאורך זמן.

**הבידול:** שלושה דברים ביחד. משחק שמפעיל גוף ומוח באותו רגע, שנבנה למשחק משותף של הורה וילד, ושמגיע דרך המעסיק.

**תועלות משניות שהמחקר בודק:** קשב, ויסות עצמי וויסות רגשי אצל הילדים. אנרגיה וחדות מחשבתית אצל ההורים.

---

## 2. מה ארגונים צריכים, ומה נשאר במוצר

הכלל לסינון: כל רכיב שנשאר עונה על צורך של מנהלת הרווחה. רכיב שלא עונה על צורך כזה יוצא, גם אם הוא רעיון טוב.

| מה הארגון צריך | מה עונה על זה במוצר | מה זה אומר לגרסה הראשונה |
| --- | --- | --- |
| השתתפות שאפשר להציג להנהלה | אתגר חודשי עם ניקוד וטבלת צוותים | דוח מצטבר אחד בסוף החודש: כמה עובדים, כמה משפחות, כמה חזרו לשחק |
| פעילות שמגיעה גם למשפחות | משחקים שנבנו להורה וילד יחד | כל משחק עובד עם שני משתתפים לפחות, בלי ציוד מיוחד |
| אפס עבודה לרווחה | ערכת השקה מוכנה | הודעת וואטסאפ, מייל, פוסטר עם קוד QR ותזכורת באמצע החודש |
| שקט בנושא פרטיות ואבטחה | הילד לא נרשם, אין וידאו, נשמר רק ניקוד | פרופיל משפחתי אחד שההורה מנהל |
| הוגנות כלפי עובדים בלי ילדים | אפשר לשחק עם מי שבבית: בן או בת זוג, אחיין, שותף לדירה | המשחקים לא דורשים שהשותף יהיה ילד |
| משהו חדש, לא עוד אפליקציית צעדים | שילוב גוף ומוח, משחקים שמתחלפים | משחק חדש כל שבוע או שבועיים |
| התחלה בלי מחלקת IT | כניסה בקישור וקוד ארגוני | בלי חיבור למערכות הארגון בשלב הראשון |

## 3. מה לא נכנס לגרסה הראשונה, ולמה

- **לוח אירועים ומפגשים:** הארגון כבר מפיק אירועים, וזה מוסיף לו עבודה במקום להוריד.
- **תזכורות בריאות כלליות ומעקב היענות:** לא מבדל, ומכניס מידע אישי שלא צריך.
- **ספריית תוכן, הרצאות ומתכונים:** נמכרים בנפרד, כסדנה שפותחת את האתגר.
- **צ'אט, שותפים לפי מיקום, אווטאר וסוכן AI:** פיתוח כבד וסיכון פרטיות, בלי שארגון ביקש את זה.
- **זיהוי תנועה במצלמה ומשחק בכמה טלפונים:** שלב ב', אחרי שהמשחקים עצמם הוכיחו שמשפחות חוזרות אליהם.
- **קופות חולים:** אחרי שיש נתונים מארגונים.

---

## 4. הקונה והמשתמש

| | הקונה | המשתמש |
| --- | --- | --- |
| מי | מנהלת רווחה או HR בארגון של כמה מאות עד כמה אלפי עובדים | עובד הורה וילדיו בני 5 עד 12 |
| מה היא רוצה | השתתפות גבוהה, פעילות שמגיעה גם למשפחות, בלי להפיק אירוע | משהו קצר וכיפי שלא דורש להתארגן |
| ממה היא חוששת | עוד כלי שאף אחד לא נכנס אליו, אבטחת מידע, עומס עליה | עוד אפליקציה, עוד מטלה, עוד זמן מסך |
| איך נראית הצלחה | אחוז עובדים פעילים, משפחות שהשתתפו, משוב טוב | צחוק, תחושת הצלחה, זמן ביחד |

## 5. השערות שהמחקר צריך לבדוק

כל אחת מהן יכולה ליפול. בסוגריים: איפה אפשר לבדוק אותה.

1. למנהלות רווחה חשוב להגיע גם למשפחות, ויש לזה תקציב, לא רק לאירועים. (מחקר שולחני חלקית, בעיקר שיחות)
2. הורים לילדים בני 5 עד 12 יקדישו כמה דקות, כמה פעמים בשבוע, למשחק משותף. (פיילוט)
3. משפחות חוזרות למשחק גם בשבוע השלישי, אחרי שהחידוש נגמר. (פיילוט. נתוני התמדה של מתחרים יכולים לתת רמז)
4. הילדים הם אלה שמזכירים להורים לשחק. אם זה נכון, זה מנוע ההתמדה של המוצר. (פיילוט)
5. עובדים בלי ילדים לא מרגישים מודרים מהאתגר. (שיחות. אפשר לבדוק איך פלטפורמות אחרות פותרות את זה)
6. ארגון מוכן לשלם לפי עובד לחודש, או על חבילה של סדנה פותחת ואתגר חודשי. (מחירי מתחרים במחקר, המחיר עצמו בשיחות)

---

## 6. המסר השיווקי (טיוטה)

**המסר המרכזי: רווחה שמגיעה הביתה.** רוב תוכניות הרווחה נגמרות בדלת של המשרד. כוח מוח ממשיכה הביתה: משחקי גוף ומוח קצרים שהורים וילדים משחקים יחד בסלון, באתגר חודשי של כל הארגון.

**הצהרת מיצוב (לשימוש פנימי):** לארגונים שרוצים שהרווחה תגיע גם למשפחות של העובדים, כוח מוח היא תוכנית חודשית של משחקי גוף ומוח קצרים להורים וילדים. בשונה מאפליקציות צעדים, מימי כיף חד-פעמיים ומקייטנות קיץ, היא בונה הרגל משפחתי שחוזר לאורך החודש, לא דורשת מהרווחה להפיק כלום, ונותנת בסוף החודש מספרים שאפשר להציג להנהלה.

**שלוש כותרות לבחירה:**
1. רווחה שמגיעה הביתה. (המועדפת, כי היא מדברת בדיוק על הבעיה שמנהלת הרווחה מכירה)
2. עשר דקות בסלון שכל המשפחה מחכה להן.
3. המשחק שהילדים יזכירו להורים לשחק.

## 7. מה מותר לטעון על התועלות (טיוטה, לאימות בשלב 4)

המחקר תומך בכיוון, אבל לא בהבטחות גדולות. רוב המחקרים נעשו בבתי ספר ולא בבית, ואף אחד מהם לא בדק את המשחקים של כוח מוח. לכן: לטעון על מה שהמשחק מתרגל, לצטט את המחקר הכללי, ולשמור טענות על תוצאות לאחרי הפיילוט.

| התועלת | מה המשחק עושה בפועל | מה המחקר מראה (בדיקה ראשונית) | ניסוח שמותר להשתמש בו | לא לכתוב |
| --- | --- | --- | --- | --- |
| קשב אצל הילדים | הוראות שמשתנות, להקשיב לפני שזזים, להחליף חוקים באמצע | אצל ילדים בני 11-12, הפסקת תנועה של 10 דקות עם אתגר מחשבתי שיפרה קשב ממוקד ומהירות עיבוד. המאמץ הגופני לבדו לא שיפר, וההנאה מהמשחק הייתה חלק מהמנגנון ([Schmidt 2016](https://pmc.ncbi.nlm.nih.gov/articles/PMC5047899)) | "משחקים שמתרגלים קשב: להקשיב, לעצור ולהחליף חוקים" | "משפר הפרעות קשב", "מוכח מדעית" |
| ויסות רגשי | עצירה על אות, המתנה לתור, טעות והמשך, הורה שמחזיק את החוקים | תוכניות שמתרגלות שליטה בדחף, בעלייה הדרגתית בקושי, עזרו לילדים בני 4-12 ([Diamond & Lee 2011](https://pmc.ncbi.nlm.nih.gov/articles/PMC3159917/)). במשחק גופני של אב וילד, הגבולות שהאב הציב הכריעו: בלי גבולות, יותר משחק פרוע נקשר ליותר תוקפנות ולוויסות רגשי חלש יותר ([Flanders](https://ojp.gov/ncjrs/virtual-library/abstracts/rough-and-tumble-play-and-development-physical-aggression-and)). הראיות כאן עקיפות | "מתרגלים יחד לעצור, לחכות ולנסות שוב" | "מרגיע התפרצויות", "מטפל בילדים עם קשיים" |
| אנרגיה וחדות להורה העובד | כמה דקות של תנועה עם אתגר לראש, בסוף יום עבודה | אימון בודד מעלה את תחושת האנרגיה באופן עקבי, גם אם לא תמיד מוריד עייפות ([Loy 2013](https://news.uga.edu/uga-kinesiology-exercise-boosts-energy/)). מטא-אנליזה מ-2025 מצאה השפעה חיובית קטנה של פעילות גופנית על ביצועים קוגניטיביים בכל הגילים, גם אחרי פעילות חד-פעמית ([מקור](https://jyx.jyu.fi/handle/123456789/104728)) | "הפסקה פעילה שמחזירה אנרגיה" | "משדרג ביצועים ב-X%", "מונע שחיקה" |
| הרכיב המנטלי: עצירה והקשבה לגוף | עצירה, נשימה והקשבה לגוף בין המשחקים | עוד לא נבדק. לחפש בשלב 4 | ייקבע אחרי שלב 4 | "מפחית חרדה", "מוריד מתח" (טענות טיפוליות) |

### מה המחקר אומר על המוצר עצמו

- **סבב של כעשר דקות, לא דקה אחת.** במחקר הקשב ההפסקה נמשכה 10 דקות, ויש סימנים שמתחת ל-6 דקות קשה לצפות לשיפור במצב הרוח ([מקור](https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2023.1180285/full), לאמת). לכן משחקים של דקה-שתיים, שלושה-ארבעה ברצף.
- **האתגר המחשבתי הוא העיקר.** בניסויים שהשוו, השילוב של תנועה ואתגר מחשבתי עבד יותר טוב מתנועה לבד ([Egger 2019](https://pmc.ncbi.nlm.nih.gov/articles/PMC6402646), [Benzing 2016](https://pmc.ncbi.nlm.nih.gov/articles/PMC5193332)).
- **כיף הוא חלק מהמנגנון, לא קישוט.** ההנאה תיווכה את השיפור בקשב.
- **ההורה מחזיק את החוקים.** משחקים עם כללי עצירה ברורים.
- **קושי שעולה בהדרגה.** כל התוכניות שעבדו העלו את האתגר לאורך הזמן.
- **יעד ותגמול יחד.** בתוכניות משפחתיות להעלאת פעילות גופנית, השילוב של הצבת יעד ותגמול היה מה שעבד ([Brown 2016](https://pmc.ncbi.nlm.nih.gov/articles/PMC4819691/)). זה בדיוק האתגר החודשי עם הנקודות.

כל אחד מהעקרונות האלה הוא גם טיעון מכירה: "המשחקים נבנו לפי מה שנמצא במחקר", בלי לטעון שהמשחקים עצמם נבדקו.

**לבדוק בשלב 4: פער במינון.** לפי בדיקה ראשונית של [Mao 2024](https://doi.org/10.3389/fpsyg.2024.1454447), ההשפעה של פעילות עם אתגר מחשבתי על תפקודים ניהוליים נמצאה בעיקר בתוכניות של יותר משישה שבועות, במפגשים של יותר מ-20 דקות, יותר מפעמיים בשבוע. המפגש של כוח מוח הוא כ-10 דקות. המחקר צריך להגיד במפורש על מה פורמט של 10 דקות בבית יכול להישען (למשל השפעה מיידית, כמו ב-Schmidt 2016), על מה לא (למשל שינוי מתמשך בתפקודים ניהוליים), והאם כדאי לבחון מפגש ארוך יותר פעם בשבוע.

## 8. מה לא להגיד בכלל

טענות כמו "מסנכרן בין שתי ההמיספרות" או "בונה נוירונים" נשמעות מדעיות, אבל אין להן בסיס. Brain Gym, תוכנית תנועה מוכרת לילדים שנבנתה על טענות כאלה, [ספגה ביקורת על היעדר ראיות](https://works.bepress.com/andrea_beam/3/). ומעבר לזה, טענה על טיפול בבעיות קשב היא כבר טענה רפואית: משחק וידאו לילדים עם ADHD נדרש ל[אישור של ה-FDA](https://www.mobihealthnews.com/news/mightier-scores-2m-nih-study-impacts-biofeedback-video-game-children-adhd) כדי לטעון אותה.

## 9. טיוטה לפנייה למנהלת רווחה

> רוב פעילויות הרווחה נגמרות כשהעובד יוצא מהמשרד. בניתי תוכנית שממשיכה הביתה: משחקי גוף ומוח קצרים שהורים משחקים עם הילדים בסלון, בלי ציוד ובלי הכנה. לאורך החודש הצוותים צוברים נקודות על כל משחק משפחתי, ובסוף החודש את מקבלת דוח פשוט: כמה עובדים השתתפו, כמה משפחות, וכמה חזרו לשחק. מאחורי המשחקים עומדות שש שנים של עבודה עם ילדים בכוח מוח, והרקע שלי כדיאטנית קלינית ומאמנת כושר. אשמח להראות לך משחק אחד, זה לוקח שלוש דקות.

---

## 10. מתחרים (השערות, לאימות בשלב 2)

בבדיקה ראשונית לא נמצא מוצר שעושה את שלושת הדברים יחד: משחק משותף להורה וילד, אתגר מחשבתי בתוך התנועה, ומכירה דרך המעסיק. כל מתחרה מכסה אחד או שניים מהם. זו השערה שהמחקר צריך לאשר או להפיל. המתחרה שנראה הכי מסוכן הוא Active Arcade, כי הוא חינמי.

### מטריצת המיצוב (בדיקה ראשונית)

| | משחק משותף להורה וילד | אתגר מחשבתי בתוך התנועה | נמכר דרך המעסיק |
| --- | --- | --- | --- |
| **כוח מוח** | כן | כן | כן |
| Active Arcade | כן | חלקית, משחקי תגובה | לא |
| Nex Playground | כן | לא בבסיס המוצר | לא |
| Kid Motion Coach | כן, במצב משפחה | לא | לא |
| GoNoodle | חלקית | חלקית, תנועה עם ספירה ומיינדפולנס | לא, בתי ספר ובית |
| BlazePod | חלקית | כן | לא |
| Mightier | לא, הילד משחק לבד | ויסות רגשי, בלי תנועה | כן |
| Personify Health | חלקית, בני משפחה מגיל 14 | לא | כן |

### מתחרים ישירים: משחק תנועה קצר בבית, באפליקציה או במכשיר

| שם | מה זה | איפה הם חזקים | איפה כוח מוח שונה |
| --- | --- | --- | --- |
| [Active Arcade](https://apps.apple.com/app/id1553158383) (Nex) | אפליקציה חינמית, משחקי תנועה במצלמת הטלפון, לבד או עם משפחה וחברים | חינם, בלי פרסומות ובלי מנוי, זיהוי תנועה בשל, [מיליוני הורדות לפי הודעה לעיתונות מ-2022](https://www.businesswire.com/news/home/20220901005259/en/Nex-Pioneers-Motion-Entertainment-With-a-Suite-of-Immersive-Experiences-for-Mobile-and-the-Living-Room) | שיטה קוגניטיבית, תוכנית ארגונית, עברית ודוח לארגון. מול מתחרה חינמי, הערך חייב להיות התוכנית ולא האפליקציה |
| [Nex Playground](https://www.smythstoys.com/uk/en-gb/gaming-and-tech/nex-playground/nex-playground-console-the-active-play-system-for-kids-and-families/p/262774) | קונסולה עם מצלמה לטלוויזיה, עד 4 שחקנים, מגיל 5, מנוי למשחקים נוספים | חוויה סלונית חזקה ותוכן ממותג | דורשת לקנות מכשיר. כוח מוח עובדת על הטלפון שכבר יש |
| [Kid Motion Coach](https://kid-motion-coach.kidslox.com/) (Kidslox) | אפליקציה לילדים בני 6-10, משימות של 5 דקות, אווטאר, תגים, לוח להורה ומצב משפחה | הפורמט הכי קרוב: קצר, משחקי, עם הורה | ממוקדת בכושר של הילד, בלי אתגר מחשבתי, נמכרת להורים |
| [GoNoodle](https://www.apkmirror.com/apk/gonoodle/gonoodle-kids-videos/) | סרטוני תנועה ומיינדפולנס לילדי יסודי, בבית ובבית הספר | מותג חזק. לפי החברה נמצאת ב-90% מבתי הספר היסודיים הציבוריים בארה"ב, [ומדברת במפורש על קשב וויסות](https://thewaltdisneycompany.com/news/gonoodle-star-wars-grogu/) | צפייה וחיקוי, בלי משוב ובלי משחק משותף אמיתי |
| [BlazePod](https://www.blazepod.com/en-ca/products/frx-trainer-course-b2b) | פודים מוארים ואפליקציה לאימון זמן תגובה וקבלת החלטות | השיטה הכי קרובה לגוף ומוח | חומרה יקרה, [תלונות על חומת תשלום וקריסות](https://fi.trustpilot.com/review/blazepod.com), לא בנוי להורה וילד |
| [NEO Kids](https://www.news5cleveland.com/news/national/balancing-fitness-and-family-theres-an-app-for-that) (NEOU) | אימוני וידאו משפחתיים של 10-20 דקות במנוי (לפי כתבה ישנה, לאמת שעדיין פעיל) | הורה וילד באותו אימון | אימון ולא משחק, בלי אתגר מחשבתי |
| Family Move ([EdUHK](https://repository.eduhk.hk/en/publications/development-and-pilot-evaluation-of-a-mobile-app-on-parent-child), [HKU](https://hub.hku.hk/handle/10722/290923)) | אפליקציה אקדמית לתרגול הורה-ילד עם נקודות ושלבים, פיילוט של 8 שבועות | לא מסחרית, אבל מראה שהרעיון נבדק אקדמית | מקור טוב לשלב המאמרים. יש שני קישורים, לשתי אוניברסיטאות שונות בהונג קונג: לבדוק איזו מהן ואם זה אותו מחקר |

### מתחרים עקיפים: אותו תקציב או אותה הבטחה, פתרון אחר

| מי | על מה הם מתחרים | מה ללמוד מזה |
| --- | --- | --- |
| [קייטנות קיץ וסבסוד קייטנות לילדי העובדים](https://www.ice.co.il/advertising-marketing/news/article/1080301) (למשל Playtika, Atera, Lightricks, [תנובה ובזק אונליין](https://finance.walla.co.il/item/3445813)) | תקציב הרווחה המשפחתי, בעיקר באוגוסט | העיתוי. מנהלות רווחה חושבות על הילדים בחופש הגדול ובחגים. אתגר של "קייטנה בסלון" באוגוסט יכול להיות דלת כניסה |
| [הרצאות וקבוצות הורות לעובדים](https://finance.walla.co.il/item/2993043) (למשל שיכון ובינוי, רוש) | תקציב ההורות בארגון | הסדנה של כוח מוח יכולה לפתוח את האתגר, כך שהיא לא מתחרה בהרצאה אלא מצטרפת אליה |
| ימי כיף משפחתיים ומתנות לאירועי ילדים | תשומת הלב של העובד ההורה | אירוע חד-פעמי מול הרגל חודשי. זה הבידול |
| [Mightier](https://www.magellanhealthcare.com/kids-emotions-mightier/) | ההבטחה לוויסות רגשי של ילדים בני 6-14, נמכר למעסיקים ולביטוחי בריאות | מוכיח שמעסיקים קונים מוצר דיגיטלי לילדים של העובדים. אבל הוא קליני, עם רצועת דופק, ופונה לילדים עם קשיים |
| [Personify Health](https://www.mobihealthnews.com/news/virgin-healthmiles-adds-family-members-teases-new-tracker-plans-change-name) (לשעבר Virgin Pulse), YuMuuv, Vantage Fit | העטיפה של האתגר החודשי | פתחו את האתגרים לבני משפחה, אבל רק מגיל 14 בגלל פרטיות (לפי כתבה ישנה, לאמת למצב היום) |
| תחליפים חינמיים בבית: יוטיוב, משחקי קופסה, קונסולה שכבר יש | הערב של המשפחה | משפחה לא צריכה אפליקציה כדי לזוז. היא צריכה סיבה ומבנה, וזה מה שהאתגר נותן |

### רשימת המתחרים הידועים

Active Arcade (Nex), Nex Playground, Kid Motion Coach (Kidslox), GoNoodle, BlazePod, NEO Kids (NEOU), Family Move, Mightier, Personify Health (formerly Virgin Pulse), YuMuuv, Vantage Fit.

עקיפים בישראל: קייטנות קיץ לילדי העובדים, הרצאות וקבוצות הורות לעובדים, ימי כיף משפחתיים.

תחליפים חינמיים: סרטוני תנועה ביוטיוב, משחקי קופסה, קונסולות בבית.

עוד שמות ששווה לבדוק: Ring Fit Adventure, Just Dance, Nintendo Switch Sports, Cosmic Kids Yoga, אתגרים משפחתיים ב-Fitbit, ספקי רווחה ישראליים שעובדים עם משפחות.

### חמשת המתחרים להשוואה לעומק (שלב 3)

1. **Active Arcade:** הכי קרוב בחוויה, וחינמי.
2. **Nex Playground:** אותה חברה כמו Active Arcade, עם מודל עסקי אחר: מכשיר ומנוי.
3. **Kid Motion Coach:** הכי קרוב בפורמט, כולל מצב משפחה ולוח להורה.
4. **GoNoodle:** הכי קרוב בהבטחה של קשב וויסות.
5. **Mightier:** הכי קרוב בערוץ המכירה, מוצר לילדים שנמכר דרך מעסיקים.

חלופה לצד הארגוני: Personify Health במקום Nex Playground.

---

## 11. מאמרי בסיס (seed papers)

| # | מאמר | קישור | מה נבדק (בדיקה ראשונית) | מה לאמת |
| --- | --- | --- | --- | --- |
| 1 | Diamond & Lee, 2011, Science | [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC3159917/) | סקירה של תוכניות לשיפור תפקודים ניהוליים בגילי 4-12. התוכניות שעבדו כללו תרגול חוזר ועלייה הדרגתית בקושי, וילדים עם תפקודים חלשים הרוויחו יותר | – |
| 2 | Vazou et al., 2016/2019, Int J Sport Exerc Psychol | [IRIS](https://iris.uniroma4.it/handle/20.500.14244/1529) | מטא-אנליזה של סוגי פעילות גופנית וקוגניציה בילדים ובני נוער. השפעה חיובית, ופעילות עם אתגר מחשבתי היא אחת הדרכים שעובדות | האם 2016 ו-2019 הם אותו מאמר (פרסום מקוון מול מודפס) |
| 3 | Mao et al., 2024, Frontiers in Psychology | [DOI](https://doi.org/10.3389/fpsyg.2024.1454447) | מטא-אנליזה: פעילות עם אתגר מחשבתי ותפקודים ניהוליים. השפעה חיובית, בעיקר בתוכניות של יותר משישה שבועות, מפגשים של יותר מ-20 דקות, יותר מפעמיים בשבוע | המינון המדויק, והפער מול מפגש של 10 דקות |
| 4 | Schmidt, Benzing & Kamer, 2016, Frontiers in Psychology | [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC5047899) | הפסקת תנועה של 10 דקות, 92 ילדים בני 11-12. האתגר המחשבתי, ולא המאמץ, שיפר קשב ממוקד. ההנאה תיווכה את ההשפעה | גודלי אפקט |
| 5 | Egger et al., 2019, PLoS One | [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC6402646) | 20 שבועות של הפסקות תנועה, 142 ילדים בני 7-9. שילוב של מאמץ ואתגר מחשבתי שיפר גמישות מחשבתית ומתמטיקה. מאמץ לבד לא | גודלי אפקט ומינון |
| 6 | Benzing et al., 2016, PLoS One | [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC5193332) | משחק תנועה חד-פעמי, 65 נערים בני 13-16. משחק עם אתגר מחשבתי גבוה שיפר גמישות מחשבתית יותר מאותו מאמץ בלי אתגר | הגילים מחוץ לטווח 5-12 |
| 7 | Brown et al., 2016, Obesity Reviews | [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC4819691/) | מטא-אנליזה של תוכניות משפחתיות לפעילות גופנית, ילדים בני 5-12. השפעה קטנה אך מובהקת. יעד ותגמול יחד הם מה שעבד | גודל אפקט |
| 8 | Flanders et al., 2009, Aggressive Behavior | [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC3283567/), [מחקר המשך](https://ojp.gov/ncjrs/virtual-library/abstracts/rough-and-tumble-play-and-development-physical-aggression-and) | משחק גופני פרוע בין אבות לילדים. הגבולות שהאב מציב קובעים אם המשחק קשור לוויסות טוב יותר או לתוקפנות. מחקר מתאמי | גילי הילדים, ממצאי מחקר ההמשך |
| 9 | Loy, O'Connor & Dishman, 2013 | [דוקטורט PDF](https://openscholar.uga.edu/record/18943/files/loy_bryan_d_201505_phd.pdf), [דיווח UGA](https://news.uga.edu/uga-kinesiology-exercise-boosts-energy/) | מטא-אנליזה: אימון בודד ותחושת אנרגיה ועייפות. אימון בודד מעלה אנרגיה באופן עקבי, הירידה בעייפות פחות עקבית | למצוא את מאמר כתב העת עצמו, לא רק את הדוקטורט |
| 10 | Physical activity context and cognition across the lifespan, 2025 | [JYX](https://jyx.jyu.fi/handle/123456789/104728) | מטא-אנליזה, 239 מחקרים, כ-48,600 משתתפים מגן ילדים עד גיל מבוגר. השפעה חיובית קטנה, גם לפעילות מתמשכת וגם לחד-פעמית | מחברים, מספרים, גישה פתוחה |
| 11 | Family Move, פיילוט אפליקציה להורה וילד | [EdUHK](https://repository.eduhk.hk/en/publications/development-and-pilot-evaluation-of-a-mobile-app-on-parent-child), [HKU](https://hub.hku.hk/handle/10722/290923) | אפליקציית תרגול הורה-ילד עם נקודות ושלבים, 8 שבועות. סימנים ראשונים לשיפור ברווחה ובפעילות, בלי קבוצת ביקורת | איזו אוניברסיטה, האם זה אותו מחקר. ייתכן שהקישור ל-EdUHK קטוע |
| 12 | Frontiers in Psychology, 2023, על אנרגיה ועייפות | [Frontiers](https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2023.1180285/full) | הבסיס לטענה שמתחת ל-6 דקות קשה לצפות לשיפור במצב הרוח | מה בדיוק כתוב שם, והאם זה מבוסס מחקר או מאמר דעה |

---

## 12. מילות מפתח התחלתיות (רשימת נתונים לשלבים 1 ו-4, לא פרומפט)

```
## A. Product and category (finding competitors)
family exergame app
parent-child exercise app
family fitness app for kids
active video games (AVG)
exergaming
motion games app
camera-based motion tracking games
markerless pose estimation fitness
active screen time
co-play / joint media engagement
intergenerational play
brain breaks for kids
movement breaks app
active family game night

## B. Employer side (finding B2B competitors)
employee wellbeing family members
family-inclusive wellness program
dependents wellness program
working parents benefits
caregiver benefits platform
corporate wellness challenge platform
team wellness challenge
gamified employee wellbeing

## C. Science (finding papers)
cognitively engaging physical activity
cognitive-motor training / motor-cognitive training
dual-task training children
exergaming executive functions
physical activity breaks attention children
acute exercise cognition children
inhibitory control / Go-No-Go
cognitive flexibility / shifting
self-regulation physical activity children
emotion regulation parent-child play
rough-and-tumble play
parent-child co-activity physical activity
family-based physical activity intervention
positive affect exercise children
acute exercise energy fatigue adults
exercise snacks
mindful movement children
yoga-based physical activity children executive function
body awareness / interoception children
breathing exercise children self-regulation

## D. Market (size and trends)
family wellness app market
kids fitness app market size
exergaming market size
corporate wellness market Israel
employee wellbeing spending Israel
parental burnout working parents
```

חיפוש לדוגמה ב-PubMed:

```
("cognitively engaging" OR "cognitive-motor" OR "dual-task" OR exergam*)
AND ("physical activity" OR exercise)
AND (child* OR famil* OR parent*)
AND ("executive function*" OR attention OR "self-regulation" OR "emotion regulation")
```

מונחי MeSH ששווה לנסות (לוודא ב-MeSH Browser): Exergaming, Executive Function, Exercise, Parent-Child Relations, Video Games, Attention, Self-Control, Emotional Regulation.

---

## 13. כללי עבודה למחקר

- לאמת כל חברה, מוצר, מחיר ומאמר מול מקור חי. מה שלא אומת מסומן "לא אומת". לא להמציא שמות, מספרים, קישורים או ציטוטים.
- קישור למקור ליד כל עובדה.
- מספרים ממאמרים לוקחים רק מהמאמר עצמו. אם נקרא רק התקציר, לכתוב את זה.
- להבחין בין מה שאומת עכשיו, מה שבא מהקובץ הזה, ומה שהוא הערכה.
- סיכומים והסברים בעברית. שמות חברות, כותרות מאמרים ומונחי חיפוש באנגלית.
- רק גישה פתוחה. לא לעקוף חומות תשלום.
- טבלאות קצרות עדיפות על פרוזה ארוכה.

## 14. שלב השיחות (נעשה על ידי המייסדת, לא על ידי הכלי)

**שמונה עד עשר שיחות עם מנהלות רווחה ו-HR**, 20 דקות כל אחת. לשאול על מה שכבר קרה, לא על מה שהיא אולי תעשה:

1. מה עשיתם ברווחה בשנה האחרונה, ומה באמת עבד?
2. מה עשיתם בשביל המשפחות של העובדים, ומאיזה תקציב זה הגיע?
3. איך את מודדת אם פעילות הצליחה, ולמי את מציגה את זה?
4. מה הכי מתיש אותך בהפקה של פעילות?
5. בפעם האחרונה שקניתם כלי דיגיטלי, מי היה צריך לאשר, וכמה זמן זה לקח?

לא לשאול "היית קונה את זה?". על השאלה הזאת כמעט כולם עונים בנימוס, וזה לא אומר כלום.

**עשר עד חמש עשרה משפחות שמנסות את המשחקים בבית**, שלוש פעמים בשבוע במשך שבועיים. מה לבדוק: מי יזם כל פעם, כמה זמן שיחקו בפועל, האם חזרו בשבוע השני, ומה הילד אמר אחרי. זה בודק את השערות 2, 3 ו-4.

---

## 15. מקורות

**מחקר**
- [Diamond & Lee, 2011, Science (PMC)](https://pmc.ncbi.nlm.nih.gov/articles/PMC3159917/)
- [Vazou et al., 2019, International Journal of Sport and Exercise Psychology](https://iris.uniroma4.it/handle/20.500.14244/1529)
- [Mao et al., 2024, Frontiers in Psychology](https://doi.org/10.3389/fpsyg.2024.1454447)
- [Schmidt, Benzing & Kamer, 2016, Frontiers in Psychology (PMC)](https://pmc.ncbi.nlm.nih.gov/articles/PMC5047899)
- [Egger et al., 2019, PLoS One (PMC)](https://pmc.ncbi.nlm.nih.gov/articles/PMC6402646)
- [Benzing et al., 2016, PLoS One (PMC)](https://pmc.ncbi.nlm.nih.gov/articles/PMC5193332)
- [Brown et al., 2016, Obesity Reviews (PMC)](https://pmc.ncbi.nlm.nih.gov/articles/PMC4819691/)
- [Flanders et al., 2009, Aggressive Behavior (PMC)](https://pmc.ncbi.nlm.nih.gov/articles/PMC3283567/)
- [Flanders et al., מחקר המשך של חמש שנים (תקציר)](https://ojp.gov/ncjrs/virtual-library/abstracts/rough-and-tumble-play-and-development-physical-aggression-and)
- [Loy et al., 2013, דיווח של אוניברסיטת ג'ורג'יה](https://news.uga.edu/uga-kinesiology-exercise-boosts-energy/)
- [Loy, עבודת דוקטורט (PDF)](https://openscholar.uga.edu/record/18943/files/loy_bryan_d_201505_phd.pdf)
- [מטא-אנליזה על פעילות וקוגניציה לאורך החיים, 2025](https://jyx.jyu.fi/handle/123456789/104728)
- [Frontiers in Psychology, 2023, אנרגיה ועייפות](https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2023.1180285/full)
- [Family Move, רשומה ב-EdUHK](https://repository.eduhk.hk/en/publications/development-and-pilot-evaluation-of-a-mobile-app-on-parent-child)
- [Family Move, רשומה ב-HKU](https://hub.hku.hk/handle/10722/290923)
- [ביקורת על Brain Gym, Exceptionality, 2010](https://works.bepress.com/andrea_beam/3/)

**מתחרים ושוק**
- [Active Arcade, App Store](https://apps.apple.com/app/id1553158383)
- [Nex, הודעה לעיתונות 2022](https://www.businesswire.com/news/home/20220901005259/en/Nex-Pioneers-Motion-Entertainment-With-a-Suite-of-Immersive-Experiences-for-Mobile-and-the-Living-Room)
- [Nex Playground, Smyths Toys](https://www.smythstoys.com/uk/en-gb/gaming-and-tech/nex-playground/nex-playground-console-the-active-play-system-for-kids-and-families/p/262774)
- [Kid Motion Coach, Kidslox](https://kid-motion-coach.kidslox.com/)
- [GoNoodle, תיאור האפליקציה](https://www.apkmirror.com/apk/gonoodle/gonoodle-kids-videos/)
- [GoNoodle ודיסני, הודעה לעיתונות](https://thewaltdisneycompany.com/news/gonoodle-star-wars-grogu/)
- [BlazePod](https://www.blazepod.com/en-ca/products/frx-trainer-course-b2b)
- [BlazePod, ביקורות ב-Trustpilot](https://fi.trustpilot.com/review/blazepod.com)
- [NEO Kids, כתבה](https://www.news5cleveland.com/news/national/balancing-fitness-and-family-theres-an-app-for-that)
- [Mightier, Magellan Healthcare](https://www.magellanhealthcare.com/kids-emotions-mightier/)
- [MobiHealthNews על Mightier ו-EndeavorRx](https://www.mobihealthnews.com/news/mightier-scores-2m-nih-study-impacts-biofeedback-video-game-children-adhd)
- [MobiHealthNews על פתיחת Virgin HealthMiles לבני משפחה](https://www.mobihealthnews.com/news/virgin-healthmiles-adds-family-members-teases-new-tracker-plans-change-name)
- [ice, קייטנות לילדי העובדים](https://www.ice.co.il/advertising-marketing/news/article/1080301)
- [וואלה, ארגונים שמפעילים ילדים בחופש](https://finance.walla.co.il/item/3445813)
- [וואלה, הרצאות הורות ותמיכה בילדי העובדים](https://finance.walla.co.il/item/2993043)

