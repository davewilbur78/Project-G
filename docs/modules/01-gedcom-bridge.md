# Module 01: GEDCOM Bridge

## Description

The GEDCOM Bridge is the onboarding layer for Project-G. It accepts a GEDCOM export from FamilyTreeMaker, parses all persons and relationships, and evaluates the quality of existing citations using a Green/Yellow/Red triage system. Green citations are fully formed and citable; Yellow citations are partial or informal; Red citations are missing or unusable. The module flags documentation gaps, surfaces persons with no sources, and pre-populates the Supabase database with structured person and source records ready for use across all other modules. The GEDCOM Analysis Assistant prompt engine powers the parsing and evaluation layer.

## Key Inputs

- GEDCOM file exported from FamilyTreeMaker

## Key Outputs

- Populated `persons` and `sources` tables in Supabase
- Citation triage report classifying each existing citation as Green (fully formed), Yellow (partial or informal), or Red (missing or unusable)
- List of persons with no sources, surfaced as gaps for follow-up

## GPS Touchpoints

- Establishes the baseline citation quality for all imported research
- Flags missing and unusable citations to enforce the GPS requirement for complete and accurate citations (GPS element 2)
- Surfaces undocumented persons to support reasonably exhaustive search planning (GPS element 1)

## Prompt Engines Used

- **GEDCOM Analysis assistant** — parses the GEDCOM structure and evaluates citation quality
- **GRA v8.5c** — GPS enforcement layer applied across all analysis

## Data Written to Supabase

- `persons` — individual records imported from the GEDCOM
- `sources` — source records extracted from GEDCOM citation fields
- `citations` — links between person facts and sources, with triage classification

## Connection to Other Modules

- Feeds person and source records to all other modules
- Yellow and Red citations queue for remediation in Citation Builder (04)
- Persons with no sources surface as action items in Research To-Do Tracker (15)
- Pre-populated persons are the starting point for Research Plan Builder (02), Timeline Builder (07), and Family Group Sheet Builder (11)

## Status: Planning
