# Module 01: GEDCOM Bridge

## Description

The GEDCOM Bridge is the onboarding layer for Project-G. It accepts a GEDCOM export from FamilyTreeMaker, parses all persons and relationships, and evaluates the quality of existing citations using a Green/Yellow/Red triage system. Green citations are fully formed and citable; Yellow citations are partial or informal; Red citations are missing or unusable. The module flags documentation gaps, surfaces persons with no sources, and pre-populates the Supabase database with structured person and source records ready for use across all other modules. The GEDCOM Analysis Assistant prompt engine powers the parsing and evaluation layer.

## Status: Planning
