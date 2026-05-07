# Module 12: Correspondence Log

## Description

The Correspondence Log tracks all outgoing research inquiries and their responses — letters to courthouses, emails to archives, requests to repositories, queries to other researchers, and DNA match outreach. For each inquiry the log records the date sent, the recipient, the repository or person contacted, the specific question asked, the date of response (if any), and the outcome. Unanswered inquiries surface as follow-up items in the Research To-Do Tracker. The log creates a complete record of who has been contacted about what, preventing duplicate outreach and documenting the research trail for GPS compliance.

## Key Inputs

- Outgoing inquiry details: date sent, recipient name, repository or person contacted, specific question asked
- Response received: date, outcome, any records provided

## Key Outputs

- Log entry per inquiry with full tracking fields
- Follow-up flags for unanswered inquiries, surfaced to Research To-Do Tracker (15)
- Complete record preventing duplicate outreach

## GPS Touchpoints

- Documents the full scope of outreach as part of reasonably exhaustive search (GPS element 1)
- Creates an auditable research trail showing what was requested, from whom, and when — a GPS compliance requirement

## Prompt Engines Used

- **GRA v8.5c** — GPS enforcement layer applied to all output

## Data Written to Supabase

- `correspondence` — inquiry records with date, recipient, question, response date, and outcome

## Connection to Other Modules

- Unanswered inquiries automatically surface as follow-up items in Research To-Do Tracker (15)
- Responses that yield new records are passed to Citation Builder (04) and Document Analysis Worksheet (05)

## Status: Planning
