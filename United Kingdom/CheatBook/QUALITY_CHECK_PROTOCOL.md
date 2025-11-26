# ADIT UK CheatBook - Quality Check Protocol

## Overview

This document provides a systematic protocol for quality-checking the entire ADIT UK CheatBook. Due to the size of the CheatBook (~320 pages), quality checks are designed to be executed in phases across multiple sessions.

**Target Audience**: QA reviewer using Claude Opus 4.5
**Estimated Sessions**: 8-10 sessions
**Prerequisites**: Access to Past Papers, Suggested Answers, ADIT UK Syllabus, June 2025 Exam Paper

---

## Web Validation Framework

### Purpose
Web validation provides an additional layer of verification beyond internal documents. Use web searches and authoritative sources to confirm accuracy of rates, legislation, case law, dates, and other verifiable facts.

### When to Use Web Validation

Web validation should be triggered when:
1. **Uncertainty exists** - Internal sources conflict or seem outdated
2. **High-risk items** - Tax rates, deadlines, or legislation that changes frequently
3. **Mid-year changes** - Budget announcements, rate changes, new legislation
4. **Case law verification** - Confirming cases haven't been overturned
5. **Current affairs** - Recent tax policy changes (e.g., non-dom abolition)

### Validation Approach by Content Type

#### Tax Rates & Thresholds
**Method**: Search for the specific rate + tax year + "UK"

| Item Type | Search Strategy | Example Query |
|-----------|-----------------|---------------|
| Income Tax rates | Search rate + band + year | "UK income tax rates 2024/25 HMRC" |
| CGT rates | Search for recent changes | "UK capital gains tax rates October 2024 budget" |
| NIC rates | Search class + rate + year | "UK Class 4 NIC rate 2024/25" |
| SDLT thresholds | Search for temporary/permanent | "SDLT thresholds April 2025 changes" |
| IHT nil rate band | Search current threshold | "inheritance tax nil rate band 2024/25" |
| CT rates | Search main rate + small profits | "UK corporation tax rate 2024 small profits" |

**Key Sources** (starting points, not exhaustive):
- HMRC guidance pages (gov.uk)
- Professional body summaries (ICAEW, CIOT, ATT)
- Major accountancy firm tax updates

#### Legislation Citations
**Method**: Verify Act name, section numbers, and current status

| Verification Need | Search Strategy | Example Query |
|-------------------|-----------------|---------------|
| Section exists | Search Act + section | "TIOPA 2010 Part 9A CFC" |
| Current version | Check for amendments | "FA 2013 Schedule 45 amendments" |
| Correct Act | Verify provision location | "statutory residence test which Act" |
| Recent changes | Search for Finance Act updates | "Finance Act 2024 CFC changes" |

**Key Sources**:
- legislation.gov.uk (official, shows amendments)
- Tax professional commentary on recent changes
- HMRC manuals

#### Case Law
**Method**: Verify case name, citation, principle, and current status

| Verification Need | Search Strategy | Example Query |
|-------------------|-----------------|---------------|
| Case citation | Search case name + year | "Gaines-Cooper v HMRC 2011 citation" |
| Principle correct | Search case + topic | "Smallwood HMRC treaty residence principle" |
| Still good law | Search for appeals/overruling | "[Case name] overruled OR appealed OR distinguished" |
| Recent cases | Search topic + recent | "UK residence case law 2023 2024" |

**Key Sources**:
- BAILII (British and Irish Legal Information Institute)
- Tax case summaries from professional bodies
- Legal databases and commentary

#### Dates & Deadlines
**Method**: Verify specific deadlines against official sources

| Verification Need | Search Strategy | Example Query |
|-------------------|-----------------|---------------|
| Filing deadlines | Search return type + deadline | "self assessment online deadline 2024/25" |
| Payment dates | Search tax + payment date | "corporation tax payment deadline 9 months" |
| Time limits | Search election + time limit | "CGT holdover relief claim time limit" |
| Recent changes | Search for deadline changes | "UK tax deadline changes 2024" |

#### Exam Structure & Syllabus
**Method**: Verify against current ADIT documentation

| Verification Need | Search Strategy | Example Query |
|-------------------|-----------------|---------------|
| Module structure | Search ADIT + module | "ADIT UK module 2.09 exam structure 2025" |
| Time allocation | Search ADIT exam duration | "ADIT exam 195 minutes 3 hours 15" |
| Syllabus changes | Search for updates | "ADIT syllabus update 2025" |

**Key Sources**:
- tax.org.uk (CIOT official)
- ADIT candidate guidance documents

#### Recent Policy Changes
**Method**: Search for announcements and implementation dates

| Topic | Search Strategy | Example Query |
|-------|-----------------|---------------|
| Non-dom changes | Search regime + abolition | "UK non-dom abolition April 2025 FIG regime" |
| Budget changes | Search budget + topic | "Autumn Budget 2024 CGT rates" |
| New legislation | Search Act + commencement | "Finance Act 2024 commencement dates" |

### Web Validation Process

#### Step 1: Identify Items Requiring Validation
During each QA phase, flag items that need web validation:
- [ ] Items with ⚠️ warnings in Golden Reference
- [ ] Rates/thresholds (especially those with mid-year changes)
- [ ] Any item where internal sources seem uncertain
- [ ] Recent legislative or policy changes

#### Step 2: Prioritize by Risk
| Priority | Criteria | Action |
|----------|----------|--------|
| HIGH | Exam-critical, frequently tested, recent changes | Validate immediately |
| MEDIUM | Important but stable, less frequently tested | Validate if time permits |
| LOW | Supplementary info, unlikely to affect exam answers | Note for future review |

#### Step 3: Execute Searches
For each item:
1. Start with specific search query
2. Check 2-3 authoritative sources for confirmation
3. Note any conflicting information
4. Record source and date of verification

#### Step 4: Document Findings
Use the Web Validation Log:

```markdown
## Web Validation Log

### Item: [Description]
### Date Checked: [YYYY-MM-DD]

| Source | Finding | URL/Reference |
|--------|---------|---------------|
| Source 1 | What it says | Link or citation |
| Source 2 | What it says | Link or citation |

**Conclusion**: [Correct / Incorrect / Needs Update]
**Action**: [None / Update document / Flag for review]
```

#### Step 5: Cross-Reference Multiple Sources
Never rely on a single source. For critical items:
- Government source (gov.uk, HMRC)
- Professional body (CIOT, ICAEW, ATT)
- Major firm commentary (Big 4, mid-tier)

If sources conflict, note the conflict and use the most authoritative/recent source.

### Integration with QA Phases

| Phase | Web Validation Focus |
|-------|---------------------|
| Phase 1 (Golden Reference) | Validate all rates against official sources |
| Phase 2-7 (Chapter checks) | Validate items that differ from Golden Reference |
| Phase 8 (Deep Verification) | Comprehensive web validation of source material |

### Handling Discrepancies

When web sources contradict CheatBook content:

1. **Confirm the discrepancy** - Check multiple sources
2. **Determine which is correct** - Prefer official government sources
3. **Check timing** - Is the CheatBook using older rates?
4. **Log the finding** - Document in Findings Log with sources
5. **Recommend action** - Update CheatBook or flag for exam date consideration

### Limitations & Caveats

- **Web search results change** - Document date of search
- **Not all sources are authoritative** - Verify source credibility
- **Exam may use specific date rates** - Note if rates change mid-year
- **Some items can't be web-verified** - Past paper content, worked examples
- **Professional judgement required** - Web validation supplements, doesn't replace, expert review

---

## How to Use This Protocol

### Step 1: Create the Golden Reference Extract (Session 1)
Before checking any chapter, first create the Golden Reference Extract from Chapter 05 Appendices. This becomes your single source of truth for cross-chapter consistency.

See: `GOLDEN_REFERENCE_EXTRACT.md` (template provided)

### Step 2: Execute Phase-by-Phase
Work through each phase in order. Each phase is designed to fit within a single session's token limit.

### Step 3: Log All Findings
Use the Findings Log template at the end of this document to track issues found.

### Step 4: Fix Issues
After each phase, fix identified issues before proceeding.

---

## Quality Check Categories

### Category A: Content Accuracy (Items 1-9)
Verifying factual correctness against source materials.

### Category B: Internal Consistency (Items 10-12)
Ensuring information matches across chapters.

### Category C: Technical Accuracy (Items 13-16)
Verifying legal/technical information is current and correct.

### Category D: Arithmetic Accuracy (Items 17-19)
Checking all numbers add up correctly.

### Category E: Usability (Items 20-22)
Ensuring the document is easy to use.

### Category F: Strategic Alignment (Items 23-25)
Verifying alignment with exam requirements.

### Category G: Practical Application (Items 26-27)
Ensuring advice is actionable.

---

## Phase 1: Golden Reference Extraction

**Session**: 1 of 8-10
**Input**: `05_Appendices/Appendices_Complete.md`
**Output**: `GOLDEN_REFERENCE_EXTRACT.md`

### Task
Extract all verifiable facts from Chapter 05 into a compact reference document:

1. **Exam Structure Facts**
   - Total time: 195 minutes (3¼ hours)
   - Part A: 2 compulsory questions × 25 marks = 50 marks
   - Part B: Choose 1 of 2 questions × 20 marks = 20 marks
   - Part C: Choose 2 of 5 questions × 15 marks = 30 marks
   - Total: 100 marks
   - Minutes per mark: ~1.95

2. **Tax Rates (2024/25)**
   - Extract all IT, CT, CGT, IHT, NIC, SDLT, VAT, ATED rates
   - Format as single consolidated table

3. **Key Definitions**
   - Extract all statutory definitions
   - One-line format each

4. **Legislation Citations**
   - Extract all Act/Section references
   - Organized by topic

5. **Case Law**
   - Extract all case names and principles
   - One-line format each

6. **Formulas**
   - Extract all calculation formulas
   - Standardized notation

7. **Deadlines/Time Limits**
   - Extract all dates and periods

### Verification
Cross-check extracted facts against:
- June 2025 Exam Paper (for exam structure, tax rates)
- ADIT UK Syllabus (for topic coverage)

---

## Phase 2: Chapter 01 - Battlefield Intelligence

**Session**: 2 of 8-10
**Input**:
- `GOLDEN_REFERENCE_EXTRACT.md`
- `01_Battlefield_Intelligence/` (all 4 files)
- Past Papers folder
- Suggested Answers folder

### Checklist

#### A. Content Accuracy

| # | Check Item | How to Verify | Status |
|---|------------|---------------|--------|
| 1 | **Past Paper References** | For each past paper mentioned, verify: question number matches, question text is accurate, suggested answer points are correct | ⬜ |
| 2 | **Exam Structure** | Verify questions per section and options match Golden Reference | ⬜ |
| 3 | **Exam Time** | Verify 195 minutes / 3¼ hours wherever mentioned | ⬜ |
| 4 | **Authorities** | Check any case law or legislation citations against Golden Reference | ⬜ |
| 5 | **Dates** | Verify all dates including tax year references | ⬜ |
| 6 | **Rates** | Any rates mentioned match Golden Reference | ⬜ |
| 7 | **Calculations** | Verify any calculations are correct | ⬜ |
| 8 | **Completeness** | All 4 sections present and complete | ⬜ |
| 9 | **Topic Coverage** | Matches CHEATBOOK_STRUCTURE_PLAN.md requirements | ⬜ |

#### B. Internal Consistency

| # | Check Item | How to Verify | Status |
|---|------------|---------------|--------|
| 10 | **Cross-chapter consistency** | All facts match Golden Reference | ⬜ |
| 11 | **Template-example alignment** | N/A for this chapter | ⬜ |
| 12 | **Cross-references** | Any references to other chapters exist | ⬜ |

#### D. Arithmetic Accuracy

| # | Check Item | How to Verify | Status |
|---|------------|---------------|--------|
| 17 | **Mark totals** | Part A (50) + Part B (20) + Part C (30) = 100 | ⬜ |
| 18 | **Time allocations** | Sum to 195 minutes | ⬜ |
| 19 | **Minutes-per-mark** | ~1.95 min/mark consistent | ⬜ |

#### E. Usability

| # | Check Item | How to Verify | Status |
|---|------------|---------------|--------|
| 20 | **Acronyms defined** | All acronyms explained on first use | ⬜ |
| 21 | **Terminology consistent** | Same terms used throughout | ⬜ |
| 22 | **Tables render** | All markdown tables display correctly | ⬜ |

---

## Phase 3: Chapter 02 Part A - Complex Analysis Questions

**Session**: 3 of 8-10
**Input**:
- `GOLDEN_REFERENCE_EXTRACT.md`
- `02_Major_Question_Types/Part_A_Complex_Analysis_Questions.md`
- `02_Major_Question_Types/Part_A_Residence_Template.md`
- Past Papers (Part A questions)
- Suggested Answers (Part A)

### Checklist

#### A. Content Accuracy

| # | Check Item | How to Verify | Status |
|---|------------|---------------|--------|
| 1 | **Past Paper References** | Verify all June 2020-2025 Part A questions cited are accurate | ⬜ |
| 2 | **Exam Structure** | Part A = 2 × 25 marks compulsory | ⬜ |
| 3 | **Exam Time** | Part A time allocation (~48 min each) correct | ⬜ |
| 4 | **Authorities** | All legislation citations correct (FA 2013 Sch 45, CTA 2009, TIOPA 2010, etc.) | ⬜ |
| 5 | **Dates** | All dates correct (tax years, deadlines) | ⬜ |
| 6 | **Rates** | All rates match Golden Reference | ⬜ |
| 7 | **Calculations** | All worked examples calculate correctly | ⬜ |
| 8 | **Completeness** | All topics covered: Corporate Residence, Individual Residence (SRT), PE, Remittance Basis | ⬜ |
| 9 | **Topic Coverage** | Matches syllabus requirements | ⬜ |

#### B. Internal Consistency

| # | Check Item | How to Verify | Status |
|---|------------|---------------|--------|
| 10 | **Cross-chapter consistency** | Definitions, rates, legislation match Golden Reference | ⬜ |
| 11 | **Template-example alignment** | Worked examples follow the templates | ⬜ |
| 12 | **Cross-references** | References to other sections valid | ⬜ |

#### C. Technical Accuracy

| # | Check Item | How to Verify | Status |
|---|------------|---------------|--------|
| 13 | **Legislation current** | All Acts/sections still in force | ⬜ |
| 14 | **Case law valid** | Cases not overturned | ⬜ |
| 15 | **OECD Model version** | Consistent reference | ⬜ |
| 16 | **Formula accuracy** | All formulas mathematically correct | ⬜ |

#### D. Arithmetic Accuracy

| # | Check Item | How to Verify | Status |
|---|------------|---------------|--------|
| 17 | **Mark totals** | Mark breakdowns add to 25 per question | ⬜ |
| 18 | **Time allocations** | Time advice sums correctly | ⬜ |
| 19 | **Minutes-per-mark** | Consistent application | ⬜ |

#### E-G. Usability, Strategic, Practical

| # | Check Item | Status |
|---|------------|--------|
| 20-22 | Usability checks | ⬜ |
| 23-25 | Strategic alignment | ⬜ |
| 26-27 | Practical application | ⬜ |

---

## Phase 4: Chapter 02 Part B - Anti-Avoidance Questions

**Session**: 4 of 8-10
**Input**:
- `GOLDEN_REFERENCE_EXTRACT.md`
- `02_Major_Question_Types/Part_B_Anti_Avoidance_Questions.md`
- `02_Major_Question_Types/Part_B_CFC_Template.md`
- Past Papers (Part B questions)
- Suggested Answers (Part B)

### Checklist

#### A. Content Accuracy

| # | Check Item | How to Verify | Status |
|---|------------|---------------|--------|
| 1 | **Past Paper References** | Verify all Part B questions cited are accurate | ⬜ |
| 2 | **Exam Structure** | Part B = Choose 1 of 2 × 20 marks | ⬜ |
| 3 | **Exam Time** | Part B time allocation (~39 min) correct | ⬜ |
| 4 | **Authorities** | All legislation correct (TIOPA 2010 Parts 4, 9A, 10, ITA 2007 ss 720-730, etc.) | ⬜ |
| 5 | **Dates** | All dates correct | ⬜ |
| 6 | **Rates** | All rates match Golden Reference | ⬜ |
| 7 | **Calculations** | All CFC, ToAA, TP calculations correct | ⬜ |
| 8 | **Completeness** | All topics: CFC, ToAA, Insurance Bonds, Thin Cap/TP, DPT/Hybrids | ⬜ |
| 9 | **Topic Coverage** | Matches syllabus | ⬜ |

#### B-G. Other Checks

| Category | Items | Status |
|----------|-------|--------|
| B. Internal Consistency | 10-12 | ⬜ |
| C. Technical Accuracy | 13-16 | ⬜ |
| D. Arithmetic Accuracy | 17-19 | ⬜ |
| E. Usability | 20-22 | ⬜ |
| F. Strategic Alignment | 23-25 | ⬜ |
| G. Practical Application | 26-27 | ⬜ |

---

## Phase 5: Chapter 02 Part C - Specific Technical Questions

**Session**: 5 of 8-10
**Input**:
- `GOLDEN_REFERENCE_EXTRACT.md`
- `02_Major_Question_Types/Part_C_Specific_Technical_Questions.md`
- `02_Major_Question_Types/Part_C_Domicile_Template.md`
- Past Papers (Part C questions)
- Suggested Answers (Part C)

### Checklist

#### A. Content Accuracy

| # | Check Item | How to Verify | Status |
|---|------------|---------------|--------|
| 1 | **Past Paper References** | Verify all Part C questions cited are accurate | ⬜ |
| 2 | **Exam Structure** | Part C = Choose 2 of 5 × 15 marks each = 30 marks | ⬜ |
| 3 | **Exam Time** | Part C time allocation (~27 min each, ~54 total) correct | ⬜ |
| 4 | **Authorities** | All legislation correct for each topic area | ⬜ |
| 5 | **Dates** | All dates correct | ⬜ |
| 6 | **Rates** | All rates match Golden Reference | ⬜ |
| 7 | **Calculations** | All calculations correct | ⬜ |
| 8 | **Completeness** | Topics: Domicile, Trusts, TP, CIR, ATED, WHT, Exit Charges, IHT, Stamp/NIC/VAT | ⬜ |
| 9 | **Topic Coverage** | Matches syllabus | ⬜ |

#### B-G. Other Checks

| Category | Items | Status |
|----------|-------|--------|
| B. Internal Consistency | 10-12 | ⬜ |
| C. Technical Accuracy | 13-16 | ⬜ |
| D. Arithmetic Accuracy | 17-19 | ⬜ |
| E. Usability | 20-22 | ⬜ |
| F. Strategic Alignment | 23-25 | ⬜ |
| G. Practical Application | 26-27 | ⬜ |

---

## Phase 6: Chapter 03 - Cross-Cutting Skills

**Session**: 6 of 8-10
**Input**:
- `GOLDEN_REFERENCE_EXTRACT.md`
- `03_Cross_Cutting_Skills/Cross_Cutting_Skills_Complete.md`

### Checklist

#### A. Content Accuracy

| # | Check Item | How to Verify | Status |
|---|------------|---------------|--------|
| 1 | **Past Paper References** | Any examples from past papers are accurate | ⬜ |
| 2 | **Exam Structure** | Correct structure throughout (especially Part C = Choose 2 of 5) | ⬜ |
| 3 | **Exam Time** | 195 minutes, time allocations correct | ⬜ |
| 4 | **Authorities** | Case law and legislation citations correct | ⬜ |
| 5 | **Dates** | All dates correct | ⬜ |
| 6 | **Rates** | Any rates mentioned match Golden Reference | ⬜ |
| 7 | **Calculations** | All example calculations correct | ⬜ |
| 8 | **Completeness** | All 6 sections complete | ⬜ |
| 9 | **Topic Coverage** | Matches structure plan | ⬜ |

#### B-G. Other Checks

| Category | Items | Status |
|----------|-------|--------|
| B. Internal Consistency | 10-12 | ⬜ |
| C. Technical Accuracy | 13-16 | ⬜ |
| D. Arithmetic Accuracy | 17-19 | ⬜ |
| E. Usability | 20-22 | ⬜ |
| F. Strategic Alignment | 23-25 | ⬜ |
| G. Practical Application | 26-27 | ⬜ |

---

## Phase 7: Chapter 04 - Execution Excellence

**Session**: 7 of 8-10
**Input**:
- `GOLDEN_REFERENCE_EXTRACT.md`
- `04_Execution_Excellence/Execution_Excellence_Complete.md`

### Checklist

#### A. Content Accuracy

| # | Check Item | How to Verify | Status |
|---|------------|---------------|--------|
| 1 | **Past Paper References** | Any examples accurate | ⬜ |
| 2 | **Exam Structure** | Correct throughout | ⬜ |
| 3 | **Exam Time** | 195 minutes consistent | ⬜ |
| 4 | **Authorities** | Any citations correct | ⬜ |
| 5-7 | Dates, Rates, Calculations | Match Golden Reference | ⬜ |
| 8 | **Completeness** | All 4 sections complete | ⬜ |
| 9 | **Topic Coverage** | Matches structure plan | ⬜ |

#### B-G. Other Checks

| Category | Items | Status |
|----------|-------|--------|
| B. Internal Consistency | 10-12 | ⬜ |
| D. Arithmetic Accuracy | 17-19 | ⬜ |
| E. Usability | 20-22 | ⬜ |
| F. Strategic Alignment | 23-25 | ⬜ |
| G. Practical Application | 26-27 | ⬜ |

---

## Phase 8: Chapter 05 - Appendices (Deep Verification + Web Validation)

**Session**: 8 of 8-10
**Input**:
- `05_Appendices/Appendices_Complete.md`
- June 2025 Exam Paper (Tax Tables)
- ADIT UK Syllabus
- **Web searches for verification** (see Web Validation Framework above)

### Checklist

This phase verifies the Golden Reference source itself against primary sources AND web validation.

#### Tax Rates Verification

| Rate Type | Internal Source | Web Validation Required | Status |
|-----------|-----------------|------------------------|--------|
| Income Tax bands/rates | June 2025 Exam Tax Tables | Search: "UK income tax rates 2024/25" | ⬜ |
| Corporation Tax | June 2025 Exam Tax Tables | Search: "UK corporation tax rate 2024" | ⬜ |
| CGT rates | June 2025 Exam Tax Tables | Search: "UK CGT rates October 2024 budget" ⚠️ | ⬜ |
| IHT thresholds | June 2025 Exam Tax Tables | Search: "IHT nil rate band 2024/25" | ⬜ |
| NIC rates | June 2025 Exam Tax Tables | Search: "UK NIC rates 2024/25 changes" ⚠️ | ⬜ |
| SDLT rates | June 2025 Exam Tax Tables | Search: "SDLT thresholds 2025 changes" ⚠️ | ⬜ |
| VAT rates | June 2025 Exam Tax Tables | Search: "UK VAT rate registration threshold" | ⬜ |
| ATED bands | June 2025 Exam Tax Tables | Search: "ATED charges 2024/25" | ⬜ |
| Remittance basis charge | June 2025 Exam Tax Tables | Search: "non-dom remittance basis 2025 abolition" ⚠️ | ⬜ |

⚠️ = Known mid-year or upcoming changes - prioritize web validation

#### Legislation Verification

| Topic | Key Provisions | Web Validation | Status |
|-------|----------------|----------------|--------|
| SRT | FA 2013 Sch 45 | Search: "statutory residence test legislation" | ⬜ |
| Corporate Residence | CTA 2009 ss 14-18 | Search: "CTA 2009 corporate residence sections" | ⬜ |
| CFC | TIOPA 2010 Part 9A | Search: "TIOPA 2010 Part 9A CFC rules" | ⬜ |
| Transfer Pricing | TIOPA 2010 Part 4 | Search: "UK transfer pricing legislation TIOPA" | ⬜ |
| CIR | TIOPA 2010 Part 10 | Search: "corporate interest restriction legislation" | ⬜ |
| ToAA | ITA 2007 ss 720-730 | Search: "transfer of assets abroad ITA 2007" | ⬜ |
| Domicile | ITA 2007 s 835BA | Search: "deemed domicile ITA 2007 835BA" | ⬜ |
| Non-dom abolition | FA 2025 (expected) | Search: "FIG regime April 2025 legislation" ⚠️ | ⬜ |

#### Case Law Verification

For each case, verify via web search:

| Case | Verification Searches | Status |
|------|----------------------|--------|
| Gaines-Cooper v HMRC | "Gaines-Cooper 2011 residence principle" + "Gaines-Cooper still good law" | ⬜ |
| Smallwood v HMRC | "Smallwood treaty residence tie-breaker" | ⬜ |
| Furniss v Dawson | "Furniss Dawson principle current status" | ⬜ |
| Ramsay v IRC | "Ramsay principle tax avoidance" | ⬜ |
| (All other cases) | [Case name] + principle + "overruled OR distinguished" | ⬜ |

#### Exam Structure Web Verification

| Item | Web Validation | Status |
|------|----------------|--------|
| ADIT UK module structure | Search: "ADIT module 2.09 UK exam structure 2025" | ⬜ |
| Total exam time | Search: "ADIT exam duration 195 minutes" | ⬜ |
| Part structure | Search: "ADIT jurisdictional module Part A B C" | ⬜ |
| Marking scheme | Search: "ADIT exam marking criteria" | ⬜ |

#### Recent Changes Web Validation (Critical)

| Topic | Search Required | Priority | Status |
|-------|-----------------|----------|--------|
| CGT rate increase | "Autumn Budget 2024 CGT rates 18% 24%" | HIGH | ⬜ |
| SDLT surcharge increase | "SDLT additional property surcharge 5% October 2024" | HIGH | ⬜ |
| SDLT threshold reversion | "SDLT nil rate band April 2025 £125,000" | HIGH | ⬜ |
| Non-dom regime | "non-dom abolition FIG regime April 2025" | CRITICAL | ⬜ |
| BADR rate increase | "business asset disposal relief rate 14% 2025" | MEDIUM | ⬜ |
| NIC Class 2 changes | "Class 2 NIC voluntary 2024" | MEDIUM | ⬜ |

---

## Findings Log Template

Use this template to log issues found during QA:

```markdown
## QA Findings Log

### Session: [X] - [Chapter/Phase Name]
### Date: [YYYY-MM-DD]
### Reviewer: [Name]

---

### Critical Issues (Must Fix)

| # | Location | Issue | Correct Value | Status |
|---|----------|-------|---------------|--------|
| 1 | File:Line | Description | What it should be | ⬜ Fixed |

### Minor Issues (Should Fix)

| # | Location | Issue | Suggested Fix | Status |
|---|----------|-------|---------------|--------|
| 1 | File:Line | Description | Suggestion | ⬜ Fixed |

### Observations (Optional Fix)

| # | Location | Observation | Recommendation |
|---|----------|-------------|----------------|
| 1 | File:Line | Description | Suggestion |

---

### Session Summary
- Critical issues found: X
- Minor issues found: X
- Observations: X
- Time spent: X hours
```

---

## Quick Reference: The 27 Quality Check Items

### Category A: Content Accuracy
1. Past paper references accurate
2. Exam structure correct (questions per section, options)
3. Exam time correct (195 min)
4. Authorities (case law, legislation) correct
5. Dates correct
6. Rates correct
7. Calculations correct
8. Content complete
9. Topic coverage per structure

### Category B: Internal Consistency
10. Cross-chapter consistency
11. Template-to-example alignment
12. Cross-references valid

### Category C: Technical Accuracy
13. Legislation current
14. Case law valid
15. OECD Model version consistent
16. Formulas mathematically correct

### Category D: Arithmetic Accuracy
17. Mark totals (50+20+30=100)
18. Time allocations sum to 195 min
19. Minutes-per-mark (~1.95) consistent

### Category E: Usability
20. Acronyms defined
21. Terminology consistent
22. Tables render correctly

### Category F: Strategic Alignment
23. Examiner report alignment
24. Syllabus coverage complete
25. Professional marks guidance correct

### Category G: Practical Application
26. Timing realistic
27. Guidance actionable

### Category H: Web Validation
28. Web-verified against authoritative sources

---

## Prompt Templates for QA Sessions

### Session 1: Golden Reference Extraction

```
I need to create a Golden Reference Extract for the ADIT UK CheatBook QA process.

Please read the Appendices_Complete.md file and extract all verifiable facts into a compact reference format:

1. Exam structure (time, marks, questions per part)
2. All tax rates (2024/25)
3. All key definitions (one-line each)
4. All legislation citations
5. All case law principles
6. All formulas
7. All deadlines/time limits

Cross-verify the exam structure and tax rates against the June 2025 Exam Paper.

Output as GOLDEN_REFERENCE_EXTRACT.md
```

### Session 2-7: Chapter Verification

```
I am conducting QA on [Chapter X] of the ADIT UK CheatBook.

Please:
1. Read the GOLDEN_REFERENCE_EXTRACT.md (attached/provided)
2. Read [specific chapter file(s)]
3. Work through the Quality Check Protocol Phase [X] checklist
4. Log all findings using the Findings Log template

Focus especially on:
- [Specific concerns for this chapter]

Reference materials available:
- [List of past papers/suggested answers to verify against]
```

### Session 8: Deep Verification + Web Validation

```
I need to verify the source accuracy of the Appendices (Golden Reference source) using both internal documents AND web validation.

Please:
1. Verify all tax rates in Appendices_Complete.md against the June 2025 Exam Paper tax tables
2. For items marked with ⚠️ (mid-year changes), perform web searches to verify current rates
3. Verify legislation citations are correct and current
4. Verify case law principles are accurately stated and cases are still good law
5. Verify formulas are mathematically correct

Web Validation Focus Areas (search and verify):
- CGT rates (October 2024 budget changes)
- SDLT thresholds and surcharges (temporary vs permanent)
- Non-dom regime abolition (April 2025 FIG regime)
- NIC rate changes (Class 2 voluntary, Class 4 reduction)
- BADR rate increases (April 2025, 2026)
- ADIT exam structure (verify against tax.org.uk)

Log all findings including:
- Source searched
- Date of search
- Finding (correct/incorrect/needs update)
- Recommended action

Use the Web Validation Log template for each item checked.
```

### Web Validation Session (Standalone)

Use this prompt when performing dedicated web validation:

```
I need to perform web validation on specific items from the ADIT UK CheatBook.

Items to validate:
1. [Item 1 - e.g., "CGT rates post-October 2024"]
2. [Item 2 - e.g., "SDLT additional property surcharge"]
3. [Item 3 - e.g., "Non-dom regime abolition timeline"]

For each item:
1. Search using the query provided (or construct appropriate query)
2. Check 2-3 authoritative sources
3. Compare findings against CheatBook content
4. Log results in Web Validation Log format

Sources to prioritize:
- Government (gov.uk, HMRC)
- Professional bodies (CIOT, ICAEW)
- Major firms (Big 4 tax updates)
- Official legislation (legislation.gov.uk)

Flag any discrepancies for immediate correction.
```

### Ad-Hoc Web Validation

During any QA phase, if you encounter an item requiring web validation:

```
Web validation needed for: [ITEM]

Current CheatBook states: [WHAT THE DOCUMENT SAYS]

Please search to verify:
- Query: [SPECIFIC SEARCH QUERY]
- Look for: [WHAT TO CONFIRM]
- Sources to check: [RELEVANT SOURCE TYPES]

Report findings and recommend action if discrepancy found.
```

---

## Success Criteria

The CheatBook passes QA when:

- [ ] All 8 phases completed
- [ ] Zero critical issues remaining
- [ ] All minor issues addressed or documented as accepted
- [ ] Golden Reference Extract verified against primary sources
- [ ] **Web validation completed for all HIGH/CRITICAL priority items**
- [ ] **All ⚠️ flagged items verified against current authoritative sources**
- [ ] All findings logged and tracked
- [ ] Final sign-off recorded

---

## Summary: The 28 Quality Check Items

| # | Category | Check Item |
|---|----------|------------|
| 1 | A. Content | Past paper references accurate |
| 2 | A. Content | Exam structure correct |
| 3 | A. Content | Exam time correct (195 min) |
| 4 | A. Content | Authorities correct |
| 5 | A. Content | Dates correct |
| 6 | A. Content | Rates correct |
| 7 | A. Content | Calculations correct |
| 8 | A. Content | Content complete |
| 9 | A. Content | Topic coverage per structure |
| 10 | B. Consistency | Cross-chapter consistency |
| 11 | B. Consistency | Template-example alignment |
| 12 | B. Consistency | Cross-references valid |
| 13 | C. Technical | Legislation current |
| 14 | C. Technical | Case law valid |
| 15 | C. Technical | OECD Model version consistent |
| 16 | C. Technical | Formulas mathematically correct |
| 17 | D. Arithmetic | Mark totals correct |
| 18 | D. Arithmetic | Time allocations sum correctly |
| 19 | D. Arithmetic | Minutes-per-mark consistent |
| 20 | E. Usability | Acronyms defined |
| 21 | E. Usability | Terminology consistent |
| 22 | E. Usability | Tables render correctly |
| 23 | F. Strategic | Examiner report alignment |
| 24 | F. Strategic | Syllabus coverage complete |
| 25 | F. Strategic | Professional marks guidance correct |
| 26 | G. Practical | Timing realistic |
| 27 | G. Practical | Guidance actionable |
| 28 | H. Web Validation | Web-verified against authoritative sources |

---

*Protocol Version: 1.1*
*Created: November 2025*
*Updated: November 2025 - Added Web Validation Framework*
*For use with: ADIT UK CheatBook v1.0*
