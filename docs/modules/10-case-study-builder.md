# Module 10: Case Study Builder

## Description

The Case Study Builder is the flagship module. It guides the researcher through building a GPS-compliant proof argument for a complex genealogical conclusion — typically an identity, parentage, or relationship claim that cannot be established by a single direct-evidence source. The module structures the argument using the five GPS elements: reasonably exhaustive search, complete and accurate citations, analysis and correlation of evidence, resolution of conflicting evidence, and soundly reasoned written conclusion. The Fact Narrator v4 engine produces narrative prose from the structured argument. Finished case studies export to PowerPoint via the python-pptx endpoint, producing a slide deck suitable for archival or presentation.

## Key Inputs

- Research question (typically an identity, parentage, or relationship claim)
- All relevant sources, citations, and Three-Layer classifications
- Conflict resolution notes from Source Conflict Resolver (06)
- Timeline data and extracted facts

## Key Outputs

- Structured GPS-compliant proof argument addressing all five GPS elements
- Narrative prose proof argument
- PowerPoint export (.pptx) suitable for archival or presentation

## GPS Touchpoints

- Addresses all five GPS elements explicitly:
  1. Reasonably exhaustive search — documented scope of research
  2. Complete and accurate citations — every claim cited
  3. Analysis and correlation of evidence — all evidence examined and correlated
  4. Resolution of conflicting evidence — conflicts documented and resolved
  5. Soundly reasoned written conclusion — the proof argument itself

## Prompt Engines Used

- **Fact Narrator v4** — generates narrative prose from the structured proof argument
- **GRA v8.5c** — GPS enforcement layer applied to all argument structure and language

## Data Written to Supabase

- TBD — requires design decision (case study storage table not yet defined in architecture)

## Connection to Other Modules

- Primary consumer of output from Source Conflict Resolver (06), Timeline Builder (07), Document Analysis Worksheet (05), and Citation Builder (04)
- Case study conclusions may be incorporated into Research Report Writer (09)
- PowerPoint export is delivered via the python-pptx endpoint defined in architecture

## Status: Planning
