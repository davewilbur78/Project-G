# Module 15: Research To-Do Tracker

## Description

The Research To-Do Tracker is a running research agenda organized by person, priority, and source type. It aggregates follow-up actions from all other modules — unresolved research questions from the Research Plan Builder, negative searches that need retry, unanswered correspondence from the Correspondence Log, unresolved conflicts from the Source Conflict Resolver, and any manually added items. Each to-do is linked to the relevant person record and can be prioritized, assigned to a research session, and marked complete. The tracker provides a clear, actionable picture of where each line of research stands and what needs to happen next.

## Key Inputs

- Follow-up actions aggregated from all other modules (automated)
- Manually added research agenda items

## Key Outputs

- Prioritized research agenda organized by person, priority level, and source type
- Clear, actionable picture of where each line of research stands and what needs to happen next
- Completion tracking per item

## GPS Touchpoints

- Ensures no research leads are dropped, directly supporting reasonably exhaustive search (GPS element 1)
- Tracks unresolved conflicts (GPS element 4) and unanswered correspondence as active agenda items

## Prompt Engines Used

- **GRA v8.5c** — GPS enforcement layer applied across all output

## Data Written to Supabase

- `todos` — to-do records linked to relevant persons, with priority, source type, origin module, and completion status

## Connection to Other Modules

- Aggregates action items from: Research Plan Builder (02), Research Log (03), Source Conflict Resolver (06), Timeline Builder (07), Correspondence Log (12), and DNA Evidence Tracker (14)
- Completed items drive new sessions back into Research Log (03)
- Acts as the operational hub that connects all research activity across the platform

## Status: Planning
