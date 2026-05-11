# Submission Checklist & Hand-Drawn Sketch Guide
## DT CultureTech — Business Analytics Part A

---

## PRE-SUBMISSION CHECKLIST

### File Structure Verification
- [ ] `README.md` — Present and complete (no placeholder text)
- [ ] `methodology.md` — ICP logic, scoring rubric, filtering process documented
- [ ] `verification_process.md` — AI hallucination risks and manual check process documented
- [ ] `company_research_notes.md` — All 25 companies profiled (no "remaining rows omitted")
- [ ] `target_company_analysis.csv` — 25 rows, 20 columns, no blank rows
- [ ] `charts/industry_distribution.png` — Chart file exists and renders correctly
- [ ] `charts/score_distribution.png` — Chart file exists and renders correctly
- [ ] `charts/employee_analysis.png` — Chart file exists and renders correctly
- [ ] `optional_code/generate_data_and_charts.py` — Script runs without errors
- [ ] `optional_code/analysis.ipynb` — Valid Jupyter notebook JSON structure

### Content Quality Verification
- [ ] No placeholder text (no "remaining rows omitted", "TBD", "example only")
- [ ] All 25 companies have non-generic personalization hooks
- [ ] Score distribution is meaningful (range ≥ 8 points between highest and lowest)
- [ ] At least 3 companies per verdict tier: HOT, WARM
- [ ] No company has identical scores across all 6 criteria (would indicate no research)
- [ ] All assumptions labelled `[ESTIMATED]` or `[ASSUMPTION]`
- [ ] SEBI risk on Growpital documented prominently
- [ ] Three existing DT clients (Growpital, Kringle.ai, IPx) included and explained

### GitHub Submission Format
- [ ] Repository is PUBLIC (test in incognito window)
- [ ] README.md renders correctly on repository landing page
- [ ] CSV file previews correctly in GitHub's CSV viewer
- [ ] All image files display in browser
- [ ] Commit messages are professional (not "upload stuff" or "final version v3")
- [ ] No personal sensitive information in any file

### Personal Integrity Check
- [ ] You can explain every score in the CSV if asked in an interview
- [ ] You have verified at least 5 companies manually (website + LinkedIn)
- [ ] You understand what LMF, PMF, MMF, CMF represent in DT's context
- [ ] You understand why Growpital was chosen (existing DT client + SEBI risk = analytical depth)
- [ ] Hand-drawn sketch is complete and photographed

---

## HAND-DRAWN SKETCH GUIDE

### What the Sketch Must Demonstrate
The hand-drawn sketch proves you understood the research process conceptually — not just that you filled in a spreadsheet. It shows:
1. How you thought about identifying companies (funnel thinking)
2. How you controlled for AI hallucinations (critical thinking)
3. How you made scoring decisions (analytical judgment)

---

### Sketch 1: The Research Funnel (MOST IMPORTANT)

**Title:** "How I Built the 25-Company Target List"

**Draw this top-down funnel:**

```
╔══════════════════════════════════════════╗
║   STAGE 1: BROAD SEARCH (~60 companies) ║
║   Sources: Tracxn, Inc42, Internshala,  ║
║   LinkedIn, YourStory, Crunchbase       ║
╚══════════════╦═══════════════════════════╝
               ▼
╔══════════════════════════════════════════╗
║   STAGE 2: HARD FILTER (~40 remaining)  ║
║   REMOVE: >1000 emp, PE-owned,          ║
║   pre-revenue, pure services, no ICP    ║
╚══════════════╦═══════════════════════════╝
               ▼
╔══════════════════════════════════════════╗
║   STAGE 3: SOFT FILTER (~30 remaining)  ║
║   PRIORITIZE: Active LinkedIn founder,  ║
║   EdTech sector, recent funding,        ║
║   Hyderabad HQ, DT client confirmation  ║
╚══════════════╦═══════════════════════════╝
               ▼
╔══════════════════════════════════════════╗
║   STAGE 4: SCORE & VERIFY (25 final)    ║
║   Apply 6-criteria scoring (C1–C6)      ║
║   Verify each company via 5-step check  ║
║   Tag: VERIFIED / ESTIMATED / ASSUMPTION║
╚══════════════╦═══════════════════════════╝
               ▼
╔══════════════════════════════════════════╗
║   FINAL OUTPUT: HOT / WARM / COLD       ║
║   HOT: 14 companies (immediate)         ║
║   WARM: 11 companies (monitor)          ║
╚══════════════════════════════════════════╝
```

**Margin notes to add:**
- At Stage 1: "AI helped generate list, but each name was independently verified"
- At Stage 2: Write "REJECTED: enterprise companies, PE-owned, dissolved" with X marks
- At Stage 4: Circle the "VERIFIED" tag and write "Most important step"

---

### Sketch 2: AI Hallucination Control Map

**Title:** "Where AI Can Lie and How I Caught It"

**Draw a 2-column table:**

| AI MIGHT LIE ABOUT | HOW I CAUGHT IT |
|---|---|
| Fabricated revenue numbers | Used revenue BAND, not specific number. Sourced from Entrackr/Tracxn |
| Fake company names | Checked official website + LinkedIn + MCA for every company |
| Wrong founder backgrounds | Verified via LinkedIn profile education section + news interviews |
| Stale company status | Searched news + "2024" OR "2025" for each company |
| Uniform scores (no research) | Checked score distribution — should vary meaningfully (17–27) |

**Add a "DANGER" symbol next to the most risky hallucination type (fabricated financials)**

---

### Sketch 3: Scoring Grid (The 6 Criteria)

**Title:** "My 6-Criteria Scoring System"

**Draw a simple grid:**

```
CRITERION          | 1 (WEAK) | 3 (MODERATE) | 5 (STRONG)
C1: Innovation     | No L&D   | Blog posts    | Published research culture
C2: Team Size      | <10 emp  | 30–100 emp    | 100–500 emp
C3: LinkedIn DM    | No profile| Inactive     | Active thought leader
C4: Budget         | Pre-seed  | Seed          | Series B+
C5: Personaliz.    | No hook   | General news  | Specific recent trigger
C6: Domain         | Unrelated | Adjacent      | Direct EdTech
```

**Mark HOT threshold: ≥ 22/30 with a red line**

---

### Sketch 4: My Thought Process (Personal Reflection)

**Title:** "How I Thought Through This Assignment"

**Draw a mindmap or sequential notes:**

```
STARTED WITH: Understanding DT CultureTech first
  → Read their Internshala job descriptions
  → Identified their existing clients (Growpital, Kringle.ai, IPx)
  → Understood their LMF/PMF/MMF/CMF frameworks

THEN: Defined who DT sells TO
  → B2B product startups, 20–500 people
  → Innovation-conscious founders
  → EdTech, FinTech, HRTech sectors

DISCOVERED: Growpital has a SEBI risk
  → Decision: Include it with risk flagged (analytical honesty)
  → Did NOT hide the negative finding

AI USED FOR: Generating initial list of 60 companies
AI REJECTED: "EduSpark Technologies" (couldn't verify), fabricated revenue figures

FINAL CHECK: Does this look like real research or AI output?
  → Scores vary (17–27, not all same)
  → Negative findings included (SEBI, budget limits)
  → Assumptions clearly labelled
  → Sources named for key claims
```

---

### Drawing Tips

1. **Use boxes and arrows** — the evaluator reads these as structured thinking, not just handwriting
2. **Write a title on every sketch** — it signals you know what each diagram communicates
3. **Include at least one "rejected" or "risk" element** — it shows critical thinking
4. **Keep handwriting legible** — neat print is better than rushed cursive
5. **Add the date** — shows this is a real artifact, not a retroactive addition
6. **One page per sketch** — don't crowd everything onto one sheet

---

*Draw the sketches AFTER completing the written submission so they accurately reflect the conclusions you reached, not assumptions you had before research.*
