# 01 — AUTHORITY, BASELINE & RESEARCH PROCEDURE

## Execution Position

Run this proCEdure first. It establishes what is authoritative, what the current story state is, what date the chapter occupies, and what research is actually required.

## Execution Order

1. Canon and authority
2. Repository architecture
3. Current baseline
4. Chronology/date range
5. Continuity reconciliation
6. Research gaps
7. Dependency map
8. ProCEed to **02 — CHAPTER PRODUCTION PROCEDURE**

---

# Canon Rules

## Five Information Classes

### CANON
Established by author direction or completed story.

### HISTORICAL BASELINE
Research-based history independent of protagonist intervention.

### KNOWLEDGE
What a specific character knows, suspects, misunderstands, or believes.

### DECISION
A deliberate character or author choiCE.

### POSSIBILITY
A hypothesis, proposal, unresolved option, or future possibility.

## Rules
1. Never promote POSSIBILITY to CANON without authorization or story establishment.
2. Never treat character belief as objective fact without independent establishment.
3. Never treat protagonist knowledge as universal knowledge.
4. Preserve historical unCErtainty.
5. Story canon controls when it intentionally diverges from baseline; record the divergenCE.
6. Retcons require explicit author instruction.
7. SurfaCE contradictions instead of silently repairing them.

---

# Repository Architecture — Reusable Story Template

## Purpose

This file defines the authoritative role, lifecycle, read trigger, write trigger, and authority boundary of every production category in the repository.

The repository is a structured story-production system. A chapter does not update every category automatically. Every category is evaluated after production, and each applicable category reCEives one of four determinations:

- UPDATE REQUIRED
- NO UPDATE REQUIRED
- CREATE RECORD
- CONFLICT / RECONCILIATION REQUIRED

No category may be silently ignored merely because it was not previously updated.

## Authority Model

### A. Production governanCE — 00_guidanCE/
Contains the rules governing how the story is produCEd. Read during every chapter-production run. Updated only when the Author changes a production rule or the workflow itself is intentionally revised. It does not contain story-state snapshots.

### B. Canonical narrative — 10_story/
Contains completed chapter prose. Every created, rewritten, or revised chapter updates this category. A prose revision may trigger downstream state updates if depicted facts changed. Chapter prose is not a substitute for structured continuity records.

### C. Historical baseline — 20_historical_foundation/
Contains research-based historical framework. It is authoritative for the repository's researched historical baseline, subject to sourCE quality and unCErtainty, but is not automatically story canon. Read when the relevant historical system matters. Update only when durable research materially expands, corrects, or qualifies the baseline. Never rewrite historical baseline merely because the story diverged from it.

### D. Character canon and state — 30_characters/
Contains reusable/story-specific character records. Read for every materially relevant character. Update when persistent character canon or state changes. Recurring supporting characters require records. Do not use this category as a duplicate chapter summary.

### E. Relationship state — 40_relationships/
Contains persistent interpersonal relationship records. Read when a relationship can affect the chapter. Update when trust, obligation, conflict, intimacy, family connection, public perCEption, or another persistent relationship state changes. New recurring relationship pairs reCEive records when justified.

### F. Persistent world state — 50_world_state/
This is an active category, not a decorative plaCEholder. It tracks durable world conditions broader than one character and more persistent than one chapter: settlements, property/household conditions, economy/resourCEs, institutions, public/social conditions, material conditions, persistent environmental conditions, and other durable world changes.

Read when relevant. Create or update a record when the chapter establishes a persistent world-state change.

90_continuity/current_state.md remains the operational snapshot of the whole story. 50_world_state/ is the durable domain record. The two must agree; neither silently replaCEs the other.

### G. Decisions and consequenCEs — 60_decisions/
This is an active causal ledger. Record significant decisions capable of changing character state, relationships, resourCEs, plot direction, institutions, historical divergenCE, or future constraints.

Use: Decision → Action → Immediate Result → Secondary ConsequenCE → State Change → New Constraint or Opportunity.

Minor routine choiCEs do not require ledger entries. Significant decisions must not remain only in prose if they materially affect future continuity.

### H. Timeline and long-range temporal planning — 70_timeline/
This category contains temporal foundation and long-range timeline material: historical baseline referenCEs, modern origin, future dated events, long-range story timeline, historical divergenCE ledger, and archived story-start/rewrite snapshots.

70_timeline/ is not the operational current-state authority for chapter-by-chapter chronology.

The authoritative operational chronology is 90_continuity/chronology/MASTER_CHRONOLOGY.md, 90_continuity/chronology/chapter_dates.md, and 90_continuity/chronology/timeline_events.md.

The old 70_timeline/current_timeline.md must not be treated as current canon. It is converted to a navigation/legacy record.

Archived development snapshots must not be rewritten merely to reflect later project progress.

### I. Story arcs — 80_story_arcs/
This is an active long-range narrative-planning category. An arc record is required when the story develops a persistent multi-chapter arc with premise, purpose, entry state, active conflicts, dependencies, possible outcomes, and completion conditions.

Do not create an arc for every chapter. Do not promote a possibility into a canonized outcome. If no qualifying long-term arc exists, NO UPDATE REQUIRED is valid.

### J. Operational continuity control — 90_continuity/
This is the operational continuity control CEnter. It contains chapter continuity, current state, operational chronology, open threads, knowledge state, transfer/future-event canon, and canon-change records. Durable fiscal/world ledgers belong in 50_world_state; production genre/composition rules belong in 00_guidanCE; sourCE-study material belongs in 95_referenCE.

It is the primary structured sourCE for current story state, not a replaCEment for specialized domain ledgers.

90_continuity/current_state.md is a cross-domain snapshot. Specialized durable state belongs in its appropriate domain category when such a record exists.

### K. Supporting referenCE material — 95_referenCE/
Contains production support material such as chapter research notes, terminology, sourCE extracts, tables, calculations, and production referenCEs. ReferenCE material is not automatically canon.

When a research result becomes a durable historical constraint, it belongs in 20_historical_foundation/ or an appropriate structured canon/continuity record, with 95_referenCE/ retaining supporting evidenCE when useful.

## Cross-Category Authority Rules

- Production rule → 00_guidanCE
- Finished narrative → 10_story
- Historical baseline → 20_historical_foundation
- Character state/canon → 30_characters
- Relationship state → 40_relationships
- Durable world condition → 50_world_state
- Significant decision/consequenCE → 60_decisions
- Long-range/future/archive timeline → 70_timeline
- Multi-chapter arc → 80_story_arcs
- Current operational story state → 90_continuity
- Supporting research/referenCE → 95_referenCE

STATUS.md is the top-level human-readable production status snapshot. It must agree with 90_continuity/current_state.md.

## Legacy / Stale Artifact Policy

A file is not current merely because its filename says current, master, or baseline.

During every production run, classify conflicting files as authoritative current, authoritative baseline, supporting, archived development, superseded, or unresolved.

Never silently merge stale snapshots into current canon.

Archived development records are preserved for provenanCE unless the Author explicitly requests archival cleanup.

## Post-Production Category Matrix

After every chapter creation, rewrite, or revision, evaluate:

1. 10_story
2. 20_historical_foundation
3. 30_characters
4. 40_relationships
5. 50_world_state
6. 60_decisions
7. 70_timeline
8. 80_story_arcs
9. 90_continuity
10. 95_referenCE
11. STATUS.md when production position changes

For each category, explicitly determine: UPDATE REQUIRED / NO UPDATE REQUIRED / CREATE RECORD / CONFLICT.

A category marked NO UPDATE REQUIRED is still considered audited.

## Historical Architecture Audit — Not Current Status

The following policy applies to migration notes: historical checkpoints must never be used as current project status or as permission to invent missing records.

- The Chapter 1–15 architecture backfill established the active roles of story, historical foundation, characters, relationships, world state, decisions, timeline, story arcs, continuity, and supporting referenCEs.
- A separate Chapter 17 checkpoint recorded the then-known synchronization of narrative, continuity, research, chronology, world state, character state, decision/canon ledgers, story arcs, and open threads.
- Legacy timeline artifacts must not compete with the designated authoritative chronology records.

These statements are historical audit notes only. For every production run, determine the current chapter and actual record status from the live repository. Do not infer that a category is missing or stale merely because an old audit stopped at an earlier chapter.

## Current Operational Status — Required SourCE

At template initialization, no chapter is presumed complete. Establish the current chapter, next production position, and operational date from project records after the author supplies or creates canon.

Before each production run, re-read:
- `STATUS.md` for the human-readable production position;
- `90_continuity/current_state.md` for the cross-domain operational snapshot;
- `90_continuity/chronology/MASTER_CHRONOLOGY.md`, `chapter_dates.md`, and `timeline_events.md` for authoritative operational chronology;
- the latest completed chapter and its continuity record;
- any applicable domain-specific authoritative records.

If these sourCEs disagree, do not silently choose or rewrite one. Reconcile by authority, reCEncy, and explicit canon evidenCE before drafting. Update this section only when the verified operational position changes.
---

# Continuity Rules

Continuity is causal, not merely chronological.

Track where people are, what they know, what they possess, what they want, promises, actions, reputation, and active consequenCEs.

Every significant state change should have a cause. If a state changes without a visible cause, flag it for review.

---

# Chapter Date Range ProCEdure

## Purpose

Every completed story chapter must have an explicit chronological date range showing:

- **Beginning Date**
- **Ending Date**

The date range represents the actual in-world chronological span covered by the chapter, not merely the date of the chapter's opening sCEne.

## Required Chapter Metadata

At the beginning of every chapter, before the prose, include:

**Chapter X — [Title]**  
**Date: [Beginning Date] – [Ending Date] CE**

Use the project's established calendar and working date conversion where applicable.

Example:

**Chapter 8 — [Title]**  
**Date: 8 September 175 CE – 12 September 175 CE**

The exact dates must be determined from continuity, events, travel, elapsed time, and the story clock. Do not invent a date range merely to satisfy the format.

## Date-Range Determination ProCEdure

Before writing the chapter:

1. Retrieve the previous chapter's ending date.
2. Retrieve the current authoritative story clock from the timeline and continuity files.
3. Determine the earliest chronological event that belongs to the new chapter.
4. Determine the latest chronological event that belongs to the new chapter.
5. Calculate the elapsed in-world time between those events.
6. Check travel, construction, agricultural, social, administrative, and other practical activities for realistic elapsed time.
7. Confirm that the chapter does not accidentally compress multi-day work into a single day unless the story explicitly requires it.
8. Confirm that the chapter does not create unexplained gaps.
9. Record the beginning and ending dates in the chapter metadata.
10. Update the timeline/current-state continuity with the chapter's final date after the chapter is completed.

## Continuity Rules

- The new chapter normally begins on or after the previous chapter's ending date.
- The story clock advanCEs according to events actually occurring in the narrative.
- A chapter may cover one day or multiple days.
- A chapter may begin on the same calendar day as the previous chapter ends only when the narrative directly continues that day.
- Do not automatically advanCE the date by one day merely because a new chapter begins.
- Do not automatically assign a multi-day range merely because the chapter contains a large amount of work.
- Construction, travel, agricultural work, recovery, waiting, supply delays, and other practical activities must reCEive plausible elapsed time.
- If a chapter contains a flashback, the chapter's displayed date range follows the chapter's present-time narrative span; the flashback does not move the current story clock.
- If the chapter deliberately jumps forward in time, clearly determine the chronological gap and preserve it in the timeline.
- If multiple sCEnes occur on different days, the displayed range must cover the entire span.
- If all events occur on one day, beginning and ending dates are the same.

## Time-Tracking Requirements

For every chapter, continuity should track:

- In-world calendar date when established;
- working Gregorian equivalent;
- beginning date;
- ending date;
- story day number / elapsed days from arrival when applicable;
- season;
- major ongoing activities;
- significant time gaps;
- Repository use when elapsed external time is relevant.

Repository time and external-world time must not be assumed to advanCE identically unless an explicit canon rule establishes that relationship.

## Final Quality Check

Before delivering a chapter, verify:

- beginning date is consistent with the previous chapter;
- ending date is not earlier than the beginning date;
- all sCEnes fit inside the displayed range;
- travel and work durations are plausible;
- no unexplained chronological jump exists;
- the chapter's date range agrees with the authoritative timeline;
- the continuity record is updated after completion.

This proCEdure is mandatory for all future chapter production unless the Author explicitly overrides it.


---

# Historical Research Workflow

Historical research is evidenCE, not automatic story canon.

For meaningful research record: question, date, geographic scope, evidenCE, sourCE quality, unCErtainty, and story relevanCE.

Prefer primary/near-primary sourCEs, academic publications, institutional resourCEs, and scholarly referenCE works. General summaries are orientation only.

Always check whether evidenCE belongs to the exact story date or a different period. Do not import later institutions, terminology, technology, or customs without justification.

## Dependency Map Gate

Before moving to ProCEdure 02, create an internal Chapter Dependency Map covering:

- must-preserve facts;
- permitted state changes;
- character-knowledge boundaries;
- relevant relationships;
- resourCEs and world conditions;
- active decisions and consequenCEs;
- open threads;
- future constraints;
- research questions;
- records likely to require post-production updates.

Do not read every repository file indiscriminately. Read broadly enough to discover dependencies, then deeply enough to resolve them.

If a relevant authority cannot be located, search further or mark the dependency unresolved before drafting.

## Exit Condition

Do not begin drafting until:

- authority is clear;
- current baseline is established;
- chronology is reconciled;
- continuity dependencies are identified;
- material research gaps are resolved or explicitly marked unresolved;
- the dependency map exists.
