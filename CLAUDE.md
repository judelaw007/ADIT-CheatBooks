# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

ADIT-CheatBooks is a structured exam preparation content library for the **Advanced Diploma in International Taxation (ADIT)**. It is primarily a content-as-code repository (95% Markdown, 5% Python tooling) — not a traditional software project.

A "CheatBook" is a last-minute exam preparation resource for the final 4 weeks before an exam, focused on application, pattern recognition, and strategic execution under time pressure. See `What_is_a_CheatBook.md` for the full methodology.

## Commands

### Convert Markdown to Word Document
```bash
python create_enhanced_docx.py <input.md> <output.docx>
```
Requires `python-docx` (`pip install python-docx`). There is also `create_enhanced_docx_optimized.py` for faster processing of large (1000+ line) files — same interface.

## Content Architecture

### Module Organization

Each ADIT module gets its own top-level directory. Completed modules have a `CheatBook/` subdirectory with full content. Planned modules currently only have syllabus files at the root.

| Module | Directory | Status |
|--------|-----------|--------|
| UK (2.09) | `United Kingdom/CheatBook/` | Complete |
| Energy Resources (3.04) | `Energy Resources/` | Complete |
| US (2.10), EU DT, Banking, EU VAT | Root-level syllabus `.md` files | Syllabus only |

### Standard CheatBook Structure (per module)

Every CheatBook follows a consistent 4-section + appendices architecture:

1. **Battlefield Intelligence** (~10-15%) — Exam architecture analysis, historical question patterns, examiner psychology, question spotting
2. **Major Question Types** (~60-70%) — Template-driven frameworks for each question archetype with fill-in-the-blank structures and timing guidance
3. **Cross-Cutting Skills** (~10-15%) — Universal exam techniques applicable across topics
4. **Execution Excellence** (~5-10%) — Exam day strategy, time management, error catalogs
5. **Appendices** (~10-15%) — Quick reference: rates, definitions, formulas, case law

### Content Conventions

- Every concept includes a ready-to-use execution template with minute-level time allocations
- Content is organized by exam structure and mark value, not by textbook topic order
- Each concept appears once; other sections cross-reference rather than duplicate
- Chapters include `.md` source files and may have corresponding `.docx` exports
- Past exam papers and suggested answers are stored in per-module `Past Papers/` or `Past Questions/` directories

## Writing New CheatBook Content

When creating or extending a CheatBook module:

- Follow the 4-section structure above — see `United Kingdom/CheatBook/CHEATBOOK_STRUCTURE_PLAN.md` or `Energy Resources/Energy Resources CheatBook Structure Plan.md` for detailed blueprints
- Use the syllabus files (e.g., `ADIT_US_Syllabus_2026.md`) as the authoritative source for topic coverage and learning-level expectations (Bloom's Taxonomy levels 1-3)
- Apply the quality standards in `United Kingdom/CheatBook/QUALITY_CHECK_PROTOCOL.md`
- Commit messages follow the pattern: `Add Chapter X: [Topic Name]`
