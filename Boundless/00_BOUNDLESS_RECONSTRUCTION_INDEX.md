# BOUNDLESS — Comprehensive Reconstruction Index

This package is a **forensic reconstruction and working rules audit**, not yet polished publication prose. It combines the current explicit reconstruction decisions with the CLEAN source material. The recovered catalogs are intentionally large: individual Skills, Martial Components, Magic Components/Energies, creature material, and other entries are retained rather than summarized away.

## Reconstruction status legend

- **✅ CONFIRMED** — established by later explicit decisions and treated as current canon unless deliberately reopened.
- **🔄 SUPERSEDED** — recovered source material that has been replaced by a later decision.
- **⚠️ REVIEW / CONVERSION** — concept or content is useful, but one or more mechanics must be reconciled with the current engine.
- **⬜ NEEDS DEVELOPMENT** — incomplete or absent; substantial design work remains.
- **❗ CONTRADICTION** — two surviving sources or decisions conflict and must not be silently reconciled.
- **💡 SUGGESTION** — design suggestion from this reconstruction pass; not canon unless Mike approves it.

**Authority used in this reconstruction:** newest explicit decisions in the current reconstruction work override older text; CLEAN source files are the baseline for material not subsequently changed. Archival Markdown is treated as a searchable transcription of its CLEAN source, not as independent canon. No discrepancy has been silently fixed.

## Source set used

Primary recovered sources:

- `Boundless General Rules CLEAN.docx` / archival Markdown transcription
- `Boundless Combat CLEAN.docx` / archival Markdown transcription
- `Boundless Specialist Basics CLEAN.docx` / archival Markdown transcription
- `Boundless Skills CLEAN.docx` / archival Markdown transcription
- `Boundless Martial CLEAN.docx` / archival Markdown transcription
- `Boundless Magic CLEAN.docx` / archival Markdown transcription
- `Boundless Creatures WIP CLEAN.docx` / archival Markdown transcription
- `Creature layout CLEAN.docx` / archival Markdown transcription
- `Creature traits CLEAN.docx` / archival Markdown transcription
- `Boundless Crafting and Materials CLEAN.docx` / archival Markdown transcription
- `Magic Structure and Energies.xlsx`, represented by its archival Markdown conversion. **Calculator formulas are deliberately ignored as rules authority.**

Older non-CLEAN material was not needed to construct this pass. No older source was allowed to override CLEAN material or later explicit decisions.

## Chapter set

1. **Core Resolution, Tiers, AP, Luck & Universal Mechanics** — current engine and cross-system rules.
2. **Specialists, Character Creation & Advancement** — stats, creation, experience, advancement, possessions, and creation-economy conflicts.
3. **Combat, Defense, Movement, Health & Armor** — opposed combat, defense paths, criticals, movement, Vitality/Fatigue, armor review, Berserk/Meginserk.
4. **Skills** — confirmed Skill thresholds and outcome framework, Hasty/Meticulous, extended checks, Teamwork, combat Skill use, integrated Skill maneuvers, and the complete recovered Skill catalog.
5. **Martial** — current Martial architecture plus the complete recovered Component and Training catalog, each retained for conversion.
6. **Magic** — current spell architecture plus the complete recovered Magic catalog and a formula-free structure/energy index from the workbook.
7. **Creatures & Traits** — current modular Trait framework plus recovered creature types and trait material.
8. **Crafting, Materials, Equipment, Quality & Durability** — recovered crafting/materials, current dependencies, and armor/equipment intersections.
9. **World, Social, Travel & Miscellaneous Rules** — reputation/disposition, travel, carrying, improvisation, sleep, disease/poison, addiction, religion, advanced creatures, ammunition.
10. **Open Questions, Contradictions & Work Queue** — consolidated unresolved decisions and recommended dependency order.
11. **Source Map** — what came from where and how to treat it.

## Current high-level engine snapshot

### ✅ Resolution

- Boundless uses pools of **d10s**.
- Each die showing **6–10 is one success**; **1–5 is a failure**.
- Most contested actions use opposed rolls; higher successes wins.
- A noncombat opposed tie resolves as the minimum successful result unless a specific rule says otherwise.
- In combat, a tie favors the attacker as a **Glancing Blow** and deals **1d10 base damage**.
- When the attacker wins, the **net success margin becomes damage dice**.
- Zero successes is ordinary failure, not automatically a critical failure.
- There are **no automatic successes** from Traits, Training, or high Stats.
- Dice bonuses stack unless a specific mutual-exclusivity rule applies. AP is not a dice-pool cap.

### ✅ Stats and Training

- Universal Stat dice: **(1 + floor(relevant Stat / 10))d10**. The base 1d10 never disappears.
- Universal tier prerequisites: **15 / 30 / 45 / 60 / 75** for Simple / Basic / Intermediate / Advanced / Master.
- Applicable Training contributes **+1d10 per degree**, with no special +2d10-per-degree exceptions.
- In Skills, **degree** is the preferred term for a Specialist's training level; **tier** may describe the task/system category.

### ✅ Action Points

- **Speed is the single source of AP.** Traits, Training, Components, hunger, and other abilities do not directly alter AP flow unless an explicit exceptional rule is later approved.
- Current AP formula: **1 + 2 × floor(Speed / 10)**.
- AP refreshes at the beginning of the Specialist's turn.
- Unused AP does not carry into the next turn.
- AP may be reserved within the current round for appropriate reactions/defense.
- A normal action must be paid for from AP available in the current turn. **AP may not normally be accumulated across turns to enact a single action.**
- An explicit Magic Component may create an exception permitting multi-turn expenditure.
- Paying AP on later turns to **maintain an effect that has already been enacted** is not multi-turn enactment and remains legal in principle.
- Universal single-action AP ceilings are **3 / 6 / 9 / 12 / 15** based on the highest tier Component/Skill involved.

### ✅ Defense framework

Only one defense path applies to a given defense roll:

- **Agility + Unarmored Training**
- **Insight + Evasion Training**
- **Stamina + Armor Training**

The paths are mutually exclusive **per defense roll**. A Specialist can know/use more than one path and can switch approaches as circumstances change, but cannot combine their Stat or Training bonuses on one defense.

- Unarmored Training is unavailable while wearing armor.
- Evasion is unavailable in medium or heavy armor.
- The selected defensive Stat uses the universal Stat-dice formula and the selected Training adds +1d10 per degree.
- Passive Defense costs no AP. Whether Passive Defense can critically succeed or fail has been deliberately reopened for stress testing; do not assume either prohibition or permission until that pass is complete.
- Active Defense costs AP, replaces Passive Defense, and can incorporate eligible Components and other modifiers.

### ✅ / ⚠️ Critical framework

- Every qualifying roll contains one identifiable **Critical Die**: the persistent base +1d10 already included in the normal dice pool. It is not an extra die.
- A **Critical Success** requires the underlying action to succeed and the Critical Die to show a natural **10**.
- A **Critical Failure** requires the underlying action to fail and the Critical Die to show a natural **1**.
- Other natural 10s or 1s do not trigger a critical by themselves, though a specific critical effect may still use the total number of natural 1s or 10s showing to determine severity.
- An attack Critical Success doubles the **damage dice**, not the rolled damage result.
- A provisional defensive Critical Success imposes **-1d10 per excess defensive success** on the attacker's next attack **against that same defender**. This remains pinned for stress testing.
- On an attacker Critical Failure, **-1d10 to the next defensive action per natural 1 showing** is confirmed. The old "no further movement" consequence has been reopened; **half Movement Speed** is the current stress-test candidate.
- A defender Critical Failure grants the attacker **+1 damage per damage die rolled**, retaining the appropriate damage type/provenance. Applying the same half-Movement consequence to the defender is under stress test.
- Passive Defense critical eligibility is separately reopened for stress testing.
- For **Skills**, Overwhelming Success occurs at **150% of the normal threshold, rounded up**; Overwhelming Failure occurs when a failed check misses its threshold by **3 or more successes**. Skill-specific consequences are contextual, while extended checks use the confirmed mark values in Chapter 4.

### ✅ Luck

- Roll **1d10 at the start of the in-game day**; the result is the available Luck Dice/points for that day.
- A spent Luck die that rolls **6–10 adds +1 success**; on **1–5 it adds nothing** and causes no penalty.
- Luck may be committed after the initial roll but before damage/final outcome is determined.
- There is **no special one-die cap on initiative**. A Specialist may spend as much available Luck on initiative as on any other eligible roll.

## Systems that are intentionally not declared finished

The largest remaining design packages are individual Skill conversion and cleanup, Martial Component conversion, the armor/mitigation ecosystem, creation/advancement economy, individual Magic conversion, Crafting/Quality/Durability, and detailed Traits. The chapter files preserve the source material so decisions can be made entry-by-entry without losing anything.
