# Changelog

## 2026-05-07 -- Case Study Builder Prototype, Singer/Springer Research Session

### Session type
Phase 2 prototype work -- Module 10 (Case Study Builder)

### Test case established
Jacob Singer / Yankel Springer identity proof selected
as the Module 10 test case. Research question: Is Yankel
Springer of Lechowitz, Volhynia the same person as Jacob
Singer who appears in New York City records from 1915
onward?

### Research work completed
Full working research session conducted on the Singer /
Springer case. The following was accomplished:

- GEDCOM file (jack_singer.ged) parsed and triaged.
  Subject record @I327@ identified with five documented
  name variants across 14+ sources. Citation quality
  triage: 12 Green, 2 Yellow, 3 Red.

- 1919 Naturalization Petition (NARA M1972, Roll 1114)
  fully transcribed and analyzed across all four panels
  using cropped and enhanced image analysis. Key
  findings: born 3 Dec 1895, Volhynia, Russia; arrived
  S.S. Marion, Nov 28, 1907, from Antwerp; filed under
  WWI military bypass (Act of May 9, 1918); Certificate
  of Arrival says Singer, Yankel.

- 1907 Passenger Manifest (S.S. Marion, T715, List 22)
  fully transcribed and analyzed. Row 17: Yankel
  Springer, age ~11, born Lechowce. Family group rows
  16-19 all Springer. Contact in America: Schmuel
  Springer. Confirms family surname was Springer at
  time of arrival.

- Seven-link evidence chain constructed connecting
  Yankel Springer to Jacob Singer across place of
  origin, birth year, vessel, arrival date, father
  identity, address continuity, government
  certification, and continuous residence.

- Two conflicts identified and analyzed: (1) Springer
  vs. Singer naming across manifest and Certificate of
  Arrival -- resolved by timeline analysis. (2) Mother
  Chine Springer (manifest) vs. Minnie Jacobs (family
  records) -- unresolved, filed as separate research
  question.

### Deliverables produced
- Singer_Springer_Research_Record.docx -- professional
  Word document capturing all research findings,
  source triage, evidence chain, conflict analysis,
  proof argument draft, and next research steps.

- case_study_builder.html -- Case Study Builder
  prototype v1. Five-stage interactive tool with
  Singer/Springer data pre-loaded. All sources,
  evidence chain, conflict analysis, and pre-written
  proof argument.

- case_study_builder_v2.html -- Case Study Builder
  prototype v2. Added full Evidence Explained citation
  layer (full citation + short footnote form for every
  source), footnoted proof argument (every factual claim
  carries an inline superscript keyed to a footnotes
  section), and removed all GEDCOM references from
  researcher-facing output.

### Design decisions made (now firm rules)

GEDCOM as infrastructure: The GEDCOM file is plumbing.
It never appears in researcher-facing output, is never
cited, and GEDCOM IDs never surface in reports or proof
arguments. Added to CLAUDE.md as a firm rule.

Ancestry tree links are not sources: Links to other
users' Ancestry trees must be flagged and rejected as
evidence. The researcher must locate the underlying
original. Added to CLAUDE.md as a firm rule.

FamilySearch ark: identifiers are valuable: These are
stable database IDs and belong in citations. Preserved
in all output.

Two output modes: The platform produces a researcher /
professional output (GPS language, EE citations, full
footnotes) and a client output (plain English narrative,
methodology invisible). Both come from the same data.
Module 9 and Module 10 must implement both modes.

Researcher view vs. client view: The working interface
(what the researcher sees while building the case) is
dense and technical -- GPS labels, EE citations,
Three-Layer analysis. This is the cockpit. The output
documents are what clients and examiners receive. The
two must never be confused.

### Wishlist items added to CLAUDE.md
- Document viewer: source images render inline in the
  source record panel. Stored in Supabase, displayed
  alongside the citation.
- Reasonably Exhaustive Search checklist: its own
  dedicated stage in the Case Study Builder, between
  Evidence Chain and Conflict Analysis.

### Next research steps (Singer/Springer case)
1. Verify manifest address (~197 Mason[?] St) against
   NYC city directories, 1907-1912.
2. Retrieve and examine Seaman's Protection Certificate
   (NARA RG 41, Box 225).
3. Search Samuel Singer/Springer naturalization records
   for first papers predating 1907.
4. Research Chine Springer (manifest) vs. Minnie Jacobs
   (family records) as a separate research question.
5. Search Lachovitz / Lechowitz metrical books at DAO
   Khmelnytskyi Oblast for 1895 birth record.
6. Search 1910 federal census for Singer/Springer
   household at Madison St, New York.

### Next prototype work
- Add Reasonably Exhaustive Search stage to Case Study
  Builder (between Stage 3 and Stage 4).
- Add EE citation builder interview to Stage 2 so
  citations are constructed interactively, not
  pre-loaded.
- Begin Module 9 (Research Report Writer) prototype
  with two output modes.

## [2.0] - 2026-05-07 UTC

### Operating Model Established
- CLAUDE.md designated as single source of truth for all project instructions
- Version numbering and UTC timestamp system added to CLAUDE.md
- Operating Model section added to CLAUDE.md explaining the single source of truth architecture
- Claude.ai project instructions box simplified to a single pointer to CLAUDE.md
- Claude Code working directory locked to /Users/dave/project-g/
- .claude/ added to .gitignore to prevent Claude Code worktree dirs from being tracked
- Claude Code working directory instruction added to CLAUDE.md

### Phase 1 Completion Documented
- CLAUDE.md updated with BCG certification framing
- Phase 1 marked complete, Phase 2 marked active
- README About section added
- All 15 module docs audited and expanded

## [Unreleased]
- Phase 2 active: Case Study Builder prototype in development

## [Phase 1 Complete]
- Full folder structure established
- CLAUDE.md master reference created
- README.md created
- System overview doc created
- Architecture doc created
- All 15 module planning docs created
- Prompts README created documenting Steve Little prompt engine assignments
