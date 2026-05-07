---
Project-G CLAUDE.md
Version: 2.0
Last updated: 2026-05-07 UTC
---

## Operating Model

This file is the single source of truth for Project-G. 
It lives in the GitHub repository at:
https://github.com/davewilbur78/Project-G/blob/main/CLAUDE.md

The Claude.ai project instructions box contains only a 
pointer to this file. All actual instructions live here.

Every time this file is updated, the version number 
increments and the Last updated timestamp is refreshed 
to the current date in UTC. Claude Code is responsible 
for updating the timestamp and version on every commit 
that changes this file.

When Claude reads this file at the start of a conversation, 
it should confirm the version and date out loud so the 
user knows exactly which version is being used.

# Project-G: Personal Genealogy Operations Platform

## What This Is

Project-G is a personal, private web application supporting serious genealogical research and professional development. It is built for one user only and will never be distributed or sold. It is a working layer that sits on top of existing tools like Ancestry.com and FamilyTreeMaker — not a replacement for them.

The platform is a suite of modular research tools that help an aspiring professional genealogist actively working toward BCG (Board for Certification of Genealogists) certification apply professional-grade methodology in daily research practice. This platform is part of that professional development path. Everything in this system follows the Genealogical Proof Standard (GPS) developed by the Board for Certification of Genealogists, but translated into plain language.

## The Modules

The platform has 15 modules. Each has a design document in docs/modules/.

1. GEDCOM Bridge — onboarding wizard that parses FamilyTreeMaker GEDCOM exports, triages citation quality (Green/Yellow/Red), flags gaps, and pre-populates projects
2. Research Plan Builder — structured research planning with auto-generated research questions
3. Research Log — session-by-session record of what was searched, found, and not found
4. Citation Builder — Evidence Explained-style citations for every source type
5. Document Analysis Worksheet — Three-Layer Model classifier (source/information/evidence)
6. Source Conflict Resolver — side-by-side conflict analysis using GPS preponderance hierarchy
7. Timeline Builder — visual chronological life timeline built from all sources
8. FAN Club Mapper — Family, Associates, Neighbors network tracking
9. Research Report Writer — formal narrative research report generator
10. Case Study Builder — GPS-compliant proof argument builder with PowerPoint export
11. Family Group Sheet Builder — fully cited nuclear family unit documentation
12. Correspondence Log — tracks all outgoing research inquiries and responses
13. File Naming System — standardized file naming and folder structure generator
14. DNA Evidence Tracker — integrates DNA match data with documentary evidence
15. Research To-Do Tracker — running research agenda organized by person and priority

## Prompt Engines (Third-Party)

This project incorporates open-source prompts from Steve Little's Open-Genealogy project (github.com/DigitalArchivst/Open-Genealogy), licensed CC BY-NC-SA 4.0, used here for personal non-commercial research only.

The following Steve Little prompts are used as internal engines inside our modules:
- OCR-HTR Transcription Tool v08 — powers document transcription on upload
- Fact Extractor v4 — extracts discrete factual claims from transcribed documents
- Fact Narrator v4 — turns extracted facts into narrative prose
- GEDCOM Analysis assistant — powers the GEDCOM Bridge parsing layer
- Image Citation Builder v2 — powers citation generation for uploaded images
- Chat Conversation Abstractor v2 — powers Research Log session summaries
- Research Agent Assignment v2.1 — powers Research Plan Builder logic
- GRA v8.5c — GPS enforcement layer running across all modules

## Tech Stack

- Frontend: Next.js with React and Tailwind CSS
- Backend: Next.js API routes
- Database: Supabase (PostgreSQL)
- AI: Anthropic Claude API (claude-sonnet-4-5 model)
- File storage: Supabase storage bucket
- PowerPoint export: python-pptx via a lightweight Python endpoint
- Deployment: Vercel (eventual)

## Build Path

Phase 1: Documentation and architecture (complete)
Phase 2: Prototype artifacts in Claude.ai to test interview logic (active — current phase)
Phase 3: Full web app built module by module via Claude Code
Phase 4: GEDCOM Bridge built as onboarding layer
Phase 5: Case Study Builder with PowerPoint export as flagship feature

## Coding Standards

- Never fabricate genealogical data, citations, sources, people, dates, or places
- GPS terminology is strictly enforced throughout the UI and all generated text
- Sources are Original, Derivative, or Authored — never "primary source" or "secondary source"
- Evidence is Direct, Indirect, or Negative — never "primary evidence" or "secondary evidence"
- Primary and Secondary apply only to Information (informant's knowledge)
- Every fact in the system must have a source citation attached
- Components are modular — each module is self-contained but feeds shared data layers
- Supabase schema is the single source of truth for all person and source data

## Important Context

- The user has years of existing research in Ancestry.com and FamilyTreeMaker
- The user is an aspiring professional genealogist actively working toward BCG certification
- Ancestry stays the tree; this platform is the working and documentation layer
- The Greene/Greenspun family line is an active unsolved research project — do not use as a test case
- The platform integrates with an existing Ashkenazi DNA genealogy workflow

## Claude Code Instructions

Always work in /Users/dave/project-g/. 
Prepend cd /Users/dave/project-g && to every bash command.
Never write files to any other directory.
