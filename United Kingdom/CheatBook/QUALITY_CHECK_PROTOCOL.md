# ADIT UK CheatBook - Quality Check Protocol

## Overview

This document provides a systematic protocol for quality-checking the entire ADIT UK CheatBook. Due to the size of the CheatBook (~320 pages), quality checks are designed to be executed in phases across multiple sessions.

**Target Audience**: QA reviewer using Claude Opus 4.5
**Estimated Sessions**: 8-10 sessions
**Prerequisites**: Access to Past Papers, Suggested Answers, ADIT UK Syllabus, June 2025 Exam Paper

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

## Phase 8: Chapter 05 - Appendices (Deep Verification)

**Session**: 8 of 8-10
**Input**:
- `05_Appendices/Appendices_Complete.md`
- June 2025 Exam Paper (Tax Tables)
- ADIT UK Syllabus
- UK Government sources for current rates

### Checklist

This phase verifies the Golden Reference source itself against primary sources.

#### Tax Rates Verification

| Rate Type | Verify Against | Status |
|-----------|----------------|--------|
| Income Tax bands/rates | June 2025 Exam Tax Tables | ⬜ |
| Corporation Tax | June 2025 Exam Tax Tables | ⬜ |
| CGT rates | June 2025 Exam Tax Tables | ⬜ |
| IHT thresholds | June 2025 Exam Tax Tables | ⬜ |
| NIC rates | June 2025 Exam Tax Tables | ⬜ |
| SDLT rates | June 2025 Exam Tax Tables | ⬜ |
| VAT rates | June 2025 Exam Tax Tables | ⬜ |
| ATED bands | June 2025 Exam Tax Tables | ⬜ |
| Remittance basis charge | June 2025 Exam Tax Tables | ⬜ |

#### Legislation Verification

| Topic | Key Provisions | Status |
|-------|----------------|--------|
| SRT | FA 2013 Sch 45 | ⬜ |
| Corporate Residence | CTA 2009 ss 14-18 | ⬜ |
| CFC | TIOPA 2010 Part 9A | ⬜ |
| Transfer Pricing | TIOPA 2010 Part 4 | ⬜ |
| CIR | TIOPA 2010 Part 10 | ⬜ |
| ToAA | ITA 2007 ss 720-730 | ⬜ |
| Domicile | ITA 2007 s 835BA | ⬜ |

#### Case Law Verification

Verify key cases are:
- Correctly named
- Principles accurately stated
- Still good law (not overturned)

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

### Session 8: Deep Verification

```
I need to verify the source accuracy of the Appendices (Golden Reference source).

Please verify all tax rates in Appendices_Complete.md against the June 2025 Exam Paper tax tables.

Also verify:
- Legislation citations are correct and current
- Case law principles are accurately stated
- Formulas are mathematically correct

Log any discrepancies found.
```

---

## Success Criteria

The CheatBook passes QA when:

- [ ] All 8 phases completed
- [ ] Zero critical issues remaining
- [ ] All minor issues addressed or documented as accepted
- [ ] Golden Reference Extract verified against primary sources
- [ ] All findings logged and tracked
- [ ] Final sign-off recorded

---

*Protocol Version: 1.0*
*Created: November 2025*
*For use with: ADIT UK CheatBook v1.0*
