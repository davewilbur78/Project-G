# Module 09: Research Report Writer

## Description

The Research Report Writer generates formal narrative research reports in GPS-compliant style. A research report documents the scope of a research project, the sources searched (including those that yielded nothing), what was found, and the conclusions reached — with full citations embedded in the narrative. The Fact Narrator v4 prompt engine converts structured extracted facts into coherent narrative prose. The report writer pulls data from the Research Log, Timeline Builder, and Document Analysis Worksheets to assemble a complete, auditable account of the research conducted for a given person or question. Reports are formatted for human review and can be exported to Word or PDF.

## Key Inputs

- Research scope and question
- Research Log sessions for the relevant person or project
- Timeline Builder data for the subject
- Document Analysis Worksheets and classified fact lists

## Key Outputs

- Formal narrative research report with embedded Evidence Explained-style citations
- Documents the scope, sources searched (including negatives), findings, and conclusions
- Exportable to Word or PDF

## GPS Touchpoints

- Fulfills the GPS requirement for a soundly reasoned written conclusion (GPS element 5)
- Documents reasonably exhaustive search (GPS element 1) by narrating what was and was not found
- Embeds complete and accurate citations (GPS element 2) throughout the narrative

## Prompt Engines Used

- **Fact Narrator v4** — converts structured extracted facts into coherent narrative prose
- **GRA v8.5c** — GPS enforcement layer applied to all generated text

## Data Written to Supabase

- TBD — requires design decision (report storage format and table not yet defined in architecture)

## Connection to Other Modules

- Draws from Research Log (03), Timeline Builder (07), and Document Analysis Worksheet (05)
- May incorporate Case Study Builder (10) proof arguments for complex conclusions
- Family Group Sheet Builder (11) data provides the foundational person and family facts for the narrative

## Status: Planning
