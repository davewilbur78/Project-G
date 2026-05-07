# Module 14: DNA Evidence Tracker

## Description

The DNA Evidence Tracker integrates DNA match data with documentary evidence to support genealogical conclusions. The module allows the researcher to import or manually enter DNA match records, link matches to persons in the Supabase database, document the hypothesized relationship and the documentary evidence supporting it, and track the status of each match (identified, working hypothesis, unresolved). The tracker is designed with Ashkenazi Jewish endogamy in mind — matches are tagged with the relevant ancestral line being investigated, and the module surfaces which brick-wall lines have corroborating DNA evidence and which do not. DNA evidence is always treated as corroborating, not standalone proof.

## Key Inputs

- DNA match data (imported or manually entered): match name, platform, shared cM, shared segments
- Person records for identified or hypothesized matches
- Hypothesized relationship and the documentary evidence supporting it
- Ancestral line being investigated for each match

## Key Outputs

- Match records linked to person records in Supabase
- Status tracking per match: identified, working hypothesis, or unresolved
- Summary of corroborating DNA evidence by ancestral line and brick wall

## GPS Touchpoints

- DNA evidence is classified as corroborating indirect evidence under GPS — never treated as standalone proof (GPS element 3)
- Tracks which brick-wall lines have DNA corroboration and which do not, informing reasonably exhaustive search planning (GPS element 1)
- Endogamy context (Ashkenazi Jewish) is documented to explain elevated shared cM values that cannot be interpreted by standard relationship tables

## Prompt Engines Used

- **GRA v8.5c** — GPS enforcement layer applied to all evidence classification and output; enforces DNA-as-corroboration rule

## Data Written to Supabase

- `dna_matches` — match records linked to persons with status, hypothesized relationship, and supporting evidence
- `persons` — new person records created for DNA matches who are added to the database

## Connection to Other Modules

- Match persons are linked to existing person records from GEDCOM Bridge (01) and FAN Club Mapper (08)
- Documentary evidence supporting match hypotheses is drawn from Citation Builder (04) and Document Analysis Worksheet (05)
- Unresolved matches surface as action items in Research To-Do Tracker (15)

## Status: Planning
