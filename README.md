# Project-G: Personal Genealogy Operations Platform

A personal, private web application for serious hobbyist genealogical research. Built for one user. Not a product. Not for distribution.

Project-G is a working and documentation layer that sits alongside Ancestry.com and FamilyTreeMaker. It provides structured, GPS-compliant research tools that help an experienced hobbyist work with professional-grade methodology.

---

## The Platform

15 modular research tools, each self-contained but feeding shared data layers:

| # | Module | Purpose |
|---|--------|---------|
| 01 | GEDCOM Bridge | Parses GEDCOM exports, triages citation quality, pre-populates projects |
| 02 | Research Plan Builder | Structured planning with auto-generated research questions |
| 03 | Research Log | Session-by-session record of searches, finds, and negatives |
| 04 | Citation Builder | Evidence Explained-style citations for every source type |
| 05 | Document Analysis Worksheet | Three-Layer Model classifier (source/information/evidence) |
| 06 | Source Conflict Resolver | Side-by-side GPS conflict analysis |
| 07 | Timeline Builder | Visual chronological life timeline from all sources |
| 08 | FAN Club Mapper | Family, Associates, Neighbors network tracking |
| 09 | Research Report Writer | Formal narrative research report generator |
| 10 | Case Study Builder | GPS-compliant proof argument builder with PowerPoint export |
| 11 | Family Group Sheet Builder | Fully cited nuclear family unit documentation |
| 12 | Correspondence Log | Tracks research inquiries and responses |
| 13 | File Naming System | Standardized file naming and folder structure |
| 14 | DNA Evidence Tracker | Integrates DNA match data with documentary evidence |
| 15 | Research To-Do Tracker | Running research agenda by person and priority |

---

## Tech Stack

- **Frontend:** Next.js, React, Tailwind CSS
- **Backend:** Next.js API routes
- **Database:** Supabase (PostgreSQL)
- **AI:** Anthropic Claude API
- **File storage:** Supabase storage
- **Export:** python-pptx (Python endpoint)
- **Deployment:** Vercel

---

## Documentation

- [System Overview](docs/system-overview.md)
- [Architecture](docs/architecture.md)
- [Module Design Docs](docs/modules/)
- [Prompt Engines](prompts/README.md)

---

## Build Phases

1. **Phase 1** — Documentation and architecture *(current)*
2. **Phase 2** — Prototype artifacts in Claude.ai to test interview logic
3. **Phase 3** — Full web app built module by module
4. **Phase 4** — GEDCOM Bridge as onboarding layer
5. **Phase 5** — Case Study Builder with PowerPoint export as flagship

---

## Methodology

All modules follow the **Genealogical Proof Standard (GPS)** developed by the Board for Certification of Genealogists. GPS terminology is enforced throughout:

- Sources: Original, Derivative, or Authored
- Information: Primary or Secondary (refers to the informant's knowledge)
- Evidence: Direct, Indirect, or Negative

No genealogical data, citations, people, dates, or places are ever fabricated.

---

## About

Project-G is a private, single-user platform for an aspiring professional genealogist working toward BCG certification. It enforces the Genealogical Proof Standard across all research activities and serves as the working and documentation layer alongside Ancestry.com and FamilyTreeMaker. It is not a product and is not for distribution.
