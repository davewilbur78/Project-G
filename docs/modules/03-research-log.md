# Module 03: Research Log

## Description

The Research Log records every research session in structured, searchable form. For each session the log captures the date, the researcher's goal, each source searched (including those that yielded nothing — negative evidence is evidence), what was found or not found, and any follow-up actions generated. The Chat Conversation Abstractor v2 prompt engine can convert a freeform research conversation or session notes into a properly structured log entry. Entries are stored in Supabase and linked to the relevant person records and research plans, creating a complete, auditable research trail.

## Key Inputs

- Session date and researcher's stated goal
- Sources searched during the session, including those that yielded nothing
- Freeform session notes or research conversation (optionally converted by prompt engine)
- Links to relevant person records and research plans

## Key Outputs

- Structured log entry: date, goal, sources searched, finds, negatives, follow-up actions
- Complete, auditable research trail across all sessions

## GPS Touchpoints

- Documents reasonably exhaustive search (GPS element 1) by recording what was searched and not found
- Captures negative evidence, which is evidence under GPS
- Supports complete and accurate citations (GPS element 2) by linking each find to its source

## Prompt Engines Used

- **Chat Conversation Abstractor v2** — converts freeform session notes or conversations into structured log entries
- **GRA v8.5c** — GPS enforcement layer applied across all output

## Data Written to Supabase

- `research_sessions` — structured log entries linked to persons and research plans

## Connection to Other Modules

- Linked to Research Plan Builder (02) — sessions are conducted against active plans
- Newly found sources are passed to Citation Builder (04) and Document Analysis Worksheet (05)
- Negative searches and follow-up actions feed Research To-Do Tracker (15)
- Session records are drawn into Research Report Writer (09) to document the scope of research

## Status: Planning
