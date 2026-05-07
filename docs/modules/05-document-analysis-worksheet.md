# Module 05: Document Analysis Worksheet

## Description

The Document Analysis Worksheet applies the Three-Layer Evidence Model to any uploaded document. Layer one classifies the source itself (Original, Derivative, or Authored). Layer two classifies the information within the source (Primary or Secondary, based on what the informant could have known firsthand). Layer three classifies the evidence produced by each fact claim (Direct, Indirect, or Negative). The OCR-HTR Transcription Tool v08 handles handwritten documents on upload. The Fact Extractor v4 then extracts discrete factual claims from the transcription. Each claim is individually classified and stored with its citation, ready for use in timelines, conflict analysis, and proof arguments.

## Key Inputs

- Uploaded document (image or scan)
- Citation record from Citation Builder (04) for the document being analyzed

## Key Outputs

- Transcription of the document text
- List of discrete factual claims extracted from the transcription
- Three-Layer classification for each claim: source type (Original/Derivative/Authored), information type (Primary/Secondary), evidence type (Direct/Indirect/Negative)

## GPS Touchpoints

- Applies the Three-Layer Evidence Model, the core analytical framework of the GPS
- Supports analysis and correlation of evidence (GPS element 3) by classifying every claim before it enters any proof argument
- Ensures Direct, Indirect, and Negative evidence are distinguished throughout

## Prompt Engines Used

- **OCR-HTR Transcription Tool v08** — transcribes handwritten and printed documents on upload
- **Fact Extractor v4** — extracts discrete factual claims from the transcription
- **GRA v8.5c** — GPS enforcement layer applied across all classification output

## Data Written to Supabase

- `documents` — document record with transcription text and file reference
- `citations` — evidence classification attached to each extracted fact claim

## Connection to Other Modules

- Receives citations from Citation Builder (04)
- Extracted and classified facts feed Timeline Builder (07) as dateable events
- Conflicting claims between documents surface in Source Conflict Resolver (06)
- Classified facts are used directly in Case Study Builder (10) proof arguments
- Transcriptions and fact lists are drawn into Research Report Writer (09)

## Status: Planning
