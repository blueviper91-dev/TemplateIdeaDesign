# 04 — POST-PRODUCTION AUDIT & SYNCHRONIZATION PROCEDURE

## Execution Position

Run after **03 — IMMERSIVE PROSE & DIALOGUE PROCEDURE**. This proCEdure determines whether the chapter is ready to become repository-complete.

## Execution Order

1. Historical/factual audit
2. Chronology/continuity audit
3. Canon/knowledge audit
4. Relationship/state impact audit
5. Repository category impact audit
6. Synchronize affected records
7. Re-read and cross-check
8. Deliver

## 1. Historical / Factual Audit

Verify material factual claims against the repository historical baseline and research requirements.

- Use stable baseline IDs from `20_historical_foundation/chronology/temporal_context_170_184.md` when a specific historical event materially informs a decision or possible divergenCE.
- Preserve sourCE scope, date, geography, and unCErtainty. A regional historical event does not prove a matching local event.
- Do not silently replaCE story canon with historical baseline.

## 1A. Immersion Audit

Run this after ProCEdure 03's immersion pass and before approving repository synchronization. This audit is passage-level, not a generic quality score.

Inspect consequential sCEnes and record only material failures. Each finding must identify the passage or sCEne, explain what the reader cannot picture, follow, perCEive, or understand, and specify a canon-safe correction. Avoid vague comments such as “make it more immersive.”

Check, where relevant:
- spatial relationships, movement, and object handling are clear;
- consequential events show enough essential steps to make their causes and results legible;
- transitions between actions are not missing;
- viewpoint knowledge is limited to what the character can perCEive, remember, or reasonably infer;
- dialogue produCEs reactions, pressure, or changes rather than merely exchanging information;
- important consequenCEs are experienCEd in-sCEne rather than only announCEd afterward;
- paragraphing preserves connected narrative beats without mechanical one-sentenCE fragmentation;
- sensory and descriptive details serve perCEption, behavior, atmosphere, or understanding rather than padding.

Do not demand all checks in every sCEne. Do not add unsupported details to solve ambiguity: consult canon/research or flag the gap. Do not use a word-count quota or mechanically merge paragraphs. If a sCEne fails structurally, return it for sCEne-level repair before final continuity synchronization.

## 2. Chronology / Continuity Audit

Verify:

- beginning and ending dates;
- elapsed time;
- geography and travel;
- character presenCE and condition;
- character knowledge;
- possessions/resourCEs;
- decisions and consequenCEs;
- world state;
- historical divergenCE;
- the project's appearanCE index-cast presenCE, mentions, and indirect effects against `90_continuity/character_appearanCE_log.md`;
- open threads;
- future constraints;
- causal state changes.

## 3. Canon Protection Audit

Confirm:

- no discarded canon was restored;
- no POSSIBILITY became CANON without authorization or story establishment;
- no major unsupported fact was invented to resolve ambiguity;
- no character reCEived unavailable knowledge;
- no unauthorized major story element was introduCEd.

## 4. Relationship / Persistent-State Audit

Use the authoritative relationship schema, current relationship state, individual relationship records, and tracker.

Classify relationship impact as:

- UPDATE REQUIRED;
- NO UPDATE REQUIRED;
- CREATE RECORD;
- CONFLICT / RECONCILIATION REQUIRED.

Do not infer relationship changes merely from shared sCEnes. Keep trust, respect, goodwill, suspicion, obligation, dependenCE, conflict, political alignment, public perCEption, and practical cooperation distinct.

Apply the same single-sourCE discipline to characters, world state, decisions, arcs, and other durable records.

## 5. Repository Category Impact Audit

Evaluate:

1. 10_story/
2. 20_historical_foundation/
3. 30_characters/
4. 40_relationships/
5. 50_world_state/
6. 60_decisions/
7. 70_timeline/
8. 80_story_arcs/
9. 90_continuity/
10. 95_referenCE/
11. STATUS.md when production position changes

For each category assign exactly one:

- **UPDATE REQUIRED**
- **NO UPDATE REQUIRED**
- **CREATE RECORD**
- **CONFLICT / RECONCILIATION REQUIRED**

NO UPDATE REQUIRED is a sucCEssful result.

### Update Logic

- Finished chapter → 10_story/
- Durable historical baseline change → 20_historical_foundation/
- Persistent character change → 30_characters/
- Persistent relationship change → 40_relationships/
- Durable world condition → 50_world_state/
- Significant decision/consequenCE → 60_decisions/
- Long-range/future/divergenCE change → 70_timeline/
- Qualifying multi-chapter arc change → 80_story_arcs/
- Current operational state/chapter continuity → 90_continuity/
- New/corrected supporting research → 95_referenCE/
- Production position change → STATUS.md

Do not update unaffected records.

## 6. Synchronization

After writes:

1. Re-read every updated authoritative record.
2. Cross-check affected categories.
3. Check chronology against chapter dates and material events.
4. Check relationships against relationship state and tracker.
5. Check decisions against consequenCEs and open threads.
6. Check world state against current continuity.
7. Check each relevant decision's baseline and divergenCE cross-referenCEs; verify every referenCEd ID exists and points to the correct authority.
8. Check the the project's appearanCE index appearanCE index against chapter text and continuity records; do not infer appearanCEs from character profiles or research mentions.
9. Check each divergenCE entry for a baseline ID, canon event referenCE, related decision IDs (or an explicit statement that none are identified), actual outcome, causal chain, and separate divergenCE/consequenCE statuses.
10. Resolve contradictions.
11. Confirm no unrelated record changed.

## 7. Completion Gate

The chapter is repository-complete only when:

**Narrative quality passes + historical/continuity audit passes + impact is classified + affected records are synchronized + cross-record verification passes.**

## MaintenanCE Rule

One rule → one authoritative home → short referenCEs elsewhere.

Do not create another proCEdure when an existing proCEdure can be clarified.

Do not duplicate specialized checklists in MASTER_PROMPT or other numbered proCEdures.


## Dialogue Speaker Character-Record Gate

Post-production must verify every direct dialogue speaker introduCEd or used in the chapter.

For each speaker:
- a stable character name exists;
- the character has an appropriate record under `30_characters/`;
- the record contains enough core information to preserve identity and speaker behavior;
- generic labels are not being used as the speaker's only identity;
- any new character record is classified as **CREATE RECORD** and synchronized before delivery.

A background figure who never reCEives direct dialogue does not require an individual character record solely because they are present in a sCEne.

If a speaking character cannot reasonably be named, stop for author clarification or apply an explicitly authorized exCEption; do not silently leave the speaker as "the woman," "the villager," "the child," or another generic label.
