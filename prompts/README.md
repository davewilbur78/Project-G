# Prompt Engines

Project-G uses a set of open-source genealogical AI prompts developed by Steve Little as internal engines powering specific module features.

## Attribution

**Author:** Steve Little
**Project:** Open-Genealogy
**Repository:** github.com/DigitalArchivst/Open-Genealogy
**License:** [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

These prompts are used here strictly for **personal, non-commercial research**. Project-G is a private tool built for one user and is not distributed or sold. This usage is consistent with the CC BY-NC-SA 4.0 license.

---

## Prompt Engines in Use

### GRA v8.5c — Genealogical Research Assistant
The GPS enforcement layer. Runs across all modules as the foundational system prompt. Enforces Genealogical Proof Standard terminology, anti-fabrication rules, Three-Layer Evidence Model classification, and structured research methodology. This is the most important prompt in the system.

**Used in:** All modules (injected into every Claude API call)

---

### OCR-HTR Transcription Tool v08
Transcribes handwritten and printed historical documents from uploaded images. Handles 19th and early 20th century handwriting styles common in vital records, census records, and correspondence.

**Used in:** Module 05 — Document Analysis Worksheet

---

### Fact Extractor v4
Takes a transcribed document and extracts discrete factual claims as structured data. Each claim is tagged with the text it came from and the type of evidence it represents (direct, indirect, negative).

**Used in:** Module 05 — Document Analysis Worksheet

---

### Fact Narrator v4
Converts a set of extracted structured facts into coherent narrative prose for use in research reports and proof arguments.

**Used in:** Module 09 — Research Report Writer; Module 10 — Case Study Builder

---

### GEDCOM Analysis Assistant
Parses GEDCOM file content, identifies persons and relationships, evaluates citation quality, and flags gaps in documentation.

**Used in:** Module 01 — GEDCOM Bridge

---

### Image Citation Builder v2
Generates Evidence Explained-style citations for uploaded document images. Identifies source type (original/derivative/authored), information type (primary/secondary), and evidence type (direct/indirect/negative).

**Used in:** Module 04 — Citation Builder

---

### Chat Conversation Abstractor v2
Converts a research session conversation log into a structured research log entry, extracting what was searched, what was found, what was not found, and what follow-up actions are needed.

**Used in:** Module 03 — Research Log

---

### Research Agent Assignment v2.1
Takes a research question and target person profile and generates a structured research plan with prioritized source types to search, record repositories to check, and suggested search strategies.

**Used in:** Module 02 — Research Plan Builder

---

## Storage

Prompt files are stored in `prompts/gra/` and referenced by the AI layer in `src/lib/ai.ts`. They are not committed to any public repository. Original prompt files remain in the parent Open-Genealogy directory alongside this project.
