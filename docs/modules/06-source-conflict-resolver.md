# Module 06: Source Conflict Resolver

## Description

The Source Conflict Resolver presents conflicting claims about the same fact side by side and guides the researcher through GPS-compliant conflict analysis. When two or more sources disagree about a date, name, place, or relationship, the module displays each source with its full Three-Layer classification, ranks the sources using the GPS preponderance hierarchy (Original over Derivative over Authored; Primary information over Secondary), and prompts the researcher to reason through which claim is best supported by the evidence. The outcome is a documented resolution note that becomes part of the proof argument for that fact, stored in Supabase and linkable to Case Study Builder entries.

## Key Inputs

- Two or more source records asserting conflicting claims about the same fact (date, name, place, or relationship)
- Three-Layer classifications for each source from Document Analysis Worksheet (05)

## Key Outputs

- Side-by-side display of conflicting sources with their full classifications
- GPS preponderance ranking of the sources (Original over Derivative over Authored; Primary over Secondary information)
- Researcher-authored resolution note documenting which claim is best supported and why

## GPS Touchpoints

- Directly addresses resolution of conflicting evidence (GPS element 4)
- Applies the GPS preponderance hierarchy to rank competing sources
- Resolution note becomes part of the proof argument, satisfying the requirement for a soundly reasoned written conclusion (GPS element 5)

## Prompt Engines Used

- **GRA v8.5c** — GPS enforcement layer governs all conflict analysis and resolution language

## Data Written to Supabase

- TBD — requires design decision (resolution notes link to existing citation records or a separate conflicts table not yet defined in architecture)

## Connection to Other Modules

- Draws source classifications from Document Analysis Worksheet (05)
- Resolution notes feed Case Study Builder (10) as documented conflict resolutions
- Resolved conflicts are referenced in Research Report Writer (09)
- Unresolved conflicts surface as action items in Research To-Do Tracker (15)

## Status: Planning
