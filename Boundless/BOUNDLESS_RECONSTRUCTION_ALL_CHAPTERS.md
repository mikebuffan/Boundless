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


---

# Chapter 1 — Core Resolution, Tiers, AP, Luck & Universal Mechanics

## Reconstruction status legend

- **✅ CONFIRMED** — established by later explicit decisions and treated as current canon unless deliberately reopened.
- **🔄 SUPERSEDED** — recovered source material that has been replaced by a later decision.
- **⚠️ REVIEW / CONVERSION** — concept or content is useful, but one or more mechanics must be reconciled with the current engine.
- **⬜ NEEDS DEVELOPMENT** — incomplete or absent; substantial design work remains.
- **❗ CONTRADICTION** — two surviving sources or decisions conflict and must not be silently reconciled.
- **💡 SUGGESTION** — design suggestion from this reconstruction pass; not canon unless Mike approves it.

**Authority used in this reconstruction:** newest explicit decisions in the current reconstruction work override older text; CLEAN source files are the baseline for material not subsequently changed. Archival Markdown is treated as a searchable transcription of its CLEAN source, not as independent canon. No discrepancy has been silently fixed.

## 1. Universal dice engine

**✅ CONFIRMED**

Boundless resolves actions with pools of d10s. Each die showing 6–10 contributes one success. Each die showing 1–5 contributes no success. Opposed actions compare success counts. Threshold actions compare the number of successes against the required threshold.

The universal Stat contribution is:

**Stat Dice = (1 + floor(relevant Stat / 10))d10**

This preserves the minimum +1d10 at every Stat value. Examples: Stat 1–9 = 1d10; 10–19 = 2d10; 30–39 = 4d10; 75 = 8d10; 100 = 11d10.

Applicable Training contributes **+1d10 per degree**. Other applicable dice sources may stack unless a rule explicitly makes them mutually exclusive.

There are no automatic successes. Critical Success, Critical Failure, and subsystem-specific Overwhelming outcomes are special roll states rather than automatic successes.

## 2. Opposed and threshold checks

**✅ Opposed checks:** higher successes wins. Combat ties become Glancing Blows in the attacker's favor. Noncombat ties default to the minimum successful outcome unless the relevant subsystem specifies otherwise.

**✅ Threshold checks:** meeting or exceeding the threshold succeeds. For Skills, the confirmed difficulty ladder is **2 / 3 / 4 / 5 / 6 successes** for Simple / Basic / Intermediate / Advanced / Master. Other subsystems may define their own threshold structures where explicitly required.

## 3. Universal tiers and prerequisites

**✅ CONFIRMED**

| Tier | Minimum relevant Stat | Universal single-action AP ceiling |
| --- | ---: | ---: |
| Simple | 15 | 3 |
| Basic | 30 | 6 |
| Intermediate | 45 | 9 |
| Advanced | 60 | 12 |
| Master | 75 | 15 |

The highest-tier Component/Skill used in an action determines that action's AP ceiling. The ceiling limits AP expenditure, not the total number of dice that may be rolled.

## 4. Action Points

**✅ CONFIRMED architecture**

Speed is the only normal source of AP.

**AP = 1 + 2 × floor(Speed / 10)**

| Speed | AP |
| ---: | ---: |
| 0–9 | 1 |
| 10–19 | 3 |
| 20–29 | 5 |
| 30–39 | 7 |
| 40–49 | 9 |
| 50–59 | 11 |
| 60–69 | 13 |
| 70–79 | 15 |
| 80–89 | 17 |
| 90–99 | 19 |
| 100 | 21 |

AP refreshes at the beginning of a Specialist's turn. Unused AP does not carry to the next turn. AP may be held during the current round for eligible defensive/reaction actions.

A normal action must be fully paid for using AP available in the current turn. AP is not normally banked or accumulated across turns to enact one action. A specific rule or Component can create an explicit exception. Maintenance AP for an effect that has already been successfully enacted is conceptually separate and remains allowed in principle.

**💡 Balance observation:** because the AP progression is odd-numbered after the base 1, full use of the 3/6/9/12/15 ceilings first becomes possible at Speed 10 / 30 / 40 / 60 / 70 respectively. This is not labeled a defect; it should simply be kept visible during testing.

## 5. Initiative and structured time

**✅ CONFIRMED:** Initiative is rolled once at the beginning of combat and the order remains static for the combat unless a later rule explicitly changes it.

**✅ Current dice:** Initiative uses Speed through the universal Stat formula, so Initiative Dice = (1 + floor(Speed/10))d10.

**⚠️ REVIEW:** tie-breaking, surprise, delayed actions, simultaneous actions, and the exact reaction timing window still require a consolidated timing rule.

## 6. Luck

**✅ CONFIRMED modern Luck**

At the start of each in-game day, roll 1d10. The result determines the Luck available for that day. Each Luck die spent on a roll is rolled separately: 6–10 adds one success; 1–5 adds nothing. A failed Luck die never removes a success.

Luck is committed after the initial roll but before damage or the final outcome is determined. Luck is not specially limited on Initiative.

### Recovered CLEAN Luck rules

**🔄 SUPERSEDED where they conflict with the modern rule above.** The following is preserved to show the older design and any useful edge cases:

# Luck

At the beginning of each day, Specialists determine the base amount for their luck pool. This is done by rolling 1d10 for each luck pool rank, and adding the results together. The total represents the Specialist’s total luck pool for the day. Unlike other pools, luck doesn’t regenerate, and can never be refilled. Once it’s used up, it’s gone until the next day.

Luck points can be used to alter the outcomes of rolls, and influence events. This influence won’t always be in the direction a Specialist would like, however. As true luck isn’t always good or always bad, neither is the luck in Boundless. Using the luck pool can give a Specialist that little nudge needed to topple an overwhelming foe, or it can reinforce the magnitude of the failure against the same foe.

## Luck and Attack Rolls

When used to determine a hit or a miss, attacker and defender can boost their rolls with luck. An attacker or defender using luck chooses an amount of luck to use, rolls to hit or to defend, flips the luck coin, then adds to or subtracts from the roll as appropriate. On an unlucky roll, the amount of luck can reduce the roll to 0, which counts as a critical fumble. Conversely, a lucky roll can turn a natural fumble into a successful roll. On a lucky roll, even if the luck chosen is higher than the roll, the total can’t exceed twice the roll amount. For example, if a player uses 50 luck, but only rolls a 30, the total result would be 60 (30 roll, plus 30 of the 50 luck), but the Specialist still loses the whole 50 points from their luck pool.

## Luck and Damage

When used to on a damage roll, the player chooses an amount of luck to use, flips the luck coin, and rolls for damage.

On a lucky flip, the Specialist adds all luck used to the damage rolled, if the damage rolled is more than the luck used. If the luck used is more than the damage rolled, it simply doubles the damage. Luck used beyond doubling the damage is simply lost. For example, a Specialist that uses 30 luck would add all 30 points if they rolled 35 damage. If the same Specialist only rolled a 23, they would simply double the total damage to 46. The remaining 7 luck are lost.

On an unlucky roll, the damage is reduced by an amount equal to the luck used, potentially to zero. On an unlucky critical fumble, the Specialist takes damage as though they were the target of the attack, and the roll was lucky. For example, if the Specialist used 15 luck points to boost the attack, and the roll is an unlucky critical fumble, the Specialist rolls damage as normal. If the damage rolled is over 15, the Specialist takes 30 points of damage. If the damage rolled is less than 15, such as a roll of 12, the Specialist takes double the damage roll. In this case, 24.

## Luck and Skills

When used to on a skill roll, the player chooses an amount of luck, flips the luck coin, and rolls as normal. On a lucky flip, the luck, up to an amount equal to the natural roll, is added to the skill roll. On an unlucky flip, the skill roll is reduced by an amount equal to the luck used, potentially to zero. In the case of an unlucky critical failure, any skill with negative consequences for failure has double the negative consequences. For example, if a Specialist is working with gun powder, the gun powder would not only explode, but it would deal double damage to the Specialist and nearby equipment. Any tools being used in an unlucky critical failure have a chance of breaking equal to the amount of luck used.

## 7. Critical Success, Critical Failure, and Overwhelming outcomes

**✅ Universal Critical Die:** every qualifying roll contains one identifiable **Critical Die**: the persistent base +1d10 already included in the normal dice pool. The Critical Die is not an additional die.

- **Critical Success (Crit+):** the underlying action succeeds and the Critical Die shows a natural **10**.
- **Critical Failure (Crit-):** the underlying action fails and the Critical Die shows a natural **1**.
- A natural 10 on the Critical Die does not create Crit+ if the action fails.
- A natural 1 on the Critical Die does not create Crit- if the action succeeds.
- Other natural 10s or 1s do not trigger a critical by themselves, though a specific critical effect may use the total number showing to determine severity.

At a physical table, the Critical Die should be visually distinguishable. In digital resolution, the engine identifies it internally.

**✅ Attack Critical Success:** double the damage dice.

**⚠️ Provisional defensive Critical Success:** when a defender wins and qualifies for Crit+, the attacker takes -1d10 per excess defensive success on their next attack against that same defender. Whether Passive Defense can critically succeed or fail has been reopened for stress testing.

**✅ / ⚠️ Attacker Critical Failure:** the confirmed penalty is -1d10 to the attacker's next defensive action **per natural 1 showing anywhere in the failed attack pool**. The previous "no further movement" consequence has been reopened; **half Movement Speed** is the current stress-test candidate.

**✅ Defender Critical Failure concept:** attacker gains +1 damage per damage die rolled, preserving the appropriate damage type. Applying the same half-Movement consequence to the defender is under stress test.

### Skill Overwhelming outcomes

**✅ Overwhelming Success (OwS):** on a Skill check, OwS occurs when the roll reaches **150% of the normal success threshold, rounded up**. With Skill thresholds 2 / 3 / 4 / 5 / 6, the OwS thresholds are 3 / 5 / 6 / 8 / 9.

**✅ Overwhelming Failure (OwF):** on a failed Skill check, OwF occurs when the roll falls short of the normal threshold by **3 or more successes**. Simple Skill checks cannot produce OwF under this rule.

OwS may coexist with Crit+; OwF may coexist with Crit-. Their Skill-specific consequences are contextual, while Chapter 4 defines their confirmed effects on extended checks.

### Recovered CLEAN critical rules

**🔄 SUPERSEDED in trigger and most effects; retained as design history.**

# Critical Success and Failure

When rolling the dice, doubles count as a critical hit while rolling 01 counts as a fumble. For example, 00, 11, 22, 33, 44, 55, 66, 77, 88 and 99 are all critical success. This gives the Specialist a 10% chance for critical hits and a 1% chance to fumble.

### Rolling 00

Rolling 00 on the dice is bittersweet. Since it’s a double, it counts as a critical success, which means the Specialist gets another roll. However, since the value on the dice gets added to the current roll, it doesn’t increase the amount already rolled at all. Essentially, rolling 00 is just reroll.

### Critical success

Critical success on any roll grants a Specialist an additional roll for that action. Furthermore, critical successes increase the cap by the amount rolled, and thus, don’t count against the roll’s cap. For example, if a Specialist makes an attack with a cap of 100 and rolls a 55, the Specialist may roll again with the damage cap increased to 155.

### Critical failure

The effects of any critical failure are twofold. First, anything already rolled for is immediately halved (though other bonuses, such as training or primary stat remain unaltered). For example, if a player has rolled 350 damage already and critically fails, the damage from rolls is reduced to 175. The second effect of a critical failure is that any remaining rolls are forfeit. Regardless of the total from previous rolls, the roll of 1 from a critical failure is not added to the total.

## 8. Improvisation

**⚠️ REVIEW, concept strongly compatible with the modern engine.** CLEAN supports substituting items and improvising Magic/Martial/Skill solutions. Exact modifiers must be converted where they rely on old math.

# Improvisation

Improvisation in Boundless is surmounting a challenge in an unexpected way. This could range from using improvised weapons in a fight, to using magic in place of a skill, to using a skill instead of combat.

## Item Improvisation

Item improvisation is when a Specialist uses an item in place of another item to do the same job. For example, using a hairpin to pick a lock, instead of a lock pick, or standing on a stool to reach an item on a high shelf, instead of a ladder.

## Magic, Martial and Skill Improvisation

Magic, martial and skill improvisation are slightly different than item improvisation. For example, a caster could use magic or brute force to pick a lock, or they may use an attack to harvest wheat. Creative players will improvise to overcome challenges when they don’t have the proper tools available for the job.

## 9. Universal damage provenance

**✅ CONFIRMED:** when an action contains multiple damage sources, the dice retain their source/type through resolution. Natural weapons and manufactured weapons are alternative weapon profiles; dice from distinct profiles are not casually merged unless an explicit Component constructs a combined/hybrid attack.

## 10. Universal condition philosophy

**✅ CONFIRMED architecture:** Conditions should operate consistently across Martial, Magic, Traits, Crafting, and environmental effects rather than creating bespoke status subsystems for every source.

**⬜ NEEDS DEVELOPMENT:** a canonical Conditions glossary does not yet exist.


---

# Chapter 2 — Specialists, Character Creation & Advancement

## Reconstruction status legend

- **✅ CONFIRMED** — established by later explicit decisions and treated as current canon unless deliberately reopened.
- **🔄 SUPERSEDED** — recovered source material that has been replaced by a later decision.
- **⚠️ REVIEW / CONVERSION** — concept or content is useful, but one or more mechanics must be reconciled with the current engine.
- **⬜ NEEDS DEVELOPMENT** — incomplete or absent; substantial design work remains.
- **❗ CONTRADICTION** — two surviving sources or decisions conflict and must not be silently reconciled.
- **💡 SUGGESTION** — design suggestion from this reconstruction pass; not canon unless Mike approves it.

**Authority used in this reconstruction:** newest explicit decisions in the current reconstruction work override older text; CLEAN source files are the baseline for material not subsequently changed. Archival Markdown is treated as a searchable transcription of its CLEAN source, not as independent canon. No discrepancy has been silently fixed.

## 1. Specialist identity and classlessness

**✅ CONFIRMED in principle:** Boundless is classless. A Specialist may use a descriptive class/title, but purchased Stats, Training, Components, Skills, and Traits define what the character can actually do.

## 2. SPECIALIST Stats

The CLEAN Specialist Basics chapter defines ten Stats: **Speed, Proficiency, Endurance, Charisma, Intelligence, Agility, Looks, Insight, Stamina, Toughness.** Later work continues to use this Stat set.

**✅ Universal derived-dice rule:** when a Stat supplies dice, use (1 + floor(Stat/10))d10 unless a specific current rule says otherwise.

**✅ Key surviving derived relationships:**

- Speed → AP and Initiative.
- Endurance → Vitality, currently 1:1.
- Stamina → Fatigue, currently 1:1.
- Toughness → carrying/physical lifting framework, exact multipliers under review.
- Agility / Insight / Stamina → the three mutually exclusive defense routes through Unarmored / Evasion / Armor Training.

### Recovered Stat descriptions

The CLEAN wording is preserved below because much of the descriptive language is still useful even where individual derivative formulas have changed.

## Specialist Scores

There are ten Specialist scores that are used to determine the various capabilities of a Specialist: Speed, Proficiency, Endurance, Charisma, Intelligence, Agility, Looks, Insight, Stamina and Toughness.

### Speed

Speed is both a measure of how fast your character can react during combat and movement speed. Use the following chart to figure out what your Speed Rating is, based on your Speed. The formula is Speed score divided by 10, and rounded up. The Specialist’s Speed Rating determines the number of movement units a Specialist may move for each move action they take as well as the number of Action Points, or AP they gain each round in combat.

| Speed score | 1-10 | 11-20 | 21-30 | 31-40 | 41-50 | 51-60 | 61-70 | 71-80 | 81-90 | 91-100 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Speed Rating | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 |

### Proficiency

Proficiency is a measure of your Specialist’s hand-eye coordination. Ranged martial components require a minimum Proficiency score of 15 for simple, 30 for basic, 45 for intermediate, 60 for advanced, and 75 for master. Specialists who intend to focus on thrown or projectile weapons favor their Proficiency stat.

### Endurance

Endurance is a measure of your resilience and is the governing stat for your Vitality. A Specialist’s maximum vitality is equal to their Endurance score. Endurance does not govern any skills.

### Charisma

Charisma is your force of personality. Charisma is used to persuade an audience or lead an army. Some magic energy components require a minimum Charisma score of 15 for simple, 30 for basic, 45 for intermediate, 60 for advanced, and 75 for master. Casters who wish to bend the will of others favor their Charisma stat.

### Intelligence

Intelligence is a measure of your logic, reasoning and the ability to process information. Some magic energy components require a minimum Intelligence score of 15 for simple, 30 for basic, 45 for intermediate, 60 for advanced, and 75 for master. Casters who wish to deal a lot of damage in combat or overcome logic based situations with spells favor their Intelligence stat.

### Agility

Agility determines how nimble and flexible you are. Some defensive martial components and advanced martial trainings require a minimum Agility score of 15 for simple, 30 for basic, 45 for intermediate, 60 for advanced, and 75 for master. Specialists who wish to dodge nimbly or excel at fighting with no armor favor their Agility stat.

### Looks

Looks are your overall appearance and can help a Specialist either stand out or blend in to a crowd.

### Insight

Insight is a measure of your overall understanding and empathy. Some magic energy components require a minimum Insight score of 15 for simple, 30 for basic, 45 for intermediate, 60 for advanced, and 75 for master. Casters who wish to deal in the body, life and death, or flashy effects favor their Insight stat.

### Stamina

Stamina is a measure of your pain tolerance and is used to determine a Specialist’s maximum Fatigue. Specialists who wish to wear armor require a minimum Stamina score of 15 for simple, 30 for basic, 45 for intermediate, 60 for advanced, and 75 for master.

### Toughness

Toughness is a measure of your physical strength, which determines your carrying limits. Melee weapon and shield martial components require a minimum Toughness score of 15 for simple, 30 for basic, 45 for intermediate, 60 for advanced, and 75 for master. Melee damage or tank focused martial Specialists favor their Toughness stat.

## 3. Character creation economy

**❗ CONTRADICTION / DECISION REQUIRED**

The CLEAN rules use **100 starting Stat points**, a maximum of 20 in a starting Stat before racial modification, and then immediately grant the first Advancement / 10 Advancement Points after Stats are distributed.

Later Trait reconstruction work contains a competing architecture: **a 100-point creation pool shared by starting Stats and Traits**, with negative Traits returning creation points. That later architecture has not yet been fully reconciled with the CLEAN starting 100 Stat points + starting Advancement model.

No merged rule is declared here.

### CLEAN starting rules

## Starting Stats

Each Specialist starts with 100 stat points to spend. On character creation, a Specialist may have up to 20 points in any given stat. Racial traits may increase or decrease the maximum possible starting stat points. No stat may have less than 1 point.

Starting stats are considered to be 0 advancements. Since 0 * 100 = 0, starting Specialists automatically gain one advancement immediately after they’ve distributed their stats.

## Starting Advancement Points

A Specialist starts with a no advancement, unless otherwise specified by the Keeper, but immediately gains an advancement once they’ve distributed their SPECIALIST stat points. This gives a starting Specialist 10 advancement points to use for buying racial traits, additional stat points, magic and/or martial components and skills. It should be noted that some racial traits may only be purchased at character creation.

## 4. Tier prerequisites and primary Stats

**✅ CONFIRMED universal prerequisites:** 15 / 30 / 45 / 60 / 75.

**✅ Later primary-Magic choices:** Charisma, Intelligence, or Insight.

**✅ Later primary-Martial choices:** Proficiency, Agility, or Toughness.

**⚠️ REVIEW:** CLEAN often assigns ranged/melee/defensive Martial prerequisites directly to Proficiency/Toughness/Stamina. Later work broadened Martial identity and separated defense paths. Individual legacy prerequisites must be audited entry-by-entry rather than silently retained.

## 5. Attacks and hybrid actions

**✅ CONFIRMED:** Martial, Magic, and Skills can coexist in hybrid actions. The primary delivery method determines whether the action hits; separate parts retain their identity and damage provenance.

### Recovered CLEAN attack text

## Attacks

The attacks section is intended to give players a place to keep their favorite attacks written down, with all calculations already recorded to help speed combat along. The idea is to build a few attacks from your components to have them ready to go at a moment’s notice.

An attack is any action intended to cause harm, although not necessarily injury, to another, whether it be via martial attacks, casting a spell, or the use of skills. In game terms, this means that any action intended to damage or hinder an opponent is considered an attack.

### Basic Attacks

A basic attack is an attack that is strictly martial, strictly magic, or strictly skill. Attacks of this sort explained in the section of the respective type of attack.

### Hybrid Attacks

Hybrid attacks are those that combine martial, magic and/or skill into a single attack. For example, a sword charged with a spell counts as a hybrid attack. In such cases, the primary delivery method is used to determine whether the attack hits or misses. Damage is determined separately for each part of the attack. Special defenses may apply to magic portions of attacks, such as an opponent who attempts to ward the spell’s effect. The Keeper determines which part of a hybrid attack is the primary delivery vehicle.

## 6. Creature identity during character creation

**🔄 CLEAN race-package restrictions are partly superseded by the modular Trait architecture.** Creature Types are now treated as classifications/collections of Traits. The Creature Type itself has no separate point cost; the Traits that qualify the Specialist for that classification do have their normal costs.

A Specialist must possess a substantial portion of the Traits associated with a Creature Type to reasonably claim that Type. The exact threshold for "substantial portion" is not yet formalized.

### Recovered CLEAN racial-feature framework

## Racial Features

For gaming purposes, human is considered the standard race. For Specialists who are not human, the notes area in the Skills section of the Specialist Record is a good place to keep track of what makes them different.

### Standard Racial Features

Standard racial features are features that every creature has, simply by existing. These are race, size category, movement types (primary and alternative).

### Selective Racial Features

Some races have various features which set them apart from other races in different ways. Some may have wings, while others may have gills and fins. As such, many races have various racial features available to choose from during character creation. Some racial features cost advancement points, and provide a positive effect, while others essentially give an advancement point bonus and impose a negative effect. In general, the bonus advancement points from selecting negative features shouldn’t outweigh the advancement point cost of positive effects, though the Keeper may allow it on a case-by-case basis.

Selective racial features may only be purchased during character creation, though they may be improved later through regular advancement point expenditures. For example; a Specialist with Harpy blood may start the game with very basic, essentially useless wings, which could later be improved to provide gliding and even flight. If the same Specialist doesn’t take the wings at character creation, however, they shouldn’t be able to spontaneously grow wings later in life.

Selective racial features give players the ability to customize their Specialist’s race to fit their play style. In general, it should be assumed that any Specialist that only has a few of the available racial traits is a cross-breed. Only Specialists who have all the racial traits of a race are considered pure-blooded.

### Choosing a creature type

An important aspect of your Specialist is your creature type. In the process of creating your Specialist, you’ll want to decide what creature type your Specialist will be, and purchase racial features with your starting advancement points. Once you’ve chosen your creature type, you can’t purchase racial features that don’t belong to that creature type. If you can’t afford a racial feature with your starting advancement points, you may purchase them once you’ve earned more advancements, unless otherwise specified in the racial feature. For example, if your creature type is pixie, you may have vestigial wings on Specialist creation (namely because you couldn’t afford to purchase the Flight racial feature). Once you’ve earned more advancement points, you could purchase the Flight racial feature to make use of your wings. You can’t, however, start as a human, and suddenly decide you’re a centaur, and spontaneously have your legs turn to horse legs, and grow two more of them.

### Constructing your own creature type

We strongly caution you to obtain Keeper approval before you go about creating your own creature type. Once you have approval, we advise you to work closely with your Keeper to create your new creature type. This could be as simple as combining two creature types, and having the available racial features of both, or it could be as complex as grabbing numerous racial features and creating an entirely new creature type. If you’re just combining two creature types in equal proportions, your result will be known as a “half-breed”. If you’re combining racial features of two or more types, your result will be a “mixed-breed”. With a mixed-breed, find the highest concentration of racial features. The overall category those features belong to determine your primary creature type. For example, if you combine traits from monstrous, undead, and demonic creature types, but most of the traits you’ve chosen are from the undead types, your Specialist is considered undead.

## 7. Experience and Advancement

**⚠️ REVIEW / CONVERSION**

The CLEAN progression engine is coherent enough to preserve, but it must be reconciled with the newer creation economy and newer 3/6/9/12/15 Trait cost ladder.

Recovered CLEAN rules include:

- Experience earned from encounters/challenges.
- Advancement when the required experience is reached; excess experience rolls over.
- Each Advancement grants 10 Advancement Points.
- CLEAN Magic/Martial/Skill costs are 1/2/3/4/5 by tier.
- Stats cost 1 point per Stat point.
- Skill degrees are sequential and normally limited to one degree of the same Skill per Advancement.
- Unspent experience is lost on death.

**❗ DECISION REQUIRED:** determine whether 1/2/3/4/5 purchase costs remain for Skills/Martial/Magic, whether the 3/6/9/12/15 Trait cost structure stays Trait-specific, and how all of this interacts with the creation pool.

### Recovered CLEAN Advancement text

# Experience Points and Advancements

Although Boundless doesn’t have predefined classes or levels, Specialists still have the ability to grow and advance. To that end, Specialists earn and use Experience Points (Exp.) to advance.

## Earning Experience Points

Specialists earn Exp. by adventuring and surviving encounters. Encounters can be combat, puzzle, trap, or even role play. Generally, an encounter is any situation in which a Specialist must use attacks, magic or skills.

## Advancements

Each time a Specialist gains an amount of Exp. equal to their current advancement, they gain another advancement. For example, a Specialist with 5 advancements gains another advancement when they’ve gained 500 additional Exp. Any Exp. beyond the amount needed for the next advancement roll over. Thus, with the previous example, if the Specialist gains enough Exp. to give them 531 Exp., they would become advancement 6, and have 31 Exp. (531 – 500 = 31) toward their next advancement.

When a Specialist earns an advancement, they gain 10 advancement points to spent on racial traits, stats, magic components, martial components, and skills. Racial trait costs are listed for each trait. Stats are purchased on a point for point basis, meaning each advancement point is good to increase a stat by 1 point. Magic and martial components cost are based on their tiers; 1 point for simple, 2 for basic, 3 for intermediate, 4 for advanced, and 5 for master. Skill ranks may be purchased at the same tier-based cost as magic and martial components, but only one tier of a given skill may be purchased in the same advancement, and the previous tier must already be purchased to learn the next. For example, a Specialist that has already learned simple Riding could purchase basic riding, but could not skip basic to purchase intermediate, nor could the Specialist purchase basic and intermediate Riding in the same advancement. A Specialist may advance different skills in the same advancement, such as Riding and Blacksmithing, regardless of the current tier of the skills, so long as the Specialist has enough remaining advancement points to purchase the prospective skill tiers.


## Death and Experience

As with most games, death carries a penalty. Although a corpse may be revitalized, the process of dying and being brought back to life takes a toll on the spirit. To reflect this, in Boundless, any unspent Exp. are lost whenever a Specialist dies.

## 8. Bank and possessions

**✅ Concept retained; ⚠️ economic details require world/equipment pass.**

Later work indicates Location means the on-person/storage location of an item and that the intended currency presentation is silver-based rather than relying on old Qwartz wording. Exact economy tables are not present in this CLEAN chapter.

# Bank and Possessions

The bank and possessions section of the Specialist Record is provided for Specialists to keep track of their wealth and possessions. This can be equipped, carried, or simply owned items, or even property.

### Equipment

Equipment consists of items a Specialist is able to carry around with them, and have ready to use at a moment’s notice. Generally, it refers to armor being worn, and weapons and/or shields held or readily available.

### Items

Items consist of objects a Specialist carries, but generally not those used in combat. These range from clothing, to jewelry, to food, to skill and trade kits.

### Property

Property is anything a Specialist owns, but isn’t currently carrying with them. This can be land, vehicles, animals, furniture, buildings, etc. Often, owned property requires staff to upkeep.

### Wealth

Wealth generally refers to the amount of Qwartz a Specialist carries, but can also encompass any other form of currency used to purchase or exchange for goods or services.

## 9. Complete CLEAN Specialist Basics source

The entire source is preserved below for line-by-line editing. Where it conflicts with the current reconstruction notes above, the notes above take precedence.

---

# Specialist Basics

# Aspects of a Specialist

A Specialist is any creature in the world that could potentially be a player character; specifically, in this case, your character. A Specialist is represented by certain numerical statistics. These statistics govern how well a Specialist can do any given task as well as how resilient they can be. Experience points (exp) determine the growth of a Specialist.

## Specialist Record (Spec Rec)

A Specialist Record (Spec Rec) is divided into 4 basic areas. Specialist Magic, Martial and Skills. We’ll examine each below.

### Specialist

At the top of the Specialist sheet is the basic information about your Specialist. The player (you), the Keeper and the campaign name are provided to help prevent players’ characters from getting mixed up.

Next up is the Specialist’s name, race, class, experience points and advancements. Name is self-explanatory. Race can be a race chosen from the creatures section, or can be made up with your Keeper’s approval. Class is a bit subjective. Unlike other game systems, your class doesn’t define your character. Instead, your character defines your class. For example, if you intend to play a stealthy, hard-hitting melee assassin, you could call yourself a ninja. Or if you plan to be a magical powerhouse, lobbing spells all about, you could call yourself a wizard or sorcerer. Having a name for your class is completely optional, but may help others to understand your role within your adventuring party better.

Experience points, or exp, are a way to track the amount of encounters or challenges your Specialist has overcome. Advancements are a way to track the number of times your Specialist has advanced. Each advancement gives a Specialist 10 Advancement Points to distribute into training or SPECIALIST scores An easy way to track your progress toward your next advancement is to “reset” your exp each time you advance. That is, when you gain enough exp to advance, erase your current exp and simply write any remaing exp after your advancement in the exp spot. Using this method, any time your current exp reaches or exceeds your advancements, you gain another advancement. For example, if you have 3 advancements and 280 exp, and you gain 31 exp, you would gain an advancement, since your current exp total would now be 311. Now, you would change your advancements to 4 and write the 11 remaining exp (311 – 300 = 11) in your exp slot.

The next section of the Specialist sheet is your SPECIALIST scores; Speed, Proficiency, Endurance, Charisma, Intelligence, Agility, Looks, Insight, Stamina and Toughness. The far-left column indicates your primary stats for Magic and Martial abilities. The second column simply lists the SPECIALIST stat names. The third column is for tracking each stat’s score. The fourth column is for various derivative scores, such as action points, vitality score, carry weight, and so on. Formulae for determining each derivative stat are provided.  This is also a good place to make note of temporary stat changes.

Following the SPECIALIST stat block is the favorite attacks area. This area is a good place to keep track of spells or attacks you use frequently. The far-left column is the name of the attack. This can be whatever you want to call the attack, but it’s generally a good idea to name it something meaningful. While you could name a spell “Ultra Death”, doing so would be silly if it was an instantaneous, touch Charm 1 (sleep) spell. The middle column is a place to list the components used in the attack. In the previous case, these are duration: instantaneous, shape: touch, energy: Charm 1 (sleep), optional: none. The far-right column is provided to indicate the minimum AP cost of the attack. In the previous example, the cost would be 1 AP, since all 3 components used in the spell are simple.

The next section is Luck. This is where a Specialist keeps track of the luck points they roll at the beginning of each day. Luck was intentionally placed between attack and defense to remind players that their Specialist may use their luck points on attack, damage, defense and mitigation. Luck points may also be used on skills, though skills have their own page within the Spec Rec.

Defense and damage mitigation make up the next section of the Specialist sheet. For armor and shield, an area is given to track the defense bonus provided by each, as well as the damage mitigation provided by each. Sections are also provided for defense bonus for evasion and warding.

Following the defense and mitigation section is the possessions section, which is broken up into two areas. Bank is provided for keeping track of a Specialist’s available money, while the possessions section is provided for keeping track of worldly goods, such as clothes, weapons, armor, vehicles, etc.

Each line of the possessions section provides a name and notes column to keep track of info about an item, such as hemp rope – 30-feet. The Location column is provided to track where the Specialist keeps the item, such as in a backpack, slung across their shoulder, or on a cart. This can be important, for example, if a Specialist must leave their cart behind to enter a cave, or if their backpack is stolen. The next column is quantity, to help track how many of a given type of item a Specialist has, such as 1 sword, 5 marbles, 2 belt pouches, etc. The second-to-last column is for weight. In general, it’s best to track weight by multiplying the individual weight of an item by the quantity of the items owned and placing the result in this box. For example, if you own 5 bricks each weighing 2kg, you would list weight as 10kg. For items which are likely to be used or lost, it may be a good idea to add the individual weight in the notes section for the item, so it can be quickly adjusted. The final column is price. Prices of items in Boundless are variable, but this is a good place to keep track of how much you paid for something, or how much you intend to sell it for. It’s worth noting that a Keeper may roleplay transactions, so be prepared to haggle.

### Magic

The magic section of the Spec Rec is relatively straight-forward. Across the top are the various tiers, simple, basic, intermediate, advanced and master. Below those are listed the energy, structure and optional components that belong to that tier. Next to each component is a checkbox to indicate whether a Specialist has learned that component or not. On advancement, magic components may be purchased at a cost of 1 advancement point each for simple, 2 each for basic, 3 for intermediate, 4 for advanced, and 5 for master. Specialists must meet the prerequisite primary casting stat for each tier in order to learn a component. Additionally, tiered energies require the previous tier to be purchased before they themselves can be purchased. Tiered energies are denoted with an asterisk.

### Martial

Much like the magic section, the martial section is topped with the simple, basic, intermediate, advanced and master tiers for the components listed below them. Beneath those are the ranged, melee and defensive categories which fall into each tier. Individual components are listed, each with their own checkboxes to indicate whether a component has been learned. It is worth noting that shot and throw components are detailed together, but the throw versions of the components are learned separately from the shot versions.

Below the components is the advanced martial training area. This is where you would list any advanced training your Specialist has. At the right of each line are the S, B, I, A and M, so you can circle the tier of training your Specialist has achieved.

### Skills

The skills section differs from the magic and martial sections. As each skill has training tiers, they’re divided into their respective SPECIALIST stats, then listed alphabetically. Instead of a checkbox, each skill has S, B, I, A and M so you can circle the degree of training your Specialist has achieved in each skill.

Below the skills section is a notes section. This is provided for you to keep track of any extra notes you feel are important, such as campaign plot information, Specialist history or personality traits and so on.

# Character Creation

There is no right or wrong way to go about building your Specialist. Some people prefer to envision a character concept and attempt to build their character to match their idea of the concept, such as choosing stealthy abilities to make a ninja, or casting abilities to make a wizard. Others prefer to come up with a personality for their Specialist, and decide what sorts of abilities would support that personality, such as a greedy Specialist may enjoy pickpocketing, and be like a rogue. Others still prefer to write a back story for their Specialist, and in the process, explain the sorts of training the Specialist may have had access to, and how they’ve become what they are today. All of these are viable methods of building a Specialist. In general, we recommend that each Specialist have a concept, a back story, and at least a few personal goals.

## Starting Stats

Each Specialist starts with 100 stat points to spend. On character creation, a Specialist may have up to 20 points in any given stat. Racial traits may increase or decrease the maximum possible starting stat points. No stat may have less than 1 point.

Starting stats are considered to be 0 advancements. Since 0 * 100 = 0, starting Specialists automatically gain one advancement immediately after they’ve distributed their stats.

## Starting Advancement Points

A Specialist starts with a no advancement, unless otherwise specified by the Keeper, but immediately gains an advancement once they’ve distributed their SPECIALIST stat points. This gives a starting Specialist 10 advancement points to use for buying racial traits, additional stat points, magic and/or martial components and skills. It should be noted that some racial traits may only be purchased at character creation.

## Specialist Scores

There are ten Specialist scores that are used to determine the various capabilities of a Specialist: Speed, Proficiency, Endurance, Charisma, Intelligence, Agility, Looks, Insight, Stamina and Toughness.

### Speed

Speed is both a measure of how fast your character can react during combat and movement speed. Use the following chart to figure out what your Speed Rating is, based on your Speed. The formula is Speed score divided by 10, and rounded up. The Specialist’s Speed Rating determines the number of movement units a Specialist may move for each move action they take as well as the number of Action Points, or AP they gain each round in combat.

| Speed score | 1-10 | 11-20 | 21-30 | 31-40 | 41-50 | 51-60 | 61-70 | 71-80 | 81-90 | 91-100 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Speed Rating | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 |

### Proficiency

Proficiency is a measure of your Specialist’s hand-eye coordination. Ranged martial components require a minimum Proficiency score of 15 for simple, 30 for basic, 45 for intermediate, 60 for advanced, and 75 for master. Specialists who intend to focus on thrown or projectile weapons favor their Proficiency stat.

### Endurance

Endurance is a measure of your resilience and is the governing stat for your Vitality. A Specialist’s maximum vitality is equal to their Endurance score. Endurance does not govern any skills.

### Charisma

Charisma is your force of personality. Charisma is used to persuade an audience or lead an army. Some magic energy components require a minimum Charisma score of 15 for simple, 30 for basic, 45 for intermediate, 60 for advanced, and 75 for master. Casters who wish to bend the will of others favor their Charisma stat.

### Intelligence

Intelligence is a measure of your logic, reasoning and the ability to process information. Some magic energy components require a minimum Intelligence score of 15 for simple, 30 for basic, 45 for intermediate, 60 for advanced, and 75 for master. Casters who wish to deal a lot of damage in combat or overcome logic based situations with spells favor their Intelligence stat.

### Agility

Agility determines how nimble and flexible you are. Some defensive martial components and advanced martial trainings require a minimum Agility score of 15 for simple, 30 for basic, 45 for intermediate, 60 for advanced, and 75 for master. Specialists who wish to dodge nimbly or excel at fighting with no armor favor their Agility stat.

### Looks

Looks are your overall appearance and can help a Specialist either stand out or blend in to a crowd.

### Insight

Insight is a measure of your overall understanding and empathy. Some magic energy components require a minimum Insight score of 15 for simple, 30 for basic, 45 for intermediate, 60 for advanced, and 75 for master. Casters who wish to deal in the body, life and death, or flashy effects favor their Insight stat.

### Stamina

Stamina is a measure of your pain tolerance and is used to determine a Specialist’s maximum Fatigue. Specialists who wish to wear armor require a minimum Stamina score of 15 for simple, 30 for basic, 45 for intermediate, 60 for advanced, and 75 for master.

### Toughness

Toughness is a measure of your physical strength, which determines your carrying limits. Melee weapon and shield martial components require a minimum Toughness score of 15 for simple, 30 for basic, 45 for intermediate, 60 for advanced, and 75 for master. Melee damage or tank focused martial Specialists favor their Toughness stat.

## Attacks

The attacks section is intended to give players a place to keep their favorite attacks written down, with all calculations already recorded to help speed combat along. The idea is to build a few attacks from your components to have them ready to go at a moment’s notice.

An attack is any action intended to cause harm, although not necessarily injury, to another, whether it be via martial attacks, casting a spell, or the use of skills. In game terms, this means that any action intended to damage or hinder an opponent is considered an attack.

### Basic Attacks

A basic attack is an attack that is strictly martial, strictly magic, or strictly skill. Attacks of this sort explained in the section of the respective type of attack.

### Hybrid Attacks

Hybrid attacks are those that combine martial, magic and/or skill into a single attack. For example, a sword charged with a spell counts as a hybrid attack. In such cases, the primary delivery method is used to determine whether the attack hits or misses. Damage is determined separately for each part of the attack. Special defenses may apply to magic portions of attacks, such as an opponent who attempts to ward the spell’s effect. The Keeper determines which part of a hybrid attack is the primary delivery vehicle.

## Racial Features

For gaming purposes, human is considered the standard race. For Specialists who are not human, the notes area in the Skills section of the Specialist Record is a good place to keep track of what makes them different.

### Standard Racial Features

Standard racial features are features that every creature has, simply by existing. These are race, size category, movement types (primary and alternative).

### Selective Racial Features

Some races have various features which set them apart from other races in different ways. Some may have wings, while others may have gills and fins. As such, many races have various racial features available to choose from during character creation. Some racial features cost advancement points, and provide a positive effect, while others essentially give an advancement point bonus and impose a negative effect. In general, the bonus advancement points from selecting negative features shouldn’t outweigh the advancement point cost of positive effects, though the Keeper may allow it on a case-by-case basis.

Selective racial features may only be purchased during character creation, though they may be improved later through regular advancement point expenditures. For example; a Specialist with Harpy blood may start the game with very basic, essentially useless wings, which could later be improved to provide gliding and even flight. If the same Specialist doesn’t take the wings at character creation, however, they shouldn’t be able to spontaneously grow wings later in life.

Selective racial features give players the ability to customize their Specialist’s race to fit their play style. In general, it should be assumed that any Specialist that only has a few of the available racial traits is a cross-breed. Only Specialists who have all the racial traits of a race are considered pure-blooded.

### Choosing a creature type

An important aspect of your Specialist is your creature type. In the process of creating your Specialist, you’ll want to decide what creature type your Specialist will be, and purchase racial features with your starting advancement points. Once you’ve chosen your creature type, you can’t purchase racial features that don’t belong to that creature type. If you can’t afford a racial feature with your starting advancement points, you may purchase them once you’ve earned more advancements, unless otherwise specified in the racial feature. For example, if your creature type is pixie, you may have vestigial wings on Specialist creation (namely because you couldn’t afford to purchase the Flight racial feature). Once you’ve earned more advancement points, you could purchase the Flight racial feature to make use of your wings. You can’t, however, start as a human, and suddenly decide you’re a centaur, and spontaneously have your legs turn to horse legs, and grow two more of them.

### Constructing your own creature type

We strongly caution you to obtain Keeper approval before you go about creating your own creature type. Once you have approval, we advise you to work closely with your Keeper to create your new creature type. This could be as simple as combining two creature types, and having the available racial features of both, or it could be as complex as grabbing numerous racial features and creating an entirely new creature type. If you’re just combining two creature types in equal proportions, your result will be known as a “half-breed”. If you’re combining racial features of two or more types, your result will be a “mixed-breed”. With a mixed-breed, find the highest concentration of racial features. The overall category those features belong to determine your primary creature type. For example, if you combine traits from monstrous, undead, and demonic creature types, but most of the traits you’ve chosen are from the undead types, your Specialist is considered undead.

# Experience Points and Advancements

Although Boundless doesn’t have predefined classes or levels, Specialists still have the ability to grow and advance. To that end, Specialists earn and use Experience Points (Exp.) to advance.

## Earning Experience Points

Specialists earn Exp. by adventuring and surviving encounters. Encounters can be combat, puzzle, trap, or even role play. Generally, an encounter is any situation in which a Specialist must use attacks, magic or skills.

## Advancements

Each time a Specialist gains an amount of Exp. equal to their current advancement, they gain another advancement. For example, a Specialist with 5 advancements gains another advancement when they’ve gained 500 additional Exp. Any Exp. beyond the amount needed for the next advancement roll over. Thus, with the previous example, if the Specialist gains enough Exp. to give them 531 Exp., they would become advancement 6, and have 31 Exp. (531 – 500 = 31) toward their next advancement.

When a Specialist earns an advancement, they gain 10 advancement points to spent on racial traits, stats, magic components, martial components, and skills. Racial trait costs are listed for each trait. Stats are purchased on a point for point basis, meaning each advancement point is good to increase a stat by 1 point. Magic and martial components cost are based on their tiers; 1 point for simple, 2 for basic, 3 for intermediate, 4 for advanced, and 5 for master. Skill ranks may be purchased at the same tier-based cost as magic and martial components, but only one tier of a given skill may be purchased in the same advancement, and the previous tier must already be purchased to learn the next. For example, a Specialist that has already learned simple Riding could purchase basic riding, but could not skip basic to purchase intermediate, nor could the Specialist purchase basic and intermediate Riding in the same advancement. A Specialist may advance different skills in the same advancement, such as Riding and Blacksmithing, regardless of the current tier of the skills, so long as the Specialist has enough remaining advancement points to purchase the prospective skill tiers.


## Death and Experience

As with most games, death carries a penalty. Although a corpse may be revitalized, the process of dying and being brought back to life takes a toll on the spirit. To reflect this, in Boundless, any unspent Exp. are lost whenever a Specialist dies.

# Bank and Possessions

The bank and possessions section of the Specialist Record is provided for Specialists to keep track of their wealth and possessions. This can be equipped, carried, or simply owned items, or even property.

### Equipment

Equipment consists of items a Specialist is able to carry around with them, and have ready to use at a moment’s notice. Generally, it refers to armor being worn, and weapons and/or shields held or readily available.

### Items

Items consist of objects a Specialist carries, but generally not those used in combat. These range from clothing, to jewelry, to food, to skill and trade kits.

### Property

Property is anything a Specialist owns, but isn’t currently carrying with them. This can be land, vehicles, animals, furniture, buildings, etc. Often, owned property requires staff to upkeep.

### Wealth

Wealth generally refers to the amount of Qwartz a Specialist carries, but can also encompass any other form of currency used to purchase or exchange for goods or services.

# Notes

The notes space on the Specialist Record is provided for players to make note of anything they feel is important. Many players like to quickly jot notes about ideas they have, adventures they’ve had, non-player Specialists (NPS), or even expand when other areas have run out of room. It’s also a good place to write down the final judgments of the Keeper any time a rules question crops up. The bottom line is, if it’s not written down, it’s not true. For example, if you intended to sew a lock pick into your tunic, but you didn’t write it down, you never did it.


---

# Chapter 3 — Combat, Defense, Movement, Health & Armor

## Reconstruction status legend

- **✅ CONFIRMED** — established by later explicit decisions and treated as current canon unless deliberately reopened.
- **🔄 SUPERSEDED** — recovered source material that has been replaced by a later decision.
- **⚠️ REVIEW / CONVERSION** — concept or content is useful, but one or more mechanics must be reconciled with the current engine.
- **⬜ NEEDS DEVELOPMENT** — incomplete or absent; substantial design work remains.
- **❗ CONTRADICTION** — two surviving sources or decisions conflict and must not be silently reconciled.
- **💡 SUGGESTION** — design suggestion from this reconstruction pass; not canon unless Mike approves it.

**Authority used in this reconstruction:** newest explicit decisions in the current reconstruction work override older text; CLEAN source files are the baseline for material not subsequently changed. Archival Markdown is treated as a searchable transcription of its CLEAN source, not as independent canon. No discrepancy has been silently fixed.

## 1. Combat sequence

**✅ Current core sequence**

1. Establish Initiative once at the beginning of combat using Speed-derived dice.
2. On a Specialist's turn, AP refreshes.
3. The acting Specialist spends AP on eligible actions within the tier ceiling of each action.
4. Opposed attacks compare the attacker's successes to the defender's chosen defense.
5. Defender wins: attack fails. Tie: Glancing Blow, 1d10 base damage. Attacker wins: net successes become damage dice.
6. Reactions/active defenses may consume AP reserved within the round.
7. Unused AP does not carry into the next turn.

**⚠️ REVIEW:** reaction priority, multiple reactions, exact tie-breaking for Initiative, delay/ready behavior, and simultaneous effects still need a formal timing section.

## 2. Attack and damage

**✅ CONFIRMED**

- One opposed attack-defense interaction replaces the CLEAN sequential to-hit → evasion → armor/block chain.
- Defender win = no normal damage.
- Tie = Glancing Blow = 1d10 base damage.
- Attacker win = one damage die per net attack success.
- Mixed damage retains source/type.
- One attack normally uses one weapon profile. Natural weapons are profiles. Dual-wield Components may explicitly construct an attack using two weapons.

## 3. Defense paths

**✅ CONFIRMED architecture**

A Specialist may know multiple defensive approaches, but **only one path contributes to any one defense roll**:

| Path | Governing Stat | Training | Equipment limitation |
| --- | --- | --- | --- |
| Unarmored | Agility | Unarmored Training | unavailable while wearing armor |
| Evasion | Insight | Evasion Training | unavailable in medium or heavy armor |
| Armored | Stamina | Armor Training | armor-path details and armor categories require the armor pass |

The chosen Stat contributes (1 + floor(Stat/10))d10. The chosen Training contributes +1d10 per degree.

**Passive Defense:** no AP; always available when a valid path exists. Whether Passive Defense can critically succeed or critically fail has been deliberately reopened for stress testing.

**Active Defense:** costs AP; replaces rather than stacks with Passive Defense; may add eligible defensive Components/Traits/equipment/modifiers. The same three base paths are available subject to equipment restrictions.

**✅ Shields:** do not add to Passive Defense by default; they are active defensive equipment unless a later explicit rule says otherwise.

## 4. Armor, shields, natural armor, and mitigation

**⚠️ MAJOR REVIEW PACKAGE**

Mitigation must **not** be silently deleted. CLEAN and later-integrated Martial content use armor rolls, shield rolls, armor mitigation, shield mitigation, penetration, favored shields, Rhino Hide, and related mechanics in multiple places. The whole ecosystem must be reviewed together before deciding what survives.

Current anchors:

- Natural armor and worn armor do not stack; worn armor overrides natural armor.
- Unarmored Training is incompatible with worn armor.
- Evasion is unavailable in medium/heavy armor.
- Shield bonuses are not part of Passive Defense.
- Exact armor dice, mitigation, armor category rules, shield mitigation, Penetration interactions, and equipment values are **not yet locked**.

## 5. Critical combat effects

**✅ Universal trigger:** combat uses the Critical Die from the core resolution engine. A successful action is Crit+ when its Critical Die shows a natural 10; a failed action is Crit- when its Critical Die shows a natural 1.

**✅ Attack Critical Success:** successful attack + Critical Die 10; double damage dice.

**⚠️ Provisional defensive Critical Success:** successful defense + Critical Die 10; -1d10 to the attacker's next attack against this same defender per excess defensive success. The effect remains under stress test, and Passive Defense eligibility is separately reopened for review.

**✅ / ⚠️ Attacker Critical Failure:** failed attack + Critical Die 1. The attacker takes **-1d10 to their next defensive action per natural 1 showing anywhere in the failed attack pool**. The previous "no further movement" consequence is no longer treated as settled; **half Movement Speed** is the current stress-test candidate.

**✅ / ⚠️ Defender Critical Failure:** failed defense + Critical Die 1. The attacker gains **+1 damage per damage die rolled**, retaining damage type/provenance. Applying the same half-Movement consequence to the defender is under stress test.

Natural 1s outside the Critical Die do not trigger Crit- by themselves, but they still scale an effect when a confirmed rule explicitly counts total natural 1s.

## 6. Movement in combat

**✅ Current architecture:** Speed no longer directly means ordinary travel distance. Movement Speed determines distance; MU is a Size-based distance multiplier. Standard movement is currently **5 MU**.

**⚠️ REVIEW:** complete Size→MU chart and the exact number/cost of ordinary movement actions per turn. Provisional anchors previously discussed were Small ≈4 ft/MU, Medium ≈6 ft/MU, Large ≈8 ft/MU, but the full chart is not canonized.

## 7. Vitality, Fatigue, downed, unconscious, death

**✅ Current state matrix**

| Vitality | Fatigue | State |
| --- | --- | --- |
| >0 | >0 | Functional |
| 0 | >0 | Downed |
| >0 | 0 | Unconscious |
| 0 | 0 | Dead |

- Endurance → Vitality 1:1.
- Stamina → Fatigue 1:1.
- Downed Specialists cannot take mechanical actions; speech remains possible.
- Stabilization stops ongoing deterioration but does not restore action; Vitality must be restored.
- **⚠️ REVIEW:** the remembered 5-Fatigue loss at the start of each Downed turn still needs source/decision verification before becoming final prose.

## 8. Charged, Conducted, Bestowed weapon/spell interactions

**✅ / ⚠️ Current direction**

- Charged: effect is held after enactment until it resolves or is dismissed.
- Conducted: magic is carried through a held nonstationary object; loss of contact dissipates it. If the delivery object's own melee damage is part of the action, resolve as a Martial+Magic hybrid; otherwise it behaves more like touch delivery.
- Bestowed: effect is transferred and persists on the carrier; structure/energy is fixed after bestowal. Later working rule: Conducted/Bestowed effects trigger on a hit or Glancing Blow, not a miss.

Exact AP/timing language still needs a final Magic pass.

## 9. Berserk and Meginserk

**⚠️ Later working design; needs final confirmation against the source chapter**

- Both are addictive drugs, not learned toggles.
- Fixed duration: 2d10 rounds.
- No bonus AP.
- No Active Defense; Passive Defense remains.
- At least half available AP each turn must be spent offensively.
- +1d10 offensive rolls per tier.
- +1d10 temporary Vitality per tier.
- Berserk uses Martial delivery; Meginserk uses Magic delivery.
- Crash: Fatigue loss = tier × rounds active, applied at once.
- Reaching 0 Fatigue from the crash causes unconsciousness, not automatic death.
- Addiction mechanics remain unresolved.

## 10. Recovered CLEAN Combat chapter

**🔄 Many resolution mechanics below are legacy.** This source is preserved in full because movement interactions, counterspelling concepts, charged/conducted/bestowed details, ammunition, and individual edge cases may still be valuable. Nothing below silently overrides the current rules above.

---

# Combat

All combat is an active process. To that end, all combat in Boundless is an active process as well. The defender doesn’t rely on hiding in his armored shell, hoping that the attacker doesn’t roll high enough to overcome his defense. Instead, the defender actively attempts to evade or deflect the incoming attack using their abilities. The only time a defender hides behind their armor is when they are shielding, as described below, and even then, this is an active defense.

# Combat Order & Action Points

In combat, time is broken into segments called “rounds”. In each round, each creature has a number of Action Points, or AP equal to their Speed Rating. For example, a creature with a Speed Rating of 3 would have 3 AP in a round. Each creature gains AP at the beginning of each round, but may only spend AP on defensive actions before their turn in the combat order.

To begin combat, each creature rolls a number of d10 equal to their Speed Rating to determine the combat order. Starting with the highest combat order score and working down to the lowest, each creature takes their turn. Creatures may attempt to increase their combat order roll by adding luck points. A lucky flip adds to the creature’s combat order result, while an unlucky flip subtracts from it. Combat order ties between players go to the Specialist with the higher Speed score. If the Specialists share the same Speed score, the players may roll again, play rock/paper/scissors, or use any other quick method for the purpose of determining which goes first, though their original combat order result is unchanged. Combat order ties between players and non-players always go to the players. Combat order ties between non-players are decided by the Keeper.

Each subsequent round, everybody rolls a new combat order. This represents how chaotic combat can be, and helps keep players and foes on their toes. Alternatively, the Keeper can rule that the initial combat order is the combat order for all subsequent round.

# Combat Actions

Combat actions are any actions a creature or Specialist can take during combat, whether to attack, defend, use a skill, or cast a spell.

During a creature’s turn, the creature gets 1 movement action automatically. In addition, they may use any AP they have to attack, defend or gain additional movement actions. In the first round of combat, a creature may not take defensive actions until after their first turn in the combat order. AP not used by the start of your next turn are wasted, and do not roll over.

# Combat Movement

Combat movement is based on each individual creature or Specialist’s movement units, or MU. A creature’s movement unit is based on their size category. In combat, a creature taking a move action may move a number of movement units equal to their Speed Rating.

# Attack and Defense

## Active Attack and Defense

Attacks may consist of martial components, magic components, skill components or any combination thereof. Defenders may be able to evade attacks entirely, or, failing that, block them with armor and/or shields. Specialists may also attempt to counterspell incoming harmful spells if they know the appropriate opposing energy.

The first stage in any attack is the attack roll versus the defender’s defense roll. The attacker’s “to-hit” roll consists of attack dice provided by the Specialists weapon and any weapon training plus any Luck modifier and any bonuses provided by descriptive text of components used. For example, a Specialist without training using a small melee weapon would get 4d10 to hit with their weapon, a penalty of 1d10 for not being trained for a total of 3d10. This Specialist may add up to 3d10 Luck dice to this roll (the number of Luck dice used must be specified before making the attack roll). On a lucky flip, this Specialist would roll 6d10 to hit. On an unlucky flip, this Specialist would roll 3d10 to hit then roll 3d10 Luck dice to subtract from the previous total.

The defender begins by rolling Evasion, if any, provided by Evasion Training, Unarmored Training, AP spent on the Evade defensive component and any Luck dice the defender wishes to add. If this is enough to beat the attackers to-hit roll the attack is evaded and the defender takes no damage.

If the evasion roll fails to beat the attackers to-hit (or has no evasion to roll) then the Specialist will roll an armor/block and may add in any additional defensive components they know, and have AP to do so, as well as any Luck dice they wish to add. If there was an evasion roll made, the total is added to the armor/block roll which constitutes the defender’s total defense roll. If the defender’s total defense roll is sufficient to beat the attackers to-hit roll the attack is considered a glancing blow and the defender takes no damage. If the to-hit roll is greater than or equal to the defender’s total defense roll, the attack moves to the damage and mitigation phase.

### Determining Attack Success

If the attacker’s to-hit is lower than the defender’s evasion roll, the attack is evaded. If the to-hit is higher than the evasion roll, but lower than the total defense roll, the attack is a glancing blow. If the to-hit is higher than the total defense roll, the attack is a hit.

### Hybrid Magic and Martial Attacks

An attack that consists of a martial weapon charged with magical energy counts as a martial attack, and is subject to being blocked as a normal martial attack. The exception is glancing blows. If the energy used is a type that cannot be blocked by physical means, such as a charm, or one that bypasses armor, such as an electricity spell, the spell portion of the attack still occurs. Treat the magic portion of the attack as normal.

### Counterspelling

Counterspelling magic works in one of two ways. The first way a Specialist may attempt to counterspell is to attack the incoming energy with an opposing energy type. In this case, the defender would roll an opposing attack roll in lieu of a defense roll. Beating the initial attacker’s attack roll means the spell has been successfully counterspelled, and the energies negate each other. Failing to beat the initial attacker’s roll means the spell is not counterspelled, and hits the defender. In this case, the defender’s energy dissipates harmlessly.

The second way a Specialist may attempt to counterspell is to create a shield of an opposing energy type to block the incoming energy. In this case, the defender may add any defensive components that would normally be able to be applied to a shield. Roll defense normally. A successful block roll means the energies negate each other. A failed block means the spell still hits the defender, and may be subject to damage mitigation, though the shield spell may persist, if cast with duration longer than instantaneous.

When attempting to counter spells of mixed energies, energy that opposes any of the energies in the attack is sufficient to counter the entire spell, as the energies in the attacking spell merge to form a new energy type. For example, a spell using cold and electric energies could be countered using fire energy.

 As an alternative rule, the Keeper may specify that only opposable energies may be countered, and other energies can’t be countered. Using the example above, fire energy would be able to counter the cold energy from a cold and electric energy spell, but the electric energy would still hit the defender.

## Size Category Modifiers

For each size category larger or smaller a target is than an attacker, there is a cumulative bonus or penalty of 5 to hit that target. For example, a medium Specialist attacking a huge target (2 size categories larger) would get a bonus of 15 (5 + 10 = 15) on their attack rolls, while the huge Specialist attacking the medium target would suffer a penalty of 15.

Specialists that get a bonus to hit take an equal penalty on their damage roll. Conversely, Specialists that get a penalty to hit gain an equal bonus on their damage roll. For example, a medium Specialist attacking a huge target gains 15 to hit, but would take a penalty of 15 to damage. This penalty can reduce damage to 0 points, and is applied after all other bonuses and/or penalties.

## Damage and Mitigation

When the attacker overcomes the defenders defense, combat proceeds to the damage mitigation phase. Defenders who make a “raw” defense add mitigation provided by their armor, if any. Mitigation of 1d10 points for light armor, 2d10 points for medium armor and 4d10 points for heavy armor.

The attacker’s damage roll consists of 1d10 per AP spent on the attack, plus any Luck modifier they wish to use, plus any modifier provided by the descriptive text of the components used in the attack. For example, 3 AP spent gives 3d10 (4, 7, 9), Luck modifier of 25 (with a lucky flip), with no additional modifiers would result in a total of 45 damage. (4 + 7 + 9 + 25 = 45).

The defender’s mitigation roll consists of mitigation provided by armor (0, 1d10, 2d10 or 4d10), plus 1d10 per AP spent on defense, plus any Luck modifier plus any bonus provided by the descriptive text of the defensive components used. For example, medium armor gives 2d10 (3, 6), 2 AP spent gives an additional 2d10 (4, 8), Luck modifier of -10 (with an unlucky flip), with no additional modifiers would result in a total of 11 defense (3 + 6 + 4 + 8 – 10 = 11).

Using the above examples, the defender would take 34 points of Vitality Pool damage. (45 – 11 = 34). If the defender’s mitigation is higher than the attacker’s damage, the damage is negated and the attack is considered a glancing blow. Physical Magic Attacks

Defending against magic attacks that mimic physical attacks works just like defending against physical attacks of the same sort. For example, a projected spell would be defended against just like a crossbow bolt. Magic structures that mimic physical attacks list the attacks they mimic in their descriptions.

Magical attacks that mimic physical attacks, such as touch, thrown and projectile (and charged weapons), are opposed by physical defenses. They can be blocked, either partially or completely, by armor and shields. If they are not fully blocked, armor still mitigates some of the damage as normal only if the energy deals direct damage. Any energy that is fully blocked by armor or shield dissipates harmlessly. A Specialist attempting to catch an energy is thereby giving up any physical defense to the energy in question. Mental defense may still be applicable. For example, a Specialist that catches an arrow charged with a Charm 2 (Captivation) spell may still make their opposed Charisma check to resist the spell.

Energies with their own specifically noted defense mechanisms can still be defended against with armor and shields if delivered by methods which mimic physical attacks. Specialists still get a chance to defend as noted in the energy description if the armor and/or shield fails to block the energy fully.

Prohibitive energies, such as Death energy, have their own restrictions listed in the energy descriptions. Failure to meet these requirements means that the spell itself fails. A failed spell still costs AP as usual, but deals no damage and does not affect any target. Should a prohibitive energy spell be successfully cast, it immediately takes effect as per the description of the spell. No other defenses are allowed unless specifically noted in the description.

Prohibitive energies are energies that have their own natural defenses in place. For example, Death energy spells being prevented from successful casting by virtue of the target having a huge vitality pool.

Energies that have special defense requirements have such spell defense requirements listed in the spell description, such as Charm energy.

## Actions as part of movement

As part of movement, a Specialist may draw a weapon or nock an arrow. More complex actions, such as loading a crossbow may not be taken without the use of Quick Load. Without the use of the Mobile Attack, Mobile Shot or Mobile Throw, Specialists may not attack as part of a movement action.

# Magical Attack and Defense

Magic attacks and defense are performed similar to martial attacks and defense, but they are separate from martial attacks and defenses as well. Magic has special rules for certain attack actions based on the structures used in a spell. Martial attacks charged with energy are considered martial attacks for the purposes of attack and defense.

## Magic actions as part of movement

Spells cannot be cast as part of movement. Prepared spells may be used as part of movement if circumstances would otherwise allow them to be used. Concentration spells may be maintained during movement. Spells may be cast while moving, if movement is by virtue of a vehicle or beast of burden.

# Critical Success & Failure

When rolling the dice, doubles count as a critical hit while a roll of 01 counts as a fumble. For example, 00, 11, 22, 33, 44, 55, 66, 77, 88 and 99 are all critical success. This gives the Specialist a 10% chance for critical hits and a 1% chance to fumble.

## Critical success

A critical success occurs when a Specialist rolls doubles on a to-hit or defense roll. When this happens the attack or defense automatically succeeds unless the opponent also rolls a critical. If both attacker and defender roll critical successes, combat is resolved as normal.

## Critical failure

A critical failure occurs when a Specialist rolls “01” on a to-hit or defense roll. When this happens, the attack or defense automatically fails. A Specialist who critically fails loses all remaining AP until their next turn. The Keeper may impose a further negative effect, such as the loss of a weapon or shield, at their discretion, which constitutes a fumble.

## Counterattack

Any time an attacker critically fails an attack and the defender critically succeeds at their defense, the defender has an opportunity to turn the attack back on the attacker. In such circumstances, the attacker rolls for damage as normal. Once the damage is determined, the attacker takes the damage, less any mitigation provided by their armor. Any defensive components that the defender chooses to use in this scenario will automatically succeed.

If the defender is using the Catch defensive component against a ranged attacker and a counterattack occurs, the defender may choose whether to catch the projectile or return the attack to the original attacker.

# Charging Weapons & Ammunition

Through the combined use of magic and martial abilities, martial weapons can deliver magical energies. Unarmed attacks can be combined with charged energies. Melee weapons can be combined with conducted or bestowed energies. Ranged weapons can be combined with bestowed energies.

Any martial attack which carries magical energy is resolved first as a martial attack, using training and to hit bonuses the Specialist has for the weapon, and any bonuses given due to the use of martial components. Depending on the result of the roll to hit, the energy may either be used, or remain.

## Charged unarmed attacks

In a charged unarmed attack, the energy is released if the attacker makes physical contact with the defender, whether the attack does damage or not. If the attacker completely misses the defender, or the defender evades the attack, the charged energy remains.

If the attacker hits the defender, but fails to deal damage with the martial components of the attack, the magical energy may still deal damage to the defender. For example, if the attacker has electrical energy charged, and the defender manages to block the attack with a metal shield, the defender may still take electrical damage. Special situations like this should be handled by the Keeper.

Other types of energy that only require touch to be effective may still bypass the armor entirely, such as the various Charm energies, still affect the defender on a successful hit, even if all the physical damage is mitigated.

## Conducted melee attacks

In a conducted melee attack, the energy is released if the weapon conducting the energy makes physical contact with the defender, whether the attack does damage or not. If the weapon completely misses the defender, or the defender evades the attack, the conducted energy remains. If the weapon ceases to be in contact with the wielder, the energy dissipates harmlessly.

If the weapon hits the defender, but fails to deal damage with the martial components of the attack, the magical energy may still deal damage to the defender. For example, if the attacker has electrical energy conducted, and the defender manages to block the attack with a metal shield, the defender may still take electrical damage. Special situations like this should be handled by the Keeper.

Other types of energy that only require touch to be effective may still bypass the armor entirely, such as the various Charm energies, still affect the defender on a successful hit, even if all the physical damage is mitigated.

## Bestowed melee attacks

A weapon bestowed with energy works exactly like a weapon with conducted energy when used for melee attacks, except that the energy remains even if the wielder ceases to be in contact with the weapon. For example, the attacker could throw the weapon, and the energy would remain until the weapon comes into contact with a viable target. For example, if the caster adds the selective target structure component to the spell, and specifies the energy only goes off when the weapon comes in contact with a troll, the weapon will remain charged until it hits a troll.

If the weapon hits the defender, but fails to deal damage with the martial components of the attack, the magical energy may still deal damage to the defender. For example, if the attacker has electrical energy conducted, and the defender manages to block the attack with a metal shield, the defender may still take electrical damage. Special situations like this should be handled by the Keeper.

Other types of energy that only require touch to be effective may still bypass the armor entirely, such as the various Charm energies, still affect the defender on a successful hit, even if all the physical damage is mitigated.

## Bestowed ranged attacks

In a bestowed ranged attack, the energy is released if the weapon or ammunition conducting the energy makes physical contact with the defender, whether the attack does damage or not. If the weapon or ammunition completely misses the defender, or the defender evades the attack, the bestowed energy remains. The energy remains even if the wielder ceases to be in contact with the weapon, until the weapon comes into contact with a viable target. For example, if the caster adds the selective target structure component to the spell, and specifies the energy only goes off when the weapon comes in contact with a troll, the weapon will remain charged until it hits a troll.

If the weapon or ammunition hits the defender, but fails to deal damage with the martial components of the attack, the magical energy may still deal damage to the defender. For example, if the attacker has electrical energy conducted, and the defender manages to block the attack with a metal shield, the defender may still take electrical damage. Special situations like this should be handled by the Keeper.

Other types of energy that only require touch to be effective may still bypass the armor entirely, such as the various Charm energies, still affect the defender on a successful hit, even if all the physical damage is mitigated.

# Death/ Dying/ Unconsciousness

Dead, dying and unconscious Specialists are those who are in dire straits. Any of these conditions are sure to ruin somebody’s day (at least temporarily). Below, we’ll discuss each of these maladies from least to most severe.

## Unconsciousness

A Specialist is rendered unconscious if their remaining Vitality points or their remaining Fatigue points reach 0 or negative numbers. In either case, the Specialist regains consciousness only when both pools are at 1 point or more, whether by magical energy or rest. If a Specialist is successfully attacked while unconscious, the attack is treated as a coup de grace, and instantly kills the Specialist.

Specialists in a berserking or meginserking state are the exception to this rule, as they can remain conscious if their Vitality pool (but not their Fatigue pool) reaches 0 or below, and will continue to fight until they die, or the effects of the drug wear off. Specialists, even with proper training in the drug taken, immediately slip into a comatose state if they’re at or below 0 Vitality points when the drug wears off. They only regain consciousness when their full natural Vitality pool is restored.

## Dying

A Specialist is considered to be dying if their Vitality points are at or below 0, and are continuing to drop. For each round a Specialist is dying, they lose 1d10 Vitality Points plus any additional points from ongoing damaging effects, such as being on fire.

A dying Specialist has a chance to stabilize equal to their Stamina score on each of their actions. Specialists who stabilize take no further damage from dying, and may begin to recuperate through rest. Specialists who fail to stabilize continue to take damage. As with unconscious Specialists, an attack on a dying Specialist is treated as a coup de grace, and results in instant death.

## Death

A Specialist dies if their Vitality points reach a negative number equal to their Endurance Score. For example, if a Specialist’s Endurance Score is 70, the Specialist is dead if their Vitality points reach -70 or lower.

Specialists taking berserking or meginserking drugs with concentration tiers higher than their training level immediately die when the effects of the drug wear off (berserkers’ hearts explode, and meginserkers’ brains turn to mush).

A dead Specialist loses all unspent Experience Points and may only be revived by use of a Life energy spell of sufficient strength.

# Berserk & Meginserk

Through proper training, and use of potentially lethal addictive substances, Specialists may enhance their combat prowess for short periods of time. This is known as berserking for martial Specialists, and meginserking for magic Specialists.

## Berserking

When a Specialist ingests one or more doses of the berserking drug, they gain a few bonuses and penalties. The Specialist gains temporary Vitality pool ranks and Action Points per round equal to the concentration tier of the drug. The Specialist also gets a bonus to damage equal to 1d10 per tier per attack, and a penalty to defense equal to 10 times the concentration tier. For example, if a Specialist imbibes a dose of concentration tier 3 berserking drug, they gain 3 temporary Vitality pool ranks and 3 AP per round. The same Specialist would get a bonus of 3d10 damage on all martial attacks, as well as a penalty of 30 to evade attempts. Specialists under the effects of the berserking drug are incapable of conscious defense, and forego defense rolls.

While in the Berserk state, Specialists are not capable of the patience or focus is takes to make complicated mental maneuvers such as spells or wielding projectile weapons. For this reason, they are only able to use the following actions, assuming they have purchased them: Wrestling, Dual Throw, Mobile Attack, Piercing Throw, Follow Through, Overwhelm and Whirlwind. A berzerking Specialist may take advantage of Double Threat training only if it involves a thrown weapon for the ranged weapon specification.

Specialists who take doses with higher concentration tiers than they’re trained to handle die immediately when the drug wears off due to their heart exploding. Specialists with proper training enter a stupor if they have one or more Vitality points, or slip into a coma if their Vitality points are at or below 0 when the drug wears off.

## Meginserking

When a Specialist ingests one or more doses of the meginserking drug, they gain a few bonuses and penalties. The Specialist gains Vitality Pool ranks and Action Points per round equal to the concentration tier of the drug. The Specialist also gains 1d10 damage per tier per spell, and get a penalty to defense equal to 10 times the concentration tier. For example, if a Specialist imbibes a dose of concentration tier 3 meginserking drug, they gain 3 Vitality pool ranks and 3 AP per round. The same Specialist would get a penalty of 30 to evade attempts. Specialists under the effects of the meginserking drug are incapable of conscious defense, and forego defense rolls.

While in the meginserk state, Specialists are not capable of taking any martial actions, as their neurons fire rapidly, and the Specialist is overwhelmed with magical energy. Such Specialists must attempt some sort of magical action on each of their actions.

Specialists who take doses with higher concentration tiers than they’re trained to handle die immediately when the drug wears off as their brains liquify. Specialists with proper training enter a stupor if they have one or more Vitality points, or slip into a coma if their Vitality points are at or below 0 when the drug wears off.

# Ammunition Recovery

For Specialists that use projectile weapons, ammunition has the potential to be fairly expensive. There is also a possibility that ammunition that hasn’t been damaged may be recovered. Certain circumstances may make a particular arrow, bolt, rock, etc. unable to be recovered, such as a troll fleeing with an arrow sticking out of his shoulder. In general, though, about 10% of used ammunition should be able to be recovered by the owner (or left to be recovered by scavengers, if the owner doesn’t take the time to recover it).


---

# Chapter 4 — Skills

## Reconstruction status legend

- **✅ CONFIRMED** — established by later explicit decisions and treated as current canon unless deliberately reopened.
- **🔄 SUPERSEDED** — recovered source material that has been replaced by a later decision.
- **⚠️ REVIEW / CONVERSION** — concept or content is useful, but one or more mechanics must be reconciled with the current engine.
- **⬜ NEEDS DEVELOPMENT** — incomplete or absent; substantial design work remains.
- **❗ CONTRADICTION** — two surviving sources or decisions conflict and must not be silently reconciled.
- **💡 SUGGESTION** — design suggestion from this reconstruction pass; not canon unless Mike approves it.

**Authority used in this reconstruction:** newest explicit decisions in the current reconstruction work override older text; CLEAN source files are the baseline for material not subsequently changed. Archival Markdown is treated as a searchable transcription of its CLEAN source, not as independent canon. No discrepancy has been silently fixed.

## 1. Skill architecture

**✅ CONFIRMED**

- Anyone may attempt any Skill. Training is expertise, not permission.
- Skills use the same d10 success-counting engine as the rest of Boundless.
- Skill Training is described by **degree**: Simple, Basic, Intermediate, Advanced, Master.
- Minimum governing Stats for those degrees are 15 / 30 / 45 / 60 / 75.
- Training contributes +1d10 per degree.
- The governing Stat contributes (1 + floor(Stat/10))d10.
- CLEAN restrictions that require an untrained Specialist's Stat to qualify for the attempted degree, halve untrained dice, forbid Meticulous attempts, or automatically make untrained failure disastrous are **🔄 superseded** and remain in the graveyard. They are not part of the modern Skill system.

## 2. CLEAN thresholds and why they cannot be used directly

**⚠️ CONVERSION REQUIRED**

CLEAN uses summed face values of the d10s. Its normal success targets are recorded as 6 / 18 / 26 / 40 / 50 in the transcription (Mike recalled 24 for Intermediate during reconstruction; this discrepancy must remain visible). CLEAN also contains separate failure bands and Progressive/Productive targets. Those numbers do not translate directly into a system where each die is simply success/failure.

No silent numerical translation is made here.

## 3. Skill difficulty thresholds

**✅ CONFIRMED**

Skill difficulty is independent of the Specialist's Training degree. A task has an inherent tier; Training and governing Stat determine the dice available to meet that threshold.

| Task tier | Successes required |
| --- | ---: |
| Simple | **2** |
| Basic | **3** |
| Intermediate | **4** |
| Advanced | **5** |
| Master | **6** |

At the minimum governing Stat and matching Training degree, baseline pools and success rates are:

| Tier | Minimum Stat | Stat dice | Training dice | Total pool | Success chance |
| --- | ---: | ---: | ---: | ---: | ---: |
| Simple | 15 | 2d10 | +1d10 | **3d10** | **50.00%** |
| Basic | 30 | 4d10 | +2d10 | **6d10** | **65.63%** |
| Intermediate | 45 | 5d10 | +3d10 | **8d10** | **63.67%** |
| Advanced | 60 | 7d10 | +4d10 | **11d10** | **72.56%** |
| Master | 75 | 8d10 | +5d10 | **13d10** | **70.95%** |

The higher baseline reliability at Advanced and Master is intentional. The threshold progression remains the simple 2 / 3 / 4 / 5 / 6 ladder rather than introducing irregular exceptions merely to flatten percentages.

Anyone may attempt any Skill. A Specialist may simply have too few dice for a particular task to be realistically or mathematically achievable; this is an emergent limit rather than an explicit permission gate.

## 4. Critical and Overwhelming Skill outcomes

**✅ CONFIRMED**

Every Skill roll includes one identifiable **Critical Die**: the persistent base +1d10 already included in the normal dice pool. It is not an additional die.

- **Critical Success (Crit+):** the Skill check succeeds and the Critical Die shows a natural 10.
- **Critical Failure (Crit-):** the Skill check fails and the Critical Die shows a natural 1.
- A 10 on the Critical Die does not create Crit+ if the underlying check fails.
- A 1 on the Critical Die does not create Crit- if the underlying check succeeds.

At a physical table, use a visually distinct die. In digital resolution, identify the Critical Die internally.

**Overwhelming Success (OwS)** occurs when the roll reaches 150% of the normal success threshold, rounded up:

| Tier | Normal threshold | OwS threshold |
| --- | ---: | ---: |
| Simple | 2 | **3** |
| Basic | 3 | **5** |
| Intermediate | 4 | **6** |
| Advanced | 5 | **8** |
| Master | 6 | **9** |

**Overwhelming Failure (OwF)** occurs when a failed Skill check falls short of the normal success threshold by **3 or more successes**:

| Tier | Normal threshold | OwF result |
| --- | ---: | ---: |
| Simple | 2 | **Impossible** |
| Basic | 3 | **0 successes** |
| Intermediate | 4 | **0-1 successes** |
| Advanced | 5 | **0-2 successes** |
| Master | 6 | **0-3 successes** |

OwS and Crit+ may occur together. OwF and Crit- may occur together.

Outside the universal classification of these outcomes and their extended-check values, their exact consequences are Skill-specific and situation-specific. The Keeper should use judgment based on the task, tools, materials, environment, and stakes. Individual Skills should provide concrete examples of suitable exceptional results without turning those examples into a rigid universal consequence table.

## 5. Hasty, Meticulous, Progressive/Productive, Ongoing use, and Teamwork

### Hasty and Meticulous

**✅ CONFIRMED**

**Hasty:** complete the task in **half the normal time** and apply **-1d10 per tier of task difficulty**.

**Meticulous:** take **double the normal time** and gain **+1d10 per tier of task difficulty**.

| Tier | Hasty | Meticulous |
| --- | ---: | ---: |
| Simple | -1d10 | +1d10 |
| Basic | -2d10 | +2d10 |
| Intermediate | -3d10 | +3d10 |
| Advanced | -4d10 | +4d10 |
| Master | -5d10 | +5d10 |

The Keeper has final authority over whether Hasty or Meticulous is possible in the circumstances, and circumstances may effectively require one mode. These are the universal pace-based Skill modifiers.

The CLEAN-era generic favorable/unfavorable circumstance ladder is **🔄 superseded and removed**. Other advantages or disadvantages should come from concrete sources such as tools, equipment, Traits, Magic, Conditions, assistance, environmental rules, or Skill-specific rules. The Keeper may instead assign a different task tier when circumstances fundamentally change the task itself.

### Progressive / Productive / Ongoing checks

**✅ CONFIRMED**

Extended tasks use the same normal Skill thresholds as ordinary checks. A current task or stage succeeds when the Specialist accumulates **4 success marks before 4 failure marks**; it fails when **4 failure marks** are accumulated first.

| Roll result | Extended-check effect |
| --- | ---: |
| Ordinary Success | +1 success mark |
| Ordinary Failure | +1 failure mark |
| OwS | +2 success marks |
| Crit+ | +2 success marks |
| OwF | +2 failure marks |
| Crit- | +2 failure marks |
| OwS + Crit+ | **Automatic success/completion of the current task or stage** |
| OwF + Crit- | **Automatic failure of the current task or stage** |

Checks occur at the end of the Skill's appropriate time interval and/or when a meaningful unexpected event or disruption threatens progress. Individual Skills and degrees should specify reasonable intervals wherever practical.

Routine sustained activity does not require constant rerolling solely to manufacture failure. For very large projects, divide the work into stages; automatic completion or failure resolves the current stage rather than necessarily resolving the entire project.

### Teamwork / Assistance

**✅ CONFIRMED**

When a Skill reasonably allows another Specialist to help, one Specialist is the **Primary** and makes the Skill check. Assistance does **not** add dice to the Primary's pool. Instead, it grants rerolls after the Primary's initial roll.

#### Helper limit

- Normally, only **one Helper** may assist a Skill check.
- The Keeper may allow more than one Helper in edge cases where the Skill and task naturally allow several people to contribute.
- A particular die may **never be rerolled more than once**, even when multiple Helpers are permitted.

#### Assistance rerolls

| Helper Training | Rerolls granted |
| --- | ---: |
| Untrained | **1d10** |
| Simple | **1d10** |
| Basic | **2d10** |
| Intermediate | **3d10** |
| Advanced | **4d10** |
| Master | **5d10** |

The Primary chooses which eligible dice to reroll.

#### Reroll restrictions

- Each die may be rerolled **only once**.
- A reroll **replaces the original result**, even if the new result is worse.
- The **Critical Die may be rerolled**.
- If the Critical Die is rerolled, its new face determines whether Crit+ or Crit- applies.
- Assistance can therefore improve or worsen ordinary success, Critical outcomes, and Overwhelming outcomes.

For extended tasks, assistance applies only to the checks for which the Helper is actually participating.

### Skills in combat

**✅ CONFIRMED**

Using a Skill actively during structured combat normally costs **1 AP per Skill check**, unless the Skill or another explicit rule states otherwise. The Skill's tier does **not** change that AP cost.

- **Active Skill check:** 1 AP.
- **Passive or reflexive Keeper-triggered Skill check:** 0 AP.
- **Assisting another Specialist:** the Helper spends 1 AP to provide Teamwork rerolls.
- A Specialist may make more than one Skill check in a turn if they have the AP and the actions make sense; there is no universal one-Skill-check-per-turn limit.
- The actual time required by the task still matters. A Skill may only be used in combat if the task can reasonably be performed on that timescale.
- Hasty still halves the task's normal time and applies its normal dice penalty. Hasty does not turn a long-form task into an instantaneous combat action.
- The Keeper may rule that a task cannot be attempted under current combat conditions when it requires sustained concentration, workspace, access, tools, or time that are not available.
- Extended and ongoing Skill tasks may continue through combat when circumstances allow. AP is spent when a check is actually made; AP is never banked across turns toward a future Skill check.

#### Meticulous use during combat

A non-ongoing Meticulous Skill check may be attempted during structured combat when the task and circumstances allow it.

- The check still costs **1 AP**.
- Meticulous remains subject to its normal **double-time** requirement and **+1d10 per task tier** bonus.
- The Meticulous Skill check is the Specialist's **only proactive action on that turn**.
- The Specialist may still reserve and spend available AP for **Active Defense or other eligible reactions** after the check.
- Passive Defense remains available as normal.

If a Meticulous task becomes an ongoing or extended Skill task because of its actual time requirement, use the normal ongoing/extended Skill rules instead. On a turn when an ongoing Skill task demands the Specialist's sustained attention, **Active Defense is normally unavailable unless it is reasonable to perform both at once**. The Keeper has final say based on the task and circumstances.

#### Independent Skill actions and attacks

Skill checks may be used independently during the same turn as an attack. Resolve each as its own action and pay its normal AP cost.

For example, a Specialist might attempt an Acrobatics check, then a Jumping check, then make a 6 AP attack. All costs come from the same turn's available AP, but the checks and attack are independent.

Failure on an earlier independent Skill check does **not** automatically cause later actions to fail. If the situation still permits it, the Specialist may adapt and continue. A failed wall-run or jump might leave the Specialist on the ground, after which they can move normally and make the planned attack if they still have the AP and opportunity to do so.

Independent Skill checks do not grant a generic bonus to a later attack.

#### Integrated Skill maneuvers

A Specialist may instead declare one or more meaningful Skill checks as **part of an attack setup**. This creates a higher-risk, higher-reward integrated maneuver.

- Each integrated Skill check costs **1 AP**.
- The attack also costs whatever AP the Specialist invests in it under the normal attack rules.
- All costs come from the Specialist's normal AP for that turn.
- For **each AP spent on integrated Skill checks**, the attack gains **+1d10** if every required setup Skill check succeeds.
- The Skill checks must be materially relevant to creating the attack opportunity. Ordinary movement or trivial actions do not qualify merely to manufacture bonus dice.
- Resolve the integrated Skill checks in sequence before the attack.
- If **any** required integrated Skill check fails, the **entire integrated maneuver fails** and the attack is not made.
- AP committed to the integrated maneuver is spent even if the maneuver fails.
- A successful integrated Skill check does not create any additional generic bonus beyond the confirmed **+1d10 per Skill AP spent**; other benefits must come from an existing rule, Condition, Martial Component, Skill-specific rule, or the actual fictional position created.

This gives Specialists a choice between cautious sequencing and flashy commitment: independent Skill actions are safer and recoverable, while integrated Skill maneuvers risk the whole sequence in exchange for bonus attack dice.

A Meticulous Skill check cannot be used as part of an integrated attack maneuver because Meticulous use consumes the Specialist's proactive focus for the turn.

## 6. Complete recovered Skill catalog

Every Skill below is retained because degree-by-degree capability descriptions are valuable even when the resolution math is obsolete. The annotation under each heading is part of this reconstruction; the Skill text itself is recovered from CLEAN.

---

# Skills

Skills affect every aspect of a Specialists day-to-day living. Anyone can use any skill at any time without any training. A Specialist can balance on a board with little effort (no training) but would probably wobble around and possibly fall off, assuming they had only an average Agility score. However, an Acrobat (a Specialist trained in Balance) could do cartwheels and other maneuvers while traversing a tightrope; something the first Specialist could only watch in awe, unless they felt like breaking every bone in their body trying to mimic the Acrobat.

In order for a Specialist to acquire training in any skills, they have to meet the minimum requirements. Initially, to train simple Skills, a Specialist needs to have a 15 in the relevant score. For example, to train in Ride, a Specialist would need to have an Insight score of 15, while Diplomacy would require a Charisma score of 15. Although day-to-day use of a Skill untrained is common, it does not always guarantee success. For example, anyone can make a sword, but without training, the sword would most likely break at the first use and look only vaguely like a sword. A master level smith could not only make a sword, but add filigree inlay, acid etching, lattice work, and more, with the sword being able to carry an edge that would make a two-dimensional object appear dull in comparison.

The Skills have different degrees of mastery. Initially, as described above, the Specialist needs to have only a 15 in the relevant governing score for simple training. The basic degree requires the Specialist to have a 30 in the relevant governing score, intermediate skills require 45 in a particular score, advanced requires 60, and master degree skill training requires a 75 in the relevant governing score. By default, a Specialist may not take more than one degree of a skill with a single Skill purchase. This represents the need to practice certain techniques before proceeding to more complex techniques. However, a Keeper may make exceptions for special circumstances, or as a house rule. A Specialist may not jump straight to master degree of a skill.


Using Skills

In order to overcome a skill challenge, a Specialist must first determine whether to attempt the skill hastily or normally, or, if circumstances permit, meticulously. Attempting a skill hastily has the increased potential to end in disaster on a failed attempt. On the other hand, a skill used meticulously has a decreased chance to end disastrously. Skills that take longer than one round to use are checked in time increments based on the skill being used whether it be once an hour, once a day, once a week, etc.

### Skill Check Success/Failure
> **Status:** ⚠️ REVIEW / CONVERSION — the concept may survive, but the legacy summed-die thresholds and any fixed numerical resolution must be converted to the current success-counting engine.

To make a trained skill check, a Specialist rolls a number of d10 equal to the 10s digit of the skill's governing stat. For example, a Specialist with 50 Charisma attempting to make a Diplomacy check would roll 5d10.

For normal skill checks, the minimum result required to succeed is 6 for simple, 18 for basic, 26 for intermediate, 40 for advanced and 50 for master. A failure is a roll of 1 for simple, 6 or less for basic, 12 or less for intermediate, 24 or less for advanced, and 35 or less for master. Any roll that is neither a success nor a failure simply represents no meaningful progress. Skill checks that don't have immediate results require a number of successful checks inversely proportional to the degree of the skill check being attempted. Simple degree skill checks require five successful rolls. Intermediate checks require four success rolls, and so on. If a Specialist accrues a number of failed rolls equal to the degree of skill being attempted, the skill check is a failure and the Specialist must abandon it or start over from scratch. Failure may also cause damage to any materials and/or tools being used.

If all dice rolled for any check are 1, the check is considered a catastrophic failure, meaning the skill check must be abandoned or restarted, just as if they'd failed a number of checks equal to the degree of skill being attempted. For example, a Specialist using master Diplomacy skill who suffers a catastrophic failure would automatically lose 50 points of disposition with the intended subject, rather than having to roll 5d10 to determine the loss.

Conversely, if all dice rolled for any check are 10, the check is considered to be a spectacular success, meaning the skill attempt is completed and any variables based on skill usage are maximized. For example, a Specialist using master Diplomacy skill who scores a spectacular success would automatically increase the disposition of the intended subject by a full 50 points, rather than having to roll 5d10 to determine their gain.

 When a skill check is attempted in favorable or unfavorable conditions, the Keeper may need to adjust the roll required for success or failure. In favorable to extremely favorable conditions, the Keeper should roll 1d10, 2d10 or 3d10 and subtract the total result from the normal success and failure numbers. For example, if a Specialist is making an intermediate check in favorable conditions, the Keeper may roll 1d10. If they roll a 3, they would subtract 3 from 26, for a result of 23 for the minimum roll needed to succeed on the check. The Keeper would also subtract the number from the failure roll of 12, for a result of 9 or less. Conversely, if conditions are unfavorable to extremely unfavorable, the Keeper would roll 1d10, 2d10 or 3d10 and add their roll to the success and failure numbers, thus increasing the difficulty of the skill check.

Some skills are used to create objects, such as a lock, which may be subject to further skill checks, such as a lock picking check. The skill checks of such objects have a minimum roll to succeed equal to, or greater than, the quality of the object. For example, if a Specialist makes a master level lock with a quality of 70, another Specialist would need to roll at least a 70 on their lock picking check to pick the lock.

### Untrained Skill Checks
> **Status:** ⚠️ REVIEW / CONVERSION — the concept may survive, but the legacy summed-die thresholds and any fixed numerical resolution must be converted to the current success-counting engine.

Specialists may attempt to use skills untrained. Doing so is difficult, however. To attempt an untrained skill check, the Specialist's relevant governing score must meet or exceed the minimum requirement to train in the attempted degree of the skill. When attempting to use a skill degree in which the Specialist is untrained, a Specialist only rolls half their skill dice (minimum 1) on the check. Furthermore, a Specialist can never attempt an untrained skill degree meticulously. Failure on an untrained skill always results in disaster.

### Hasty Skill Check
> **Status:** ⚠️ REVIEW / CONVERSION — the concept may survive, but the legacy summed-die thresholds and any fixed numerical resolution must be converted to the current success-counting engine.

A Specialist attempting to use a skill hastily does so at increased risk of failing and breaking or destroying materials and/or equipment. A hasty skill check is made in half the time, however the Specialist uses one fewer skill dice for the roll. Not all skills may be attempted hastily, and are notated as such. Normally a Specialist attempting to make a sword using the Weapon smith skill would work in 8 hour increments and require a total of 2 success rolls. The same Specialist attempting to make the sword hastily would work in 4 hour increments, still require 2 success rolls and would additionally take a 1d10 penalty on all skill check rolls.


Progressive/Productive Skill Check

Progressive or productive skill checks require a Specialist to make skill checks at certain intervals, as listed in the skill description. The minimum result required to succeed is 7 for simple, 16 for basic, 27 for intermediate, 40 for advanced and 55 for master. A failure is a roll of 1 for simple, 4 or less for basic, 9 or less for intermediate, 16 or less for advanced, and 25 or less for master. Any roll that is neither a success nor a failure simply represents no meaningful progress. To complete the skill use, the Specialist must accumulate a number of successes inversely proportional to the degree of the skill being used, or 5 for simple, 4 for basic, 3 for intermediate and so on. If, at any time, the number of failures is greater than the number of successes, the entire skill check is failed, and results in damaging tools and/or loss of materials as appropriate.

### Ongoing Skill Check
> **Status:** ⚠️ REVIEW / CONVERSION — the concept may survive, but the legacy summed-die thresholds and any fixed numerical resolution must be converted to the current success-counting engine.

A Specialist using a skill that is relatively easy to perform, or that goes on for long periods of time, such as riding a horse or rowing a boat may be performing an ongoing skill check, as determined by the Keeper. Ongoing skill checks are only checked every so often, or not at all if the Keeper deems their skill level sufficient to maintain the skill with little effort given present circumstances. An ongoing skill may, without warning, become a regular skill check if conditions change in such a way that would increase the difficulty of the skill, such as an ambush while riding a horse.

### Meticulous Skill Check
> **Status:** ⚠️ REVIEW / CONVERSION — the concept may survive, but the legacy summed-die thresholds and any fixed numerical resolution must be converted to the current success-counting engine.

Under the right circumstances, a Specialist may be meticulous in the use of a skill. A Specialist using a skill meticulously doubles or quadruples the amount of time they devote to the skill. Doubling the time gives the Specialist an additional 1d10 to their skill check roll. Quadrupling the time gives the specialist an additional, cumulative 2d10 (for a total of 3d10) to their skill check roll. Furthermore, quadrupling the time negates normal failures, but not catastrophic failures.

### Skills in Combat
> **Status:** ⚠️ REVIEW / CONVERSION — the concept may survive, but the legacy summed-die thresholds and any fixed numerical resolution must be converted to the current success-counting engine.

Using skills in combat costs AP. For each needed skill check, a Specialist must spend 1 AP. If a skill requires more skill checks than a Specialist has AP in a single round of combat, the Specialist may not use that skill in combat. Only skills that have immediate results or may be attempted hastily may be used in combat, subject to the Keeper's approval.

# Skill Descriptions

The following is a list of skills divided into categories based on their governing Specialist stat. Each skill features a general description and a list of simple, basic, intermediate, advanced and master level actions they allow a Specialist to perform. This list is merely a guideline, and it is ultimately between the Keeper and the player as to whether or not a Specialist would be able to perform a particular task using their skills.

## Speed

### Explosives:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with Explosives skill are able to work with volatile substances more safely and efficiently than those without. This skill enables users to create, modify, disable or bypass explosive devices of various types and strengths. Creatures caught inside the blast are treated as being automatically hit by the blast, but damage may still be mitigated as normal.

Specialists with simple training in explosives are able to work with fuse and powder based explosive devices, such as cannons, dynamite and grenades. Dynamite and grenades created using this skill deal 1d10 damage in a radius of 3 movement units appropriately sized for the creator when used in combat.

Basic training in explosives allows a Specialist to precisely time explosions with fuse and powder based explosives, as well as the ability to create water proof fuses. Additionally, this allows the use of simple and basic applications of this skill in conjunction with the trap-making skill.


Intermediate training in explosives affords a Specialist the ability to work with liquid and solid chemical reactions to produce explosive devices. Explosives made with the intermediate degree of training deal 3d10 damage in a 5 movement unit radius appropriately sized for the caster when used in combat.

Advanced training in explosives renders a Specialist able to create shaped charge blasts, as well as precisely time any explosion. The blast may be in a circle with a radius of up to 5 movement units, emanating from the explosive device or may be shaped. Shaped blasts may be any continuous portion of a circle, for example a 270 degree arc or 45 or 90 degree cone. The blast may also be in a line from the device with a maximum range of 10 movement units. The blast area may be positioned independently of the device, so long as the device remains within the blast area, subject to Keeper approval.

With master training in explosives, a Specialist is able to sense explosive devices via minute signs, such as the smell of particular chemicals and explosive components. This also allows Specialists to identify chemicals and substances that can be made into explosives. Explosives made with master degree skill deal 10d10 damage in a radius of up to 10 movement unit radius appropriately sized for the creator when used in combat. Finally, this allows all applications of this skill to be used in conjunction with the trap-making skill.

### Fishing:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with Fishing skill gain knowledge of techniques used to catch aquatic wildlife.

Specialists with simple degree training are able to use basic tools for catching fish and other aquatic life, including basic fishing poles, hooks, lures, bait, and nets.

Basic training grants a Specialist the ability to use improvised tools to simulate those listed in simple fishing.

Intermediate training allows a Specialist to create lures and baits to attract various aquatic wildlife.

Advanced training gives a Specialist understanding of how to quickly identify the most probable places to catch specific types of aquatic wildlife.

Master training enables a Specialist to create targeted baits to attract specific types of aquatic wildlife.

### Hunting:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with Hunting skill gain an understanding of the psychology of wild game, as well as the ability to use specialized tools and weapons to aid in catching them.

Simple training allows a Specialist to capture or kill up to medium sized game using weapons such as spears, bow and arrows, or nets. They are also able to set capture or kill traps, dependent upon possession of appropriate trap-making skill ranks. Some wild game requires combat in order to hunt with weapons, such as spears or bow and arrows. In such a case, a Specialist still needs martial training in the weapons to avoid taking the penalties for using them untrained in combat. For smaller game where no combat is required, the Specialist may use the aforementioned weapons without penalty, subject to Keeper approval. For example, a Specialist could shoot a rabbit with an arrow without combat training, but would merely anger a bear without proper martial training.

A Specialist with basic hunting training is able to employ visual camouflage such as duck blinds or camouflage nets to prevent potential prey from seeing them. Such camouflage is not suitable for combat or for hiding from intelligent creatures.

Intermediate training grants a Specialist the know-how to capture or kill up to large sized game in the same manner as simple degree hunting skill.

Specialist with advanced training know how to use musks and perfumes to mask their own scent to prevent potential prey from smelling them.

Master degree hunting training enables Specialists to capture or kill any size game with appropriate checks. Note that some prey may require battle to fell, as determined by the Keeper.

### Listening:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Listening skill are increasingly able to tune out background noise, and hone in on specific sound sources, as well as pick up on very quiet sounds.

Simple degree training lets the Specialist passively scan for abnormal sounds. Specialists with this skill are allowed to make a listen check whenever there’s a potential for them to hear something out of the ordinary. When appropriate, the Keeper should roll for the player on this skill, to avoid tipping off those that fail the check that there was something to be heard.

Specialists with basic degree training are able to listen through physical barriers, such as doors, windows and walls.

Intermediate training allows a Specialist to interpret vocal and environmental sounds to glean certain information, such as the relative size of a creature based on the volume of its call, or the direction of a snapping twig.

Advanced training gives the Specialist the ability to reflexively filter sounds, such as explosions, to prevent potential hearing loss.

Master training enables the Specialist to focus on a specific source of sound, and tune out all other sources in any environment.

### Pick pocket:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Pick pocket skill are able to use their nimble fingers to pilfer objects from others without their knowledge.

Simple pick pocket training allows a Specialist to attempt to remove an object no larger than can be easily concealed within one’s hand from sleeping creatures without waking them.

A Specialist with basic pick pocket training may attempt to remove any object from a sleeping creature without waking them.

Intermediate training grants a Specialist the ability remove an object no larger than can easily be concealed within one’s hand from conscious creatures without their knowledge. The Specialist may only attempt to remove passively placed (not worn or held) objects.

Specialists with advanced training may attempt to employ misdirection to remove larger objects from creatures without their knowledge. They may only attempt to remove passively placed (not worn or held) objects.

Master degree training allows a Specialist to attempt to remove any object, including worn or held objects, from conscious creatures without their knowledge. Furthermore, they may place objects on such creatures without their knowledge.

### Spot:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Spot skill are able to notice things out of the ordinary.

With simple training, a Specialist is able to notice things that are obviously out of place or that contrast with their environment, such as a campfire, or a dingy white brick among clean white bricks with a quick search.

Basic training enables a searching Specialist to notice things that are less obviously out of place, such as a board made of a different type of wood, or a crack in a brick.

Intermediate training allows a Specialist to passively notice things that must actively be searched for with simple degree spot training.

Advanced degree training gives a Specialist the ability to passively notice things that must actively be searched for with basic degree spot training.

Finally, master training lets a Specialist find minute details out of place, such as a smooth spot on a stone where it has been pressed or rubbed, or the very slight bleaching where a page of a book has been open longer than others.

## Proficiency

### Bowyer:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Bowyer skill are able to maintain, construct and modify bows and crossbows.

Simple: Able to assemble (string) and maintain bows.

Basic: Able to assemble (string) and maintain crossbows.

Intermediate: Able to repair damage to bows.

Advanced: Able to repair damage to crossbows.

Master: Able to improve and reinforce bows and crossbows.

### Calligraphy:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Calligraphy skill are able to read and write official and royal documents in any language in which they are fluent.

Simple: Able to read official writs, and royal decrees.

Basic: Able to write with basic, albeit somewhat sloppy and often illegible, handwriting.

Intermediate: Able to write with better handwriting, with far fewer mistakes.

Advanced: Able to write legible handwriting with no mistakes.

Master: Able to write passable official and royal documents.

### Carpentry:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Carpentry skill are able to use various woodworking tools to construct objects, primarily out of wood.

Simple: Able to cut, smooth, and assemble misshapen, rickety, uncomfortable furniture. Simple furniture often tends to be shoddy, and breaks if used for anything other than its intended purpose (and sometimes when used for its intended purpose).

Basic: Able to more adequately assemble basic, though still ugly and uncomfortable furniture. Furniture made with the basic skill is more sturdy, and has to be intentionally abused (or greatly overused) to break.

Intermediate: Able to make smooth, polished, attractive furniture. Only excessive abuse breaks this furniture.

Advanced: Able to work with lumber to fashion buildings in addition to furniture.

Master: Able to make mechanisms out of wood, such as gears and pulleys, or even extremely basic automatons and clockworks.

### Cartography:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Cartography skill are able to read, understand, draw, mark, and encrypt maps.

Simple: Able to interpret simple maps.

Basic: Able to interpret basic maps, such as topographical. Able to interpret symbols with reasonable accuracy.

Intermediate: Able to draw simple maps with relative accuracy.

Advanced: Able to draw topographical maps, and devise map legends to assist in understanding.

Master: Able to encrypt maps with vague information about specific locations.

### Counterfeiting:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Counterfeiting skill are able to make passable facsimiles of increasingly rare objects. These objects appear to be the real thing to untrained eyes, and casual observers, but don’t hold up under any sort of scrutiny. If the counterfeiter doesn’t possess the requisite skill to make the base object, such as sewing for counterfeit clothing, they may still purchase a similar object and make modifications to it.

Simple: Able to make simple counterfeit objects, such as replicas of tokens.

Basic: Able to make basic counterfeit objects, such as designer clothing.

Intermediate: Able to make intermediate counterfeit objects, such as fake jewelry.

Advanced: Able to make advanced counterfeit objects, such as non-functioning replicas of machines and devices.

Master: Able to make masterful counterfeit objects, such as visually convincing replicas of Qwartz. It should be noted that any interaction with the Qwartz gives it away as a counterfeit, due to the obvious lack of magical properties.

### Disable device:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Disable device skill are able to modify the workings of machines and other devices.

Simple: Able to stop devices from fulfilling their intended functions (namely by breaking them).

Basic:  Able to stop devices from fulfilling their intended functions without breaking them.

Intermediate: Able to bypass, or temporarily prevent devices from fulfilling their intended functions. Objects bypassed are bypassed indefinitely, generally by stopping gears, or otherwise halting some type of process. There is a chance that bypassed devices will break, as determined by the Keeper.

Advanced: Able to bypass devices without breaking them. Furthermore, devices may be bypassed with crude timers, to allow the device to resume their functions after a roughly determined period of time, specified in seconds, minutes, hours, days, etc.

Master: Able to change how a device functions.

### Escape:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Escape skill are able to abscond from various forms of capture, detainment, and imprisonment.

Simple: Able to wriggle or break free of personal restraints, such as a creature attempting to hold your wrists, or a bear hug.

Basic: Able to wriggle free of ropes and other crude forms of restraint.

Intermediate: Able to slip out of basic manacles.

Advanced: Able to slip out of full shackles.

Master: Able to squeeze between bars, climb out of nets, or otherwise get out of advanced restraints.

### Fletching:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Fletching skill are able to maintain, assemble and modify arrows and bolts.

Simple: Able to maintain regular arrows and darts.

Basic: Able to maintain regular bolts.

Intermediate: Able to assemble arrows and darts from arrowheads/dart tips, shafts and various fletching (flights).

Advanced: Able to assemble bolts from bolt heads, shafts and various fletching (flights).

Master: Able to craft special purpose, such as flame, acid vial or poison vial tipped arrows, darts and bolts.

### Herbology:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Herbology skill can determine whether plants are edible, beneficial, benign, or toxic. Note: While the properties of plants may be determined through use of the Herbology skill, the Alchemy or Apothecary skill is required to utilize any properties resembling magic.

Simple: Able to determine the properties of plants in the region in which you’ve spent most of your life (plants you’re familiar with).

Basic: Able to determine the properties of unfamiliar plants through basic experimentation (though sometimes this can be dangerous, such as when dealing with highly toxic plants).

Intermediate: Able to determine the properties of plants through more elaborate, though somewhat safer experiments.

Advanced: Able to determine the properties of plants through advanced and completely safe experiments.

Master: Able to determine the properties of plants using the basic senses of sight, smell, taste, and touch.

### Jeweler:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Jeweler skill are able to work with rare metals and precious stones to create decorative and salable jewelry.

Simple: Able to work with malleable metals to form basic adornments, such as rings and bracelets.

Basic: Able to work with appropriate tools to form more intricate types of jewelry, such as links for necklaces.

Intermediate: Able to set cut stones into receptacles built into metals.

Advanced: Able to facet raw jewels and gems for placing into jewelry.

Master: Able to make extremely intricate designs, add filigree, emboss, etch, and otherwise refine high end jewelry.

### Leatherworking:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Leatherworking ability are able to refine and shape leather into various supple leather garments, with the exception of Leather armor (as leather armor requires the Leather armoring skill).

Simple: Able to remove the entire hide or skin from a creature.

Basic: Able to sew leather together to make uncomfortable leather garments.

Intermediate: Able to shape leather into more comfortable garments.

Advanced: Able to refine leather to make it more supple and smooth.

Master: Able to sew and shape leather into any reasonable shape (assuming enough material is available), such as clothing, sails, saddles, etc.

### Lock picking:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Lock Picking skill are able to use tools to bypass various locks.

Simple: Able to pick simple locks.

Basic: Able to pick basic locks.

Intermediate: Able to pick intermediate locks.

Advanced: Able to pick advanced locks.

Master: Able to pick (you guessed it) master locks. Additionally, able to produce makeshift tools to use. May also attempt to pick magical locks without the use of magic.

### Musical instrument (specified):
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Musical Instrument skill are able to play a selected instrument in a variety of ways.

Simple: Able to play individual notes (or simple chords on stringed instruments).

Basic: Able to play an instrument from sheet music with relative accuracy.

Intermediate: Able to play recognizable songs, start to finish with or without sheet music.

Advanced: Able to compose songs.

Master: Able to perform songs free-form, and make it up as you go.

### Poisons:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Poisons skill are able to harvest or extract and safely work with poisons.

Simple: Able to employ proper safety equipment for dealing with plant-based toxins.

Basic: Able to expose yourself to controlled doses of plant-based toxins, in order to build up a resistance. This process is dangerous, and potentially fatal, as determined by the Keeper.

Intermediate: Able to employ proper equipment for safety and harvesting or extracting animal-based toxins.

Advanced: Able to expose yourself to controlled doses of animal-based toxins, in order to build up a resistance. This process is dangerous, and potentially fatal, as determined by the Keeper.

Master: Able to refine and distill toxins from plants and animals, to increase potency. Also, potentially able to resist any toxin, assuming you’ve gone through the process of building up resistances to several types of toxins, as determined by the Keeper.

### Rope use:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Rope use skill are able to perform a variety of tasks and tricks using ropes.

Simple: Able to tie simple knots, and untangle long lengths of rope.

Basic: Able to devise basic pulley systems and tie basic knots (such as a slip-knot), and use ropes for rappelling.

Intermediate: Able to tie intermediate knots and use ropes for climbing.

Advanced: Able to tie advanced knots and lasso creatures and objects.

Master: Able to tie master knots, and build nets.

### Scribe:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Scribe skill are able to keep records of events, and copy tomes.

Simple: Able to hastily scrawl roughly legible accounts of events as they occur.

Basic: Able to record events more legibly as they occur.

Intermediate: Able to accurately take dictation.

Advanced: Able to copy lengthy tomes from any language known by the Specialist into any other language also known by the Specialist.

Master: Able to make exact duplicates of writings and drawings.

### Sewing:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Sewing skill are able to use needle, thread and other tools to stitch, mend and fashion items out of cloth.

Simple: Able to weave threads into cloth.

Basic: Able to make basic clothing patterns, and sew basic garments.

Intermediate: Able to design unique clothing patterns, and sew together comfortable garments.

Advanced: Able to work with fine fabrics and sew luxurious garments.

Master: Able to weave fine fabrics and design royal garments.

### Sleight of hand:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Sleight of hand skill are able to use misdirection and quick fingers to entertain or steal.

Simple: Able to palm miniscule objects, which can completely fit in one’s hand.

Basic: Able to hide miniscule objects in such a way that onlookers don’t notice.

Intermediate: Able to use misdirection to quickly hide or reveal handheld objects no larger than a fist.

Advanced: Able to use misdirection to quickly hide or reveal moderately sized objects, no larger than one’s torso.

Master: Able to use misdirection to quickly hide or reveal large objects.

### Trap making:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Trap making skill are able to make various types of traps to catch or kill creatures.

Simple: Able to construct simple snare traps.

Basic: Able to construct basic weighted cage traps.

Intermediate: Able to create spring-loaded traps, such as bear traps.

Advanced: Able to create complex, difficult to detect traps.

Master: Able to incorporate any spell, attack type or other skill known into traps.

### Wood carving:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Wood carving skill are able to shape pieces of wood and lumber into tools and sculptures.

Simple: Able to whittle simple tools and sculptures, such as a pointy stick, or an axe handle.

Basic: Able to whittle basic tools and sculptures, such as wooden statues, or a whistle.

Intermediate: Able to use various wood working tools to carve intricate tools and sculptures, such as a flute, or a jewelry box.

Advanced: Able to carve intricate patterns into wood, or create complex wooden sculptures, such as a wooden chain, or a ball in a cage carved from a single piece of wood.

Master: Able to carve detailed and realistic sculptures.

### Writing:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Writing skill are able to recount, embellish and fabricate stories.

Simple: Able to recount the most important details of recent events.

Basic: Able to recount the most important details of more distant events.

Intermediate: Able to recount events with vivid clarity, or write fantastical fabrications.

Advanced: Able to write believable fabrications as though they were actual events.

Master: Stephen King. ‘Nuff said.

## Charisma

### Acting:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Acting skill are able to put on performances with appropriate tone of voice and emotion.

Simple: Able to rehearse a script, and recall lines with minimal prompting.

Basic: Able to rehearse and recall lines with no prompting.

Intermediate: Able to add generally appropriate emotion to scenes.

Advanced: Able to add appropriate emotion to scenes.

Master: Able to adlib, and perform believably on the fly.

### Bluff:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Bluff skill are able to convince others of things that aren’t true.

Simple: Able to convince others that minor details are or were different than reality.

Basic: Able to convince others of slightly harder to swallow fallacies.

Intermediate:  Poker face.

Advanced: Able to distract opponents in combat, possibly tricking them into lowering their defenses.

Master: Able to convince others that completely outrageous ideas are the truth.

### Diplomacy:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Diplomacy skill are able to use proper etiquette and protocol when dealing with others, including leaders and foreign cultures.

Simple: Able to show proper respect to obvious upper class citizens.

Basic: Able to recognize slightly less conspicuous members of the upper class and nobility.

Intermediate: Able to observe and quickly fit into foreign and unfamiliar customs.

Advanced: Able to recognize dignitaries attempting to remain incognito.

Master: Able to mediate for royalty, and follow proper etiquette even in unfamiliar cultures.

### Interrogation:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Interrogation skill are able to employ various means to gather information from those who would rather not divulge it.

Simple: Able to interpret voice inflections from captives.

Basic: Able to make subjects uncomfortable while attempting to elicit information.

Intermediate: Able to read body language to better understand how to more easily loosen a subject’s tongue.

Advanced: Able to interpret a subject’s body language to discern when a subject is lying.

Master: Able to form a bond with a subject, and convince them to willingly divulge information.

### Intimidate:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Intimidate skill are able to make themselves seem to be a great threat, whether it’s true or not.

Simple: Able to frighten children and small animals.

Basic: Able to frighten elderly and invalids.

Intermediate: Able to frighten rookie soldiers and inexperienced town guards.

Advanced: Able to frighten veteran soldiers and town guards.

Master: Able to frighten beasts and seasoned warriors.

### Leadership:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Leadership skill are able to inspire others to follow them.

Simple: Able to gather a small following of like-minded individuals.

Basic: Able to gather additional like-minded individuals.

Intermediate: Able to rally many like-minded individuals to a cause.

Advanced: Able to persuade and inspire large groups.

Master: Able to command the loyalty of an entire kingdom.

### Merchant:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Merchant skill are able to barter goods and services for the best price.

Simple: Able to recognize bargains.

Basic: Able to maintain a vending stall to sell various goods.

Intermediate: Able to barter and exchange goods for similarly valuable goods.

Advanced: Able to convince potential customers that an object is more valuable than it is.

Master: Used carriage salesman.

### Mimicry:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Mimicry skill are able to copy the actions and sounds of others.

Simple: Able to copy another’s inflection.

Basic: Able to modulate your pitch to sound like another of the same gender.

Intermediate: Able to modulate your pitch to sound like somebody of either gender.

Advanced: Able to mimic physical actions and gestures typical of another individual.

Master: Able to believably portray another individual for any length of time.

### Public speaking:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Public speaking skill are able to draw in crowds of people and present them with information, and possibly rally them to a cause.

Simple: Able to stand in front of a crowd, and read from a script.

Basic: Able to stand in front of a crowd, and present information from notes.

Intermediate: Able to engage an audience, and present information in an understandable and entertaining way.

Advanced: Able to interact with a crowd and generate interest in information.

Master: Able to enthrall and entertain large audiences in the presentation of information.

### Singing:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Singing skill are able to modulate their voices into pleasant and melodic tones, often with lyrics.

Simple: Able to hum, and sing simple nursery rhymes.

Basic: Able to sing from sheet music with relative accuracy.

Intermediate: Able to sing recognizable songs, start to finish with or without sheet music.

Advanced: Able to compose songs.

Master: Able to sing free-form, and make it up as you go.

### Torture:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Torture skill are able to torment captives physically or psychologically.

Simple: Able to employ methods of inflicting physical pain with only a moderate mortality rate.

Basic: Able to inflict physical pain with only a low mortality rate.

Intermediate: Able to inflict physical pain with no mortality rate.

Advanced: Able to torment captives emotionally.

Master: Able to inflict emotional and mental anguish on captives.

## Intelligence

### Administration:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Administration skill are able to keep track of numerous individuals, and their tasks, to accomplish desired goals.

Simple: Able to coordinate the efforts of up to 3 individuals to achieve a desired short-term (a few days) goal.

Basic: Able to coordinate the efforts of up to 10 individuals to achieve a desired short-term (up to a week) goal.

Intermediate: Able to coordinate up the efforts of up to 20 people to achieve a desired medium length (up to a month) goal.

Advanced: Able to coordinate the efforts of any number of people to achieve a desired medium length (up to 3 months) goal.

Master: Able to coordinate the efforts of several groups to achieve a desired goal over any length of time.

### Alchemy:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Alchemy skill are able to combine various ingredients to produce effects which often seem, and sometimes are, magical.

Simple: Able to document effects produced in nature by various creatures, plants and objects.

Basic: Able to mix chemicals in such a way as to mimic basic effects produced by creatures, plants and objects.

Intermediate: Able to harvest and preserve unusual substances from creatures, plants and objects.

Advanced: Able to temporarily change the chemical makeup of chemicals and objects.

Master: Able to produce effects similar to those produced by spells through mixtures and applications of various chemicals.

### Apothecary:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Apothecary skill are able to combine various mundane ingredients into salves, poisons, tonics, and potions.

Simple: Able to mix various roots and plants into pastes and salves to help treat minor wounds and soothe pain.

Basic: Able to mix ingredients into minor toxins and pain killers in paste, salve, or liquid form.

Intermediate: Able to form ingredients into powder form.

Advanced: Able to make numbing agents. Also, able to make pills from any recipe they have.

Master: Able to mix very potent pain killers, toxins, and even healing potions.

### Appraise:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Appraise skill are able to determine the monetary value of goods or services.

Simple: Able to discern the price and value of mundane trade goods.

Basic: Able to discern the value of jewels and gems.

Intermediate: Able to assess the value of art.

Advanced: Able to determine equivalent exchange rates of various forms of currency.

Master: Able to determine the value of obscure, unique, and ancient objects.

### Architecture:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Architecture skill are able to draft designs for buildings.

Simple: Able to sketch building concepts.

Basic: Able to find level ground on which to build, and incorporate landscape into building design.

Intermediate: Able to find areas near natural resources in which to build.

Advanced: Able to incorporate any landscape, such as the placing a building within the branches of a large tree, into designs.

Master: Able to draw multi-plane, fully detailed plans for buildings.

### Camping:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Camping skill are able to set up and tear down campsites, and use the environment to enhance the comfort of themselves and others.

Simple: Able to locate and gather various types of wood suitable to build and sustain a camp fire.

Basic: Able to pitch a tent.

Intermediate: Able to store foods and other consumables out of the reach of wildlife.

Advanced: Able to find the most comfortable positions in which to sleep.

Master: Able to build shelters from whatever nature provides, and find the safest places to sleep.

### Chemistry:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Chemistry skill are able to work with various chemicals and substances to create different effects.

Simple: Able to mix and document experimentations with various chemicals.

Basic: Able to refine chemical compounds.

Intermediate: Able to cross-reference chemical reactions and accurately predict reactions of chemicals.

Advanced: Able to readily identify common chemicals.

Master: Able to identify the properties (caustic, toxic, flammable, etc.) through use of the senses and/or application of scientific method.

### Cryptography:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Cryptography are able to encrypt and decipher messages and unknown languages.

Simple: Able to interpret coded messages through use of the keys.

Basic: Able to create keys and use them to encode messages.

Intermediate: Able to interpret coded messages with generic keys, or through trial and error.

Advanced: Able to decode messages without any key.

Master: Able to decipher complex characters and documents in unknown languages.

### Education:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Education skill are able to teach others skills they have, up to and including, but not exceeding their current skill level. Note: Students being trained still only learn the skills being taught by purchasing skill ranks and applying the appropriate skill training points toward the skill.

Simple: Able to teach another up to simple techniques of any skill you possess.

Basic: Able to teach another up to basic techniques of any skill you possess.

Intermediate: Able to teach another up to intermediate techniques of any skill you possess.

Advanced: Able to teach another up to advanced techniques of any skill you possess.

Master: Able to teach another any techniques of any skill you possess.

### Engineering:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Engineering skill are able to build machines and devices with complex inner workings, such as clockworks and automatons.

Simple: Able to take apart simple devices which run on gears and springs.

Basic: Able to reassemble simple devices which run on gears and springs.

Intermediate: Able to take apart intermediate devices which run on gears and springs.

Advanced: Able to reassemble intermediate devices which run on gears and springs.

Master: Able to design and construct new devices which run on gears and springs.

### Finance:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Finance skill are able to track cash flow, and budget money accordingly.

Simple: Able to track and predict weekly and monthly expenditures for a given business.

Basic: Able to estimate weekly and monthly income for a given business.

Intermediate: Able to anticipate and budget money for a business through various seasons and events.

Advanced: Able to track and estimate weekly and monthly expenditures for multiple businesses.

Master: Able to budget money for multiple businesses.

### Geography:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Geography skill are able to determine information about their surroundings based on the environment.

Simple: Able to discern obvious visual cues to glean information about your environment, such as thriving vegetation tends to exist where there’s a source of water.

Basic: Able to discern visual cues to glean information about your environment, such as the difference between dead vegetation and simply dry vegetation, in order to point the direction to water.

Intermediate: Able to interpret visual cues to find likely sources of edible vegetation.

Advanced: Able to discern the direction of the nearest fertile soil based on visual cues.

Master: Able to glean the most likely direction of water, vegetation, fertile soil, etc. with or without visual cues.

### Geology:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Geology skill are able to identify various types of earth and stone, and can understand their history based on their composition.

Simple: Able to identify basic types of stone, such as granite and marble.

Basic: Able to identify uncommon and obscure types of stone, such as limestone or pyrite.

Intermediate: Able to read core samples or areas of exposed layers to determine changes which have occurred in the land over several centuries or millennia.

Advanced: Able to locate veins of metal ores based on stone and earth formations.

Master: Able to locate likely areas to mine raw gems based on stone and earth formations.

### Heraldry:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Heraldry skill are able to identify royal and noble houses based on their crests. They’re also familiar with the history and nature of said families.

Simple: Able to identify the crests of current royal houses.

Basic: Able to identify the crests of current noble houses.

Intermediate: Familiar with the history of current and past noble and royal houses.

Advanced: Familiar with the nature of current and past noble and royal houses.

Master: Able to appeal to the nature of nobles and royals in proper form, due to your thorough understanding of the house.

### History:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the History skill are able to recall or quickly research events that have taken place in the past.

Simple: Able to recount, with moderate accuracy, recent events of the areas you’ve been in.

Basic: Able to accurately recount events of the last several years in the areas you’ve been, and outlying areas.

Intermediate: Able to quickly research history revolving around a specific item or event with moderate accuracy.

Advanced: Able to quickly and precisely research history revolving around a specific item or event.

Master: Able to potentially recall specific historical information without ever specifically having read it.

### Law:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Law skill are familiar with the legal structure of any region whose law they’ve studied, and can be advocates in defense or opposition of those accused of crimes.

Simple: Able to laboriously research laws of a land to defend or prosecute a suspect in a court of law.

Basic: Able to quickly research the laws of a land to defend or prosecute a suspect in a court of law.

Intermediate: Able to make reasonable assumptions about laws of an area based on behaviors of individuals.

Advanced: Able to focus or obscure suspicion on a particular suspect, using circumstantial evidence, or emotional appeal.

Master: Able to find appropriate and potentially obscure loopholes in the laws of an area.

### Local geography (specified):
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Local Geography skill are familiar with a particular region and its available resources.

Simple: Able to find or give directions to major areas of interest, such as farms, towns, streams, etc. in the area this skill pertains to.

Basic: Able to locate or give directions to moderate areas of interest, such as a particular business or landmark in the area this skill pertains to.

Intermediate: Able to locate or give directions to uncommon or hidden areas of interest, such as an abandoned mineshaft, or a cave behind a waterfall in the area this skill pertains to.

Advanced: Able to locate or give directions to minute and obscure places, such as a burnt oak tree, or a solitary daisy, within the area this skill pertains to.

Master: I know the ship like the back of my hand.

### Mathematics:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Mathematics skill are able to perform calculations of varying degrees.

Simple: Able to add and subtract.

Basic: Able to multiply and divide.

Intermediate: Able to solve complex equations for variables.

Advanced: PEMDAS, geometry.

Master: Calculus, linear algebra.

### Metallurgy:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Metallurgy skill are familiar with the composition of various metals, and can combine them into alloys.

Simple: Familiar with the compositions of basic metals and ores, such as iron and copper.

Basic: Able to smelt and refine basic metals and ores to remove impurities, and thereby strengthen them.

Intermediate: Familiar with rarer metals and ores, such as gold and silver.

Advanced: Able to smelt and refine rarer metals and ores.

Master: Able to combine metals into alloys, such as bronze and steel.

### Navigation:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Navigation skill are able to recognize landmarks and determine direction based on available input, such as the position of the sun or the stars.

Simple: Able to recognize popular landmarks and references to them on maps.

Basic: Able to find uncommon landmarks and references to them on maps.

Intermediate: Able to use the sun’s position to determine direction.

Advanced: Able to use stars and constellations to determine direction.

Master: Able to maintain a course based on minimal input, such as wind direction, accounting for shifts in wind direction and speed, even on overcast nights where stars aren’t visible.

### Researching:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Researching skill are able to find and cross-reference information.

Simple: Able to find books which directly reference a particular subject, such as a book entitled Noble Houses when researching noble houses.

Basic: Able to find books which indirectly reference a particular subject, such as a book entitled A Tea Party at Sir Walter’s when researching noble houses.

Intermediate: Able to find books which don’t even indirectly reference a subject, but are close enough to the topic at hand to potentially provide information, such as a book entitled Wondrous Gardens when researching noble houses.

Advanced: Able to find books with encoded messages about particular topics.

Master: Able to decrypt encoded volumes, and cross-reference obscure tomes to glean information about a particular subject.

### Smuggling:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Smuggling skill are able to hide and transport potentially contraband objects and creatures.

Simple: Able to nonchalantly carry very small objects into or out of areas. Objects are easily found by a search.

Basic: Able to nonchalantly carry small to moderate sized objects into or out of areas. Objects are found by a search with some effort.

Intermediate: Able to hide large objects or people within larger objects and sneak them past security. Objects are discovered by rigorous searching.

Advanced: Able to sneak huge objects or people nearly in plain sight. Objects are detected by rigorous searching.

Master: Able to sneak nearly anyone or anything past nearly anybody. Only the closest and most strenuous searches reveal them. “These are not the automatons you’re looking for.”

### Strategy:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Strategy skill are able to formulate plans of attack based on information about enemies.

Simple: Able to track and operate one unit in battle.

Basic: Able to track and operate several units of one type in battle, i.e. archers or infantry, but not both.

Intermediate: Able to track and operate several units of varied type in battle.

Advanced: Able to formulate advanced tactics based on unit strengths and weaknesses of friendly and opposing forces.

Master: Able to plan decisive combat tactics for entire armies consisting of numerous and varied units and battalions.

## Agility

### Acrobatics:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Acrobatics skill are able to leap, duck, dive, tuck, roll, flip and otherwise perform impressive feats of agility.

Simple: Able to perform cartwheels and handsprings.

Basic: Able to perform front flips and rolls.

Intermediate: Able to perform single backflips and dives.

Advanced: Able to perform continuous backflips and handstands.

Master: Olympic gymnast.

### Aquabatics:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Aquabatics skill are able to move nimbly and gracefully, and perform tricks in water.

Simple: Able to perform cartwheels and handsprings under water.

Basic: Able to perform front flips and rolls under water.

Intermediate: Able to perform single backflips and dives under water.

Advanced: Able to perform continuous backflips and handstands under water.

Master: Olympic gymnast under water.

### Balance:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Balance skill are able to position and distribute their weight and the weight of their possessions to help prevent falling on or from narrow surfaces.

Simple: Able to walk or stand on objects or paths an inch or two narrower than the width of your shoulders in a normal stance.

Basic: Able to stand on objects as narrow as your foot.

Intermediate: Able to walk on objects as narrow as your foot.

Advanced: Able to walk or stand on objects as narrow as your thumb.

Master: Able to stand or walk on the edge of a blade (with proper protection from it), or a thread (if it will support your weight).

### Dancing:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Dancing skill are able to gracefully twirl and glide about with or without a dance partner.

Simple: Able to follow simple, specified, measured dance steps without a partner.

Basic: Able to follow simple, specified, measured dance steps with a properly trained partner.

Intermediate: Able to string together varied dance moves without a partner.

Advanced: Able to string together varied dance moves with a partner.

Master: Able to lead an untrained partner in varied and even spontaneous dance moves.

### Hiding:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Hiding skill are able to conceal themselves in their surroundings.

Simple: Able to hide behind huge objects.

Basic: Able to blend in with surroundings colored similar to your clothing.

Intermediate: Able hide behind objects slightly smaller than yourself.

Advanced: Able to blend in with surroundings of moderately different color than your clothing.

Master: Able to blend in with nearly any surrounding, and hide in plain sight.

### Skating:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Skating skill are able to use special shoes to glide across frozen bodies of water, and perform tricks.

Simple: Able to don skates and stand without falling over or breaking an ankle.

Basic: Able to move across frozen surfaces while wearing skates, albeit with jerky, uncoordinated movements.

Intermediate: Able to move across frozen surfaces without falling.

Advanced: Able to travel quickly across frozen surfaces.

Master: Winter Olympics figure skater.

### Skiing:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Skiing skill are able to use skis to move quickly across snow-covered surfaces.

Simple: Able to don skis and stand without falling over or breaking an ankle.

Basic: Able to move across snow-covered surfaces while wearing skis, albeit with jerky, uncoordinated movements.

Intermediate: Able to move across snow-covered surfaces without falling.

Advanced: Able to travel quickly across snow-covered surfaces.

Master: Winter Olympics slalom competitor.

### Sneaking:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Sneaking skill are able to move quietly, and out of the sight of others.

Simple: Able to creep at ¼ of normal speed with minimal noise.

Basic: Able to remain out of sight while creeping.

Intermediate: Able to creep at up to ½ of normal speed with minimal sound.

Advanced: Able to creep at up to ½ of normal speed without sound.

Master: Able to creep unseen at your normal walking speed without sound.

### Tumble:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Tumble skill are able to recover from instances in which they lose their balance, whether on purpose or by accident, that would otherwise leave them prone.

Simple: Able to roll with the impact of a charge attack to regain your feet.

Basic: Able to reduce the damage from a charge attack.

Intermediate: Able to tuck and roll at the instant of impact to regain your feet after a fall.

Advanced: Able to reduce the damage from a fall.

Master: Able to regain your feet quickly after a massive tremor.

### Ventriloquism:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Ventriloquism skill are able to speak without moving their lips, and “throw their voice”, to make it appear that other creatures, or even objects are speaking.

Simple: Able to talk with minimal movement of your lips.

Basic: Able to handle the basic workings of a ventriloquist dummy to make its mouth move.

Intermediate: Able to coordinate your speech with the movement of objects, such as the lid of a box or the mouth of a ventriloquist dummy, to make it seem as though the object is talking.

Advanced: Able to “throw your voice” to make it sound as though your voice is issuing from somewhere else.

Master: Able to anticipate the movements of other creatures’ mouths, and make it seem as though they’re saying something they’re not.

## Looks

### Camouflage:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Camouflage skill are able to apply makeup and apparel to assist themselves and others in blending with their surroundings.

Simple: Able to apply face paints similar to natural environments to reduce visibility.

Basic: Able to color fabrics similar to natural environments to reduce visibility.

Intermediate: Able to paint objects similar to natural environments to reduce visibility.

Advanced: Able to quickly change makeups and clothes to adapt to different surroundings.

Master: Able to apply colors and coverings to creatures and objects to make them nearly invisible from a distance.

### Disguise:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Disguise skill are able to apply makeup and clothing to change their physical appearance, and give the illusion that they’re somebody else.

Simple: Able to change your features slightly through the use of makeup.

Basic: Able to change your features to be difficult to recognize with makeup and prosthetics, such as wigs.

Intermediate: Able to make yourself look similar to another person with makeup and prosthetics. This disguise doesn’t hold up under scrutiny.

Advanced: Able to make yourself look enough like somebody else to pass as that person to onlookers who are even moderately familiar with the individual.

Master: Able to make yourself look like somebody so well, even very familiar individuals will be fooled, at least by your appearance (other skills may be needed to impersonate the individual’s voice and mannerisms).

### Panhandling:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Panhandling skill are able to play on the sympathy of others in order to elicit various forms of charity from them.

Simple: Able to wave a cup around, and ask for change.

Basic: Able to look dirty and ragged to potentially elicit charity.

Intermediate: Able to look hungry, thirsty, injured, etc. to elicit emotional responses and possibly charity.

Advanced: Able to read and interpret reactions of individuals or even crowds, and tell a sob story to loosen the strings on their Qwartz pouches.

Master: Able to convince people you lost your leg in “the war”, even if you’re obviously standing on two legs.

### Sex appeal:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Sex appeal skill are able to appeal to the carnal urges and desires of others.

Simple: You can identify, and potentially seduce desperate individuals.

Basic: You can identify, and potentially seduce lonely individuals.

Intermediate: You can identify, and potentially seduce single individuals.

Advanced: You can identify, and potentially seduce jilted lovers and spouses.

Master: Able to charm and potentially seduce nearly anybody, regardless of their sexual preference.

## Insight

### Archaeology:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Archaeology skill are able to carefully excavate ruins and artifacts without damaging them.

Simple: Able to dig up objects and ruins. Objects and ruins have a high chance of being destroyed or damaged beyond repair.

Basic: Able to dig up objects and ruins. Objects and ruins have a moderate chance of being damaged.

Intermediate: Able to carefully dig up objects and ruins. Objects and ruins have only a minimal chance of being damaged.

Advanced: Able to restore objects and structures, so long as similar examples exist.

Master: Able to excavate or otherwise recover any object or structure of any size from any environment, potentially without causing any damage to the object or structure. Objects and structures that were already damaged stay that way, but aren’t likely to be further damaged.

### Artistry:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Artistry skill are able to use various media to create visually appealing objects.

Simple: Able to finger paint.

Basic: Able to sculpt basic clay objects or paint with an easel and paint brushes.

Intermediate: Able to sculpt or paint lifelike art.

Advanced: Able to work with porcelain and other delicate materials to create fine works of art.

Master: Able to sculpt, chisel, paint, or otherwise create masterworks of art.

### Cooking:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Cooking ability are able to prepare meals which are suitably palatable.

Simple: Able to put a dead animal over a fire until it’s no longer raw.

Basic: Able to season meat with various spices.

Intermediate: Able to concoct various dishes by combining suitable ingredients.

Advanced: Able to season dishes to create an enjoyable dining experience.

Master: Able to scintillate the palates of large groups of people with multiple course meals.

### Empathy:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Empathy skill are able to read facial expressions and body language to gain insight into the emotions of others.

Simple: Able to identify the emotions of individuals who are experiencing strong emotional states.

Basic: Able to identify the emotions of individuals who are experiencing moderate emotional states.

Intermediate: Able to identify the emotions of individuals who are experiencing minimal or complex emotional states, even if they are trying to hide their emotions.

Advanced: Able to interpret minute and very subtle hints to determine the emotional states of those you’ve spent a lot of time with.

Master: Able to interpret minute and very subtle hints to determine the emotional states of complete strangers.

### Falconry:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Falconry skill are able to train birds of prey to hunt and follow other simple commands.

Simple: Able to handle a well-trained bird of prey, and issue very simple and basic commands taught by its trainer.

Basic: Able to handle moderately well-trained birds of prey, and issue moderate commands taught by its trainer.

Intermediate: Able to handle untrained birds of prey, and begin teaching it very simple commands.

Advanced: Able to train birds of prey in moderately complex commands.

Master: Able to train wild birds of prey, and teach very complex commands.

### First Aid:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the First Aid skill are able to employ various methods to treat injuries.

Simple: Able to apply a bandage to a wound.

Basic: Able to apply salves to rashes and wounds.

Intermediate: Able to set bones and improvise splints.

Advanced: Able to improvise salves and ointments for wounds, rashes, and other injuries.

Master: Able to perform surgery, and make salves and tonics to help people recover from disease, as well as helping them regain vitality points.

### Gardening:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Gardening skill are able to grow fruits, vegetables and other plants.

Simple: Able to grow weeds, and other extremely hardy plants.

Basic: Able to grow hardy plants, such as potatoes.

Intermediate: Able to grow moderately hardy fruits and vegetables.

Advanced: Able to grow minimally hardy plants.

Master: Able to grow delicate flowers, and other extremely frail plants.

### Handle animal:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Handle animal skill are able to read the body language of animals to gain insight into their thoughts and emotions.

Simple: Able to handle well-trained animals, other than a bird or beast of burden, and issue very simple and basic commands taught by its trainer.

Basic: Able to handle moderately well-trained animals, other than a bird or beast of burden, and issue moderate commands taught by its trainer.

Intermediate: Able to handle untrained animals, other than a bird or beast of burden, and begin teaching it very simple commands.

Advanced: Able to train animals, other than a bird or beast of burden, in moderately complex commands.

Master: Able to train wild animals, other than a bird or beast of burden, and teach very complex commands.

### Housekeeping:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Housekeeping skill are able to tidy up and organize buildings ranging from small cottages to large castles.

Simple: Able to dust, sweep and mop.

Basic: Able to organize items which are obviously out of place.

Intermediate: Able to clean and maintain, or oversee a small group of people in cleaning and maintaining a medium sized structure.

Advanced: Able to organize items which are disorganized.

Master: Able to clean and maintain large structures, or a large portion of a huge structure, and oversee the work of a large staff of housekeepers.

### Lip reading:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Lip reading skill are able to watch the mouths of others to determine the words or sounds they’re making, even when they can’t hear them.

Simple: Able to pick out a large number of words without being able to hear them.

Basic: Able to pick out most of the words from a few people without being able to hear them.

Intermediate: Able to read not only lips, but also the movements of muscles in the throat, and the position of the tongue to help narrow down potentially ambiguous or similar sounding words.

Advanced: Able to pick out most of the words in a conversation from any individuals whose mouths you can see.

Master: Able to interpret, and likely reproduce the sounds made by any individual, even if you don’t know their language. This does not, however, confer the ability to understand the meaning of words in languages you don’t know, though you could tell them, with moderate accuracy, to others who may understand. Extremely complex words still have the potential to be misinterpreted, as determined by the Keeper.

### Local culture (specified):
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Local culture skill are able to observe and follow customs of a particular area.

Simple: Able to follow public customs of the selected area.

Basic: Able to observe and participate in minor rituals of the selected area.

Intermediate: Able to correct others in proper observance of customs and rituals in the selected area.

Advanced: Able to anticipate, and properly instruct others in the observance of customs and rituals in the selected area.

Master: Able to recognize and follow customs similar to those in the selected area, even in other areas, with relative accuracy.

### Meteorology:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Meteorology skill are able to determine the weather based on the seasons and prevalent weather patterns.

Simple: Able to tell the difference between normal clouds and rain clouds.

Basic: Able to tell which direction a storm is moving.

Intermediate: Able to read moderately subtle signs in weather patterns to predict changes.

Advanced: Able to read minute signs in weather patterns to predict changes.

Master: Able to sense when a change in the weather is coming almost instinctively.

### Question:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Question skill are able to elicit specific information from others.

Simple: Able to ask people questions about any topic.

Basic: Able to recognize potentially touchy subjects, and ask questions discretely.

Intermediate: Able to recognize individuals who are more likely to know answers to a particular question.

Advanced: Able to recognize individuals who are likely to be forthcoming with answers to questions.

Master: Able to ask questions subtly or cryptically, so as not to draw unwanted attention to sensitive subjects.

### Riding:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Riding skill are able to train and ride beasts of burden, and maintain riding gear.

Simple: Able to ride well-trained beasts of burden, and issue very simple and basic commands taught by its trainer.

Basic: Able to ride moderately well-trained beasts of burden, and issue moderate commands taught by its trainer.

Intermediate: Able to ride untrained beasts of burden, and begin teaching it very simple commands.

Advanced: Able to ride beasts of burden, and train it in moderately complex commands.

Master: Able to ride wild beasts of burden, and teach very complex commands.

### Search:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Search skill are able to carefully examine objects and surroundings to find things of value, or out of the ordinary.

Simple: Able to discover large objects which are out of place or potentially valuable.

Basic: Able to find obvious trap triggers.

Intermediate: Able to find moderately well hidden objects and secret doors.

Advanced: Able to find clever and well hidden traps and trap triggers.

Master: Able to find objects which blend in with their surroundings, but are out of place in any way.

### Teamster:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Teamster skill are able to control teams of animals that pull vehicles, such as a team of horses pulling a carriage, or a team of dogs pulling a sled.

Simple: Able to handle the reigns of a vehicle to steer teams of animals on a well-travelled and maintained road.

Basic: Able to use the reigns of a vehicle to speed up or slow down a team of animals on roads with only minimum upkeep.

Intermediate: Able to guide and steer teams of animals with verbal commands on any road or trail wide enough for the vehicle.

Advanced: Able to increase or decrease the speed of teams of animals with verbal commands over any terrain that will fit a vehicle, possible exceptions being swamps, washed out roads, etc.

Master: Able to coordinate multiple drivers and teams of animals pulling multiple vehicles in a caravan. Also able to organize multiple trade caravans across various trade routes from a central location.

### Tracking:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Tracking skill are able to follow the signs left by other creatures.

Simple: Able to follow fresh, obvious visual cues left by hasty targets, such as footprints in snow, or fresh cart tracks in mud.

Basic: Able to follow fresh clues left by a careful target.

Intermediate: Able to follow clues left by a target within the fairly recent past.

Advanced: Able to find clues left by a careful target within the fairly recent past, even despite environmental changes, such as shifting sands, or heavy rain.

Master: Able to find minute signs left by targets from any period of time.

### Trapping:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Trapping skill are able to employ various forms of traps to capture animals and creatures.

Simple: Able to place traps in areas with the potential to catch or kill something.

Basic: Able to choose appropriate traps to catch a particular size of creature.

Intermediate: Able to discern what types of creatures are likely to be in a particular area.

Advanced: Able to place traps in areas with a high likelihood of catching something.

Master: Able to calibrate traps to be triggered by creatures fitting one or more criteria, such as a particular weight range or height.

## Stamina

### Animal husbandry:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Animal husbandry skill are able to maintain various large groups of animals, ranging from chickens, to cattle, etc.

Simple: Able to raise and care for a single, small group of animals.

Basic: Able to breed and care for a single, moderately sized group of animals.

Intermediate: Able to care for a few, similar groups of animals, such as chickens and ducks, or cows and sheep.

Advanced: Able to care for a few, varied groups of animals, such as cows and chickens, or horses and turkeys.

Master: Able to breed, care for, and maintain the populations of a wide variety of groups of animals.

### Boating:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Boating skill are able to balance weight and work the oars in small watercraft.

Simple: Able to row a small watercraft, such as a canoe or a raft.

Basic: Able to balance loads and people in small watercraft to prevent tipping.

Intermediate: Able to maintain a steady course, even against a current.

Advanced: Able to effectively avoid rocks in strong currents.

Master: Able to effectively guide a boat through rapids.

### Climbing:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Climbing skill are able to scale surfaces using natural textures and/or climbing tools.

Simple: Able to scale surfaces with abundant foot and handholds.

Basic: Able to set up climbing rigs, and use pitons to scale non-overhang surfaces.

Intermediate: Able to scale surfaces with minimal foot and handholds, with or without climbing tools.

Advanced: Able to scale sheer surfaces with proper climbing tools.

Master: Able to scale any surface, including overhangs, with proper tools.

### Farming:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Farming skill are able to harvest, plant, maintain, and rotate crops in large fields.

Simple: Able to recognize when crops are ripe and harvest simple crops by hand.

Basic: Able to employ tools and beasts of burden to harvest and bail crops such as wheat.

Intermediate: Able to irrigate fields and tend the needs of crops to keep them healthy.

Advanced: Able to grow crops in difficult conditions, such as rocky or sandy soil.

Master: Able to rotate crops for soil health and maximum efficiency of available planting space. Also able to grow crops in almost any terrain or weather pattern.

### Prospecting:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Prospecting skill are able to locate and dig up various deposits of metals and other minerals.

Simple: Able to break chunks of ore out of rock with a pickaxe.

Basic: Able to employ explosives for digging up ore. This skill does not confer the ability to make explosives.

Intermediate: Able to excavate veins of metals and minerals with proper tools.

Advanced: Able to excavate precious stones with the proper tools.

Master: Able to excavate veins of metals, minerals and precious stones with improvised tools.

### Sailing:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Sailing skill are able to handle and maintain the riggings and sails on larger watercraft.

Simple: Able to steer large watercraft.

Basic: Able to properly maintain riggings on large watercraft.

Intermediate: Able to maintain the sails on large watercraft.

Advanced: Able to guide large watercraft against the current in large bodies of water.

Master: Able to coax movement out of large watercraft using only the slightest breeze.

### Swimming:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Swimming skill are able to keep themselves afloat, and propel themselves through water effectively.

Simple: Able to tread water.

Basic: Able to doggy paddle.

Intermediate: Able to swim at half walking speed in calm water.

Advanced: Able to stay afloat in turbulent water.

Master: Able to swim at normal walking speed, or half speed in against a current.

## Toughness

### Armor Smithing:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Armor Smithing skill are able to forge and assemble armors consisting mainly of metal.

Simple: Able to repair damaged plate mail and banded mail.

Basic: Able to shape and assemble plate mail and banded mail.

Intermediate: Able to repair damaged chain mail or scale mail.

Advanced: Able to shape and assemble chain mail or scale mail.

Master: Able to repair, fashion, shape and assemble any armor consisting of mainly metal.

### Blacksmithing:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Blacksmith skill are able to forge various items and tools out of metal.

Simple: Able to properly pour molten metal into casts.

Basic: Able to make tongs out of refined pieces of metal.

Intermediate: Able to cut, grind, file, polish, and otherwise refine tools.

Advanced: Able to refine metals into sheets, round stock, and other shapes, to prepare for further shaping.

Master: Able to heat and shape metal into strong tools. Also able to properly quench items to make them sturdy and resilient.

### Furrier:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Furrier skill are able to make and fit horse shoes.

Simple: Able to put shoes on a horse, or remove a horse’s shoes.

Basic: Able to shape horseshoe nails.

Intermediate: Able to modify existing horseshoes.

Advanced: Able to forge horseshoes from the proper metal.

Master: Able to make sturdy horseshoes that fit properly.

### Jumping:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Jumping skill are able to leap long distances, or attempt to land accurately.

Simple: Able to perform a running long jump.

Basic: Able to perform a running high jump.

Intermediate: Able to perform a standing long jump.

Advanced: Able to perform a standing high jump. Also able to take less damage when jumping down from dangerous or potentially lethal heights. This skill only reduces damage if the jump down was intentional (falling or being pushed still deal normal damage).

Master: Able to aim for, and land on, a spot half the size of your foot, assuming you’re able to jump to it (whether it be above you, below you, or at the same height as you).

### Leather armoring:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Leather armoring skill are able to shape, form, harden and assemble armors from the hides or skins of various creatures.

Simple: Able to repair damaged armor consisting mainly of large pieces of leather.

Basic: Able to shape, harden and assemble armor consisting mainly of large pieces of leather.

Intermediate: Able to repair damaged armor consisting of smaller pieces or strips of leather.

Advanced: Able to shape, harden and assemble armor consisting mainly of smaller pieces or strips of leather.

Master: Able to repair, shape, harden or assemble any type of armor consisting mainly of leather, including complex woven and layered leather armors.

### Masonry:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Masonry skill are able to use various materials to build sturdy structures.

Simple: Able to build, repair, or identify weaknesses in simple grass, straw, and stick huts.

Basic: Able to build, repair, or identify weaknesses in log cabins.

Intermediate: Able to build, repair, or identify weaknesses in structures consisting of wood and mortar.

Advanced: Able to build, repair, or identify weaknesses in structures consisting of large stones.

Master: Able to build, repair or identify weaknesses in nearly any constructed or carved structure.

### Weapon Smithing:
> **Status:** ⚠️ REVIEW — recovered Skill/degree content. Preserve the concept and degree descriptions unless contradicted; audit any roll totals, fixed target numbers, time rules, or special failure rules against the current engine.

Specialists with the Weapon Smithing skill are able to forge metal into destructive implements.

Simple: Able to properly pour molten metal into weapon casts.

Basic: Able to make blades out of refined pieces of metal.

Intermediate: Able to cut, grind, file, polish, and otherwise refine weapons.

Advanced: Able to shape metal into knives, swords, axes, arrow heads, and other weapons.

Master: Able to fold, layer, and properly quench items to make them sturdy and resilient.


---

# Chapter 5 — Martial

## Reconstruction status legend

- **✅ CONFIRMED** — established by later explicit decisions and treated as current canon unless deliberately reopened.
- **🔄 SUPERSEDED** — recovered source material that has been replaced by a later decision.
- **⚠️ REVIEW / CONVERSION** — concept or content is useful, but one or more mechanics must be reconciled with the current engine.
- **⬜ NEEDS DEVELOPMENT** — incomplete or absent; substantial design work remains.
- **❗ CONTRADICTION** — two surviving sources or decisions conflict and must not be silently reconciled.
- **💡 SUGGESTION** — design suggestion from this reconstruction pass; not canon unless Mike approves it.

**Authority used in this reconstruction:** newest explicit decisions in the current reconstruction work override older text; CLEAN source files are the baseline for material not subsequently changed. Archival Markdown is treated as a searchable transcription of its CLEAN source, not as independent canon. No discrepancy has been silently fixed.

## 1. Current Martial architecture

**✅ CONFIRMED**

Martial uses the same universal engine as the rest of Boundless. A Specialist builds an action from known Components, applicable Training, the relevant Stat, equipment/weapon profile, Traits, situational modifiers, and AP expenditure. Components are tiered Simple through Master. Martial and Magic may be combined into hybrid actions.

The universal **Critical Die** applies to Martial resolution: a successful qualifying action with a natural 10 on its Critical Die is Crit+; a failed qualifying action with a natural 1 on its Critical Die is Crit-. Specific Martial critical effects are defined by the combat/core rules or by an explicit Component.

**✅ Current tier prerequisites:** 15 / 30 / 45 / 60 / 75 in the relevant governing Stat.

**✅ Later primary-Martial Stat set:** Proficiency / Agility / Toughness. Individual Components may still call on other Stats for opposed checks or effects; CLEAN's blanket Proficiency-ranged / Toughness-melee / Stamina-defensive assignment must be audited rather than automatically applied.

**✅ Training rule:** applicable Training contributes +1d10 per degree. Legacy +2d10-per-degree exceptions are not current.

**✅ Dual wielding:** two weapons do not automatically generate extra actions. An explicit Martial Component/mechanic must construct the dual-wield action.

## 2. AP and Component conversion rules

**✅ Modern AP:** 1 + 2×floor(Speed/10), Speed only. Action ceiling 3/6/9/12/15 by highest tier used. An action must normally be paid in the current turn.

**⚠️ CONVERSION:** CLEAN frequently assumes every Component costs 1 AP and that AP can translate directly into static caps, negative AP counters, repeated attacks, or old defense stages. Those ideas must be rebuilt under the current engine.

**Design constraint from current reconstruction:** avoid arbitrary static resolution numbers such as Catch/Seize Weapon beginning at "40" and decreasing by 5. Convert to dice/successes/opposed checks/AP/Conditions rather than preserving a separate arithmetic subsystem.

## 3. Defense-related Martial content

**✅ Defense paths:** Agility/Unarmored, Insight/Evasion, Stamina/Armor; only one applies per defense roll.

**⚠️ Armor and mitigation:** Martial entries such as Penetration, Armor Conditioning, Favored Shield, Rhino Hide, Pack Attack, and others interact with mitigation. Do not rewrite them until the entire armor ecosystem is reviewed.

## 4. Component-by-component status rule

Unless an entry is explicitly marked otherwise below, treat its **concept/name/tier/prerequisite as recovered design evidence** and its exact numerical implementation as **⚠️ REVIEW / CONVERSION**. This is intentionally conservative: it prevents a useful Component from being lost while also preventing old static math from silently becoming canon.

## 5. Complete recovered Martial catalog

---

# Martial

If Magic is the heart and soul of fantasy, Martial is the backbone of fantasy. Martial abilities deal with the melee and ranged aspect of fantasy combat. Martial abilities are often overlooked in fantasy worlds.

To the untrained, many martial abilities appear as simple as swinging a sword or pointing an arrow and letting it fly. The mechanics behind the Martial system work exactly like the Magic system, in which a Specialist can customize different offensive and defensive maneuvers to use in combat. Specialists with marital training have the option to focus in melee combat, ranged combat, defensive combat or any combination of the three.

Melee combat is the art of fighting up close and personal. This could involve everything from bare hands to swords to hammers and more. The instant a melee weapon leaves a Specialist’s hand as part of an attack, it becomes a ranged weapon. Ranged combat is the art of throwing weapons effectively or utilizing projectile weapons from afar. Although thrown weapons are fairly self-explanatory, a projectile weapon is any weapon that fires a projectile whether from a crossbow, a bow, a slingshot, a sling or even a catapult. Defensive combat is the art of using shields and armor effectively to deflect, minimize and mitigate as much damage as possible. A Specialist can wield a shield in conjunction with either melee or ranged combat, or even use two shields at once in an almost total defensive style of combat.

# Building an Attack

Attacks in Boundless aren’t pre-assembled. Specialists build their own attacks from the components and training they have available. While attacks may be built on the fly, we recommend martial Specialists keep at least a few pre-built attacks on hand to help speed up Combat.

Martial attacks are built by spending Action Points or AP to combine and execute known martial components. Each component costs 1 AP to use. Martial components may be combined with magical components to create hybrid attacks.

Offensive components may only be used on a Specialist’s own turn unless the Specialist possesses and uses the Offensive Defense component. Defensive components may be used on another creature’s turn, but must be used before to-hit or damage are rolled.

# Simple

Simple martial components are the easiest types of attacks. These maneuvers are only slightly better than those of children with toys learned from watching adults practice. A Specialist must have at least 15 points in the appropriate martial stat, Proficiency for ranged, Toughness for melee or Stamina for defensive, to perform simple attacks.

## Offensive

### Accuracy
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

A Specialist with Accuracy may forego Active defense in favor of a more accurate attack using offensive dice. Each AP spent on Accuracy will decrease your Passive defense by 5 as well as increasing your offensive cap and reducing the Passive defense of the target(s) by the same amount against this attack only. A Specialist may not spend AP to reduce their own Passive defense beyond 0. No matter the amount of Passive defense the Specialist sacrifices, the Specialists and the target(s) Passive defense can never be dropped below 0. The penalty to your Passive defense lasts until the start of your next turn.

### Desperation
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

A Specialist with Desperation places all their eggs into one basket to make a single, exceptionally powerful attack and spends their next turn recovering. A Specialist who chooses to make a Desperation attack forgoes Passive defense and may only use up to 1 AP on Active defense for this turn and the subsequent turn. The Specialist may save 1 AP from this turn and the next but spends any remaining AP on this single attack. Each AP spent on this attack increases the offensive cap by 5 points. In addition, if the target takes damage from this attack, the Specialist may choose to knock the target prone or give the target negative AP equal to the AP spent on this attack.

### Distance
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Usable with: Ranged

Distance allows a Specialist to attack from greater distances with reduced penalties. Each ranged weapon has a built-in range, expressed in movement units, at which one does not incur penalties to attack. Attacking beyond this range normally reduces the offensive cap by 10 for each movement unit beyond the range of the weapon. Each AP of Distance is sufficient to increase the effective base range of the weapon by one movement unit. Distance only works with a single weapon. For dual weapons, please refer to Dual.

### Precision
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Precision gives a Specialist a bonus to attack a target within range. This ability may be used in conjunction with Accuracy. Precision may not be used in conjunction with Dual. Precision gives a Specialist a bonus of 1d10 to hit for each AP spent on Precision.

### Riposte
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Usable with: Melee, *

Riposte gives Specialists the ability to quickly counterattack when they successfully defend against any melee attack until the beginning of their next turn. This counterattack is made using the weapon’s normal to-hit dice plus a number of d10 equal to the AP spent on Riposte.

* The counterattack may be made with a ranged weapon, if appropriate, but only in response to a melee attack.

### Simple Attack
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Simple Attack allows a Specialist to fire a projectile weapon, throw a thrown weapon or strike with a melee weapon or unarmed attack to deal damage to a target. Each AP spent on Simple Attack allows the Specialist to add 1d10 to damage with a weapon upon a successful hit. This is in addition to the damage provided by weapon training. All Specialists begin play knowing this component, but it may only be applied to weapons with which the Specialist has taken weapon training.

### Taunt
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

A Specialist with Taunt is able to get into the head of their opponent and draw their attacks. Instead of using a weapon or dealing damage, the Specialist shouts insults at their opponent. This attack automatically “hits”. Instead of dealing damage as normal, the Specialist rolls 3d10 per AP spent to set the strength of the taunt. The target must succeed on an Insight Reaction. If the target’s reaction roll is less than half, they must use all their AP on offensive actions directed at the Specialist on their next turn. If the target’s reaction roll is more than half, they aren’t compelled to use offensive actions, though any offensive actions they do take must be directed at the Specialist.

### Wrestle
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Usable with: Melee

Special: Must have 2 hands free

Wrestle allows a Specialist the opportunity to subdue an opponent, or to injure an already subdued opponent. To wrestle effectively, the initiating Specialist must have two hands free and must be within melee range. When Wrestle is used, the Specialist and the foe make opposed Toughness Reactions, with the Specialist gaining 1d10 to their check for each AP spent on Wrestle. If the defender also has the Wrestle component, they may likewise spend any AP they have to gain an additional 1d10 to their check per AP spent.

The winner of the opposed Wrestle check may choose to pin or disengage their opponent. If the losing opponent is already pinned, the winner may deal 1d10 blunt damage to the pinned opponent for each AP they spent on Wrestle.

 Defensive

### Defense
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Defense provides 1d10 to armor/shield roll for each AP spent on Defense. If the Specialist is wielding a shield and uses this component, they gain a single additional 1d10 on their armor/shield roll, regardless of the number of AP spent on this ability. Specialists must spend the AP on this ability before making any defensive roll, including evasion. If the incoming attack is evaded, the AP spent on this component are still spent.

### Evade
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Evade allows a Specialist to dodge out of the way of incoming attacks. In order to learn Evade, a Specialist must have at least 1 degree of Evasion Training.

Each AP spent on Evade grants a Specialist an additional 1d10 to their evade roll. This is in addition to any evasion dice granted by Evasion Training and Unarmored Training. A Specialist must spend AP on Evade before they roll their evasion roll. This component may not be used to retroactively to increase a Specialist’s evasion roll one die at a time until it thwarts the attack roll.

# Basic

Basic martial attacks are a step above simple. Though they are slightly more complex than simple maneuvers, Specialists can still learn them early on in their martial careers. A Specialist must have at least 30 points in the appropriate martial stat, Proficiency for ranged, Toughness for melee or Stamina for defensive, to perform basic attacks.

## Offensive

### Aggressive
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

A Specialist with the Aggressive component may forego defense in favor of a more brutal attack. Each AP spent increases attack damage by 2d10 and reduces defense by 1d10 until your next turn. May not use more AP than you have defensive dice. You also forego using defensive components until your next turn.

### Deception
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

A Specialist with Deception is able to attack opponents who have been deceived into believing they are dead. In order to use Deception, a Specialist must be able to convince an opponent they have died, such as by means of the Bluff skill. If the opponent is successfully deceived, the Specialist may attack when the opponent draws near to examine the body, or when the opponent attempts to leave the area. Each AP spent on Deception adds 1d10 to hit and damage, and reduces the target’s evade roll by 1d10.

### Distraction
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

A Specialist with the Distraction component is able to distract their opponent and leave them open to attacks. This Distraction deals no damage. Each AP spent increases effective damage dice by 1d10. On a failed Insight reaction, target takes 1d10 penalty to defense against the next attack per AP spent on Distraction.

### Lacerating
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Requirement: Slashing weapon

Specialists with Lacerating excel at opening wounds in targets that bleed excessively unless treated. When a Specialist makes a Lacerating attack, they add 1 damage to the attack per AP spent on the attack. On each of the Specialist’s subsequent turns, wounds that have not been treated with first aid or magical healing gush blood, causing the target to take additional damage equal to the total AP spent on Lacerating.

### Pinpoint
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Pinpoint gives a Specialist the ability to hit small targets, such as foes behind cover, or engaged in melee combat. In general, a Specialist can hit a target of the same size without a penalty to attack. For each size category the target is smaller than the Specialist, the Specialist incurs a cumulative 1d10 penalty to attack. Each AP spent on Pinpoint is sufficient to reduce the penalty as though the target were 1 size category larger. Pinpoint can reduce some, or all, of the penalty for shooting at smaller targets. For example, if a large Specialist wants to attack a small size target (2 size categories smaller), they would normally incur a penalty of 3d10 on their attack roll (1d10 + 2d10 = 3d10). By spending 1 AP on Pinpoint, the large Specialist would instead suffer only a penalty of 1d10, treating the small target as if it were medium. By spending 2 AP, the large Specialist would eliminate the penalty altogether. In essence, the Specialist’s eyes “zoom in” on the target, thereby making it easier to hit. Pinpoint can “zoom in” on a target to the point of reducing the penalty to hit even miniscule objects (less than an inch) to zero, but it never gives a bonus to attack for spending AP beyond that point.

### Quick
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Quick allows a Specialist to load and fire, retrieve and throw or draw and attack with a weapon within the same action. The Quick component reduces the AP cost to draw or load a weapon to 1 AP. Without the use of this component, medium weapons cost 2 AP to draw or load, and large weapons cost 3 AP to draw or load.


Trip

Trip allows a Specialist to trip a target with a projectile, thrown or melee weapon. This attack attempts to sweep the target from their feet. If this attack hits, roll 1d10 per AP spent on Trip. Instead of dealing damage, the damage rolled sets the strength of the trip. The target must make an Agility Reaction. If the target rolls less than half the strength of the trip, they are knocked prone. If they roll more than half, but fail to beat the strength of the trip they have to spent double AP on movement actions until their next turn.


Withdraw

A Specialist with the Withdraw component may withdraw after making an attack. When using this component, a Specialist may take an immediate hop backwards of one movement unit after completing an attack. This may be done whether the attack succeeded or not.

## Defensive

### Parry
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Usable with: Melee, *

Parry allows a Specialist to attempt to block attacks with their weapon instead of a shield. Parry provides plus 1d10 to defensive rolls against melee attacks for each AP spent on Parry, while using a weapon.

* Melee or ranged weapons may be used to parry against melee attacks.

### Protect
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Protect allows a Specialist to defend an ally against an intended attack. In order to use Protect, the Specialist must be within 1 MU of any point on a direct line between the attacker and the attacker’s target. On a successful protection, the attack is defended as appropriate for any components used. For example, if used in conjunction with Catch against a fired arrow, the protector catches the arrow. If not used in conjunction with other components, the attack is simply blocked. If the protection attempt fails, the original target may still defend against the attack as normal, but the protector takes damage from the attack as though they were the target, and failed their defense roll.

Attempting to protect a target imposes a penalty on the Specialists defensive action. This penalty starts at 5d10 for 1 AP and is reduced by 1d10 for each additional AP spent on Protect. At 5 AP, the penalty is negated (0d10). At 6 AP and above, the Specialist gains a bonus of 1d10 per additional AP spent on Protect.

### Shadow
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Specialists with Shadow are able to maintain the approximate distance between themselves and other creatures.

When used to follow another creature or maintain distance laterally, the Specialist may move up to their Speed Rating for each AP spent to maintain the distance between them and a target when the target takes an action that involves movement.

When used to retreat from another creature, the Specialist chooses a number of AP to spend, and moves a number of movement units equal to the AP spent times their Speed Rating away from the target when the target takes an action that involves movement.

# Intermediate

Intermediate attacks are a step above basic. Martial Specialists require some training before they begin to learn intermediate attacks. A Specialist must have at least 45 points in their primary martial stat to perform intermediate attacks.

## Offensive

### Cheap Shot
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

A Specialist with Cheap Shot excels at attacking disabled foes. On a successful Cheap Shot against a foe who is stunned, paralyzed, or otherwise unable to defend themselves, this attack automatically deals full damage. If the damage dealt is more than the target’s Endurance Score, the target is slain outright. Cheap Shot costs only 1 AP, but may not be used in conjunction with other components. Spending additional AP on Cheap Shot increases to-hit by 1d10, and damage dealt on a successful attack by 10.

### Dual
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Dual allows a Specialist to apply ranged attack components to an off-hand ranged weapon. To apply Dual, build the attack as normal and determine the degree. In order to apply the attack to the Specialists off-hand, the Specialist must spend 1 AP per degree on Dual. For example, 1 AP for Simple, 2 AP for Basic, etc.

### Harass
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

A Specialist with Harass excels at annoying opponents into attacking them. When a Specialist uses Harass, the effects apply to all attacks made in that round (even defensive attacks). Each AP spent on Harass bestows one aggression, or “aggro,” token on any target who takes damage until the Specialist’s next round. Using Harass adds additional aggro tokens with each subsequent use. At the beginning of its turn, any target with at least one aggro token must make Insight Reactions, the strength of which is set by the Specialist rolling 1d10 for each aggro token the enemy has accumulated. A target who rolls less than half the strength must use all AP to attack the Specialist on their next turn. A target who rolls more than half, but less than the strength may only target the Specialist with damaging components, but may choose not to attack. A target who rolls equal to, or greater than, the strength may choose to target someone other than the Specialist.

If a target with aggro tokens targets the Specialist, each AP spent in attacking the Specialist removes one aggro token.

### Irregular Attack
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

A Specialist with Irregular Attack uses their weapon to deal alternative types of damage. Using Irregular Attack, the Specialist changes the way they attack to take advantage of the weapon’s physical characteristics to deal piercing, slashing, blunt or hacking damage in place of its usual damage type. The weapon must be capable of dealing the specified damage type. For example, a Specialist could choose to do piercing, slashing, blunt or hacking damage with a sword, but could would not be able to deal slashing damage with a maul or club.

### Mobile
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Mobile allows a Specialist to shoot or throw a weapon at a target while moving on foot. Normally, you may only move before or after an attack.

During any movement action a Specialist takes, the Specialist may spend additional AP on Mobile to attack while moving. Each AP spent is sufficient to allow 1 attack. For example, a Specialist who spends 3 AP on Mobile may make 3 attacks during their move action. Movement actions used in conjunction with Mobile must be in a straight line, though subsequent moves may be in different directions. The Specialist’s attack(s) may be made from any point between the beginning and ending point of the move.

### Pack Attack
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Specialists with Pack Attack excel at working together to take down a single target as quickly and viciously as possible. Specialists derive the greatest benefit from Pack Attack by making consecutive attacks against the same target. For each successful Pack Attack made against a target, the target gains a Pack Attack token. For each Pack Attack token a creature has, they take a penalty of 1d10 to their Evasion against any other Specialist using Pack Attack. Furthermore, when using Pack Attack against a target that already has Pack Attack tokens, the Specialist may choose one additional effect to apply to their pack attack. Possible effects are additional Evasion reduction, armor/shield reduction, mitigation reduction, increased to hit or increased damage on a successful hit. The effect must be chosen prior to making the attack. Pack Attack increases or decreases the target’s or Specialist’s roll as appropriate.

Any creature that begins its turn with Pack Attack tokens immediately loses all Pack Attack tokens on them.

### Pushback
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

A Specialist with Pushback may force opponents away from them. When using Pushback, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the Pushback. If the opponent fails on a Toughness Reaction, they’re pushed back by 1 movement unit for each AP spent on Pushback. A Specialist may not spend more AP on Pushback than the 10s digit of their Toughness Score. The Specialist may choose whether to move with the target or not.

### Stun
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Stun allows a Specialist to immobilize a foe for a short time on a successful attack. When making a Stun, roll attack vs defense as normal. If the attack succeeds, the attacker forgoes dealing damage. Instead, the attacker bestows negative AP counters. Each AP spent on Stun is sufficient to bestow 1 negative AP counter to the target. Specialists with negative AP counters may not take any actions other than to remove negative AP counters at the cost of 1 AP per counter. Negative AP counters last until removed by spending AP.

## Defensive

### Disarming Block
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

A Specialist with Disarming Block is able to knock the weapons out of foes hands on successfully blocking attacks. To use Disarming Block, a Specialist foregoes their evasion and armor dice to their defense roll. Instead, they only gain their shield dice and 1d10 per AP spent on Disarming Block. On a successful block, the attacker’s weapon is knocked out of their hand.

### Seize Weapon
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Seize Weapon gives the Specialist the opportunity to take an attackers weapon from them, if they are within melee range. Seize weapon doesn’t allow a Specialist to take ammunition or projectiles, but does allow them to grab the weapon that fires ammunition or projectiles, such as a bow or sling. Seize Weapon may only be used if the Specialist has at least one empty hand. If the seize attempt is successful, the Specialist disarms the attacker, and may choose to stow, hold or drop the weapon as part of the seize action. If Seize Weapon is used in conjunction with Defense or Parry, the Specialist may not spend more AP on Defense or Parry than they spent on Seize Weapon.

Attempting to seize an incoming weapon imposes a penalty on the Specialists defensive action. This penalty starts at 40 for 1 AP and is reduced by 5 for each additional AP spent. At 9 AP spent, the penalty is negated (0). At 10 AP and above, Seize Weapon gains 5 bonus for each additional AP spent on Seize Weapon.

# Advanced

Advanced attacks are a step above intermediate attacks. Martial Specialists require extensive training before they can begin to learn advanced attacks. A Specialist must have at least 60 points in their primary martial stat to perform advanced attacks.

## Offensive

### Charge
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

A Specialist with Charge may apply the force of their movement to their weapon for devastating damage. Each AP spent on Charge Attack allows a Specialist to move a number of movement units equal to their Speed Rating, and adds 1d10 to their damage on a successful attack. Movement made with this attack must be in a straight line toward the target.

### Deadly
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Deadly allows a Specialist wielding a ranged weapon to hit their target with great accuracy, typically from cover or concealment, to do massive damage. Each AP spent on Deadly adds 1 point of bonus damage to each damage die rolled for the attack. For example, if a Specialist spends 3 AP on Deadly, they would roll 3d10, and add 3 points of bonus damage for each die, for a total of 9 bonus damage.

If other offensive components are used in conjunction with Deadly, the bonus damage applies all damage dice rolled. For example, if a Specialist spends 2 AP on Deadly and 2 AP on Mobile, the Specialist would roll a total of 4 damage dice, adding 4 bonus damage to each, for a total of 16 bonus damage.

### Disable
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

A Specialist with Disable is able to use their weapon to pin or otherwise hinder the use of foes weapons or shields. On making a successful Disable, roll for damage as normal. Instead of dealing damage directly, the foe must make a Toughness Reaction versus the strength of the disabling attack. If the target rolls less than half the strength of the disabling attack, their weapon or shield is pinned until the end of their next turn. If the target rolls more than half, but less than the strength of the disabling attack, their weapon or shield is pinned until the beginning of their next turn. If they roll more than the strength of the disabling attack, their weapon or shield is not pinned. On a successful hit with this attack, the Specialist relinquishes the weapon used. Assuming the weapon remains intact, it may be recovered later.

### Disarm
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Disarm allows a Specialist to attempt to knock objects (typically weapons) out of the hands of their foes. Specialists must know Pinpoint or Parry in order to learn Disarm. Disarm is essentially the art of using Pinpoint to target a handheld object (or the hand holding the object) in order to cause the target to drop it.

To use Disarm offensively, a Specialist must know Pinpoint. The Specialist specifies the number of AP to spend and an object held by the target, then rolls to attack the target as normal. If the Specialist misses the target, the AP are still spent.  If the Specialist hits, he or she rolls damage as normal. Instead of applying the damage to the target, this sets the strength of the disarming attempt. The target of disarming must succeed at a Toughness Reaction versus the strength of the disarm or lose hold of the object.

To use Disarm defensively, the Specialist must know Parry. When used defensively with a ranged weapon, the Specialist doesn’t actually try to shoot the weapon out of their foe’s hand, but instead uses their bow, crossbow or thrown weapon to attempt to knock the foe’s weapon out of their hand. In order to apply this component, a Specialist must first successfully defend against the attack by beating the attacker’s to-hit roll with their total defense roll (evasion and/or armor/shield). Upon successful defense, the Specialist spends the appropriate AP and rolls damage as normal. Instead of applying the damage to the target, this sets the strength of the disarming attempt. The target of disarming must succeed at a Toughness Reaction versus the strength of the disarm or lose hold of the object.

### Hook Shield
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

A Specialist with Hook Shield is able to kick, hit, or otherwise push past an opponent’s shield and invade their territorial bubble. A Specialist attempting to use Hook Shield rolls to hit as normal, adding 1d10 for each AP spent on Hook Shield. The target rolls defense adding their Evasion dice and Shield dice, but not Armor dice. If the Hook Shield roll equals or beats the target’s Evasion and Shield rolls, the Specialist may make an immediate attack against the target, forcing the target to forego their Evasion and Shield rolls, as well as Shield mitigation.

### Mounted
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Mounted allows a Specialist to shoot or throw a weapon at a target while riding a mount. Normally, while mounted, you may only attack if your mount is stationary.

During any mounted movement action a Specialist takes, the Specialist may spend additional AP on Mounted to attack while moving. Each AP spent is sufficient to allow 1 attack. For example, a Specialist who spends 3 AP on Mounted may make 3 attacks during their move action. Movement actions used in conjunction with Mounted must be in a straight line, though subsequent moves may be in different directions. The Specialist’s attack(s) may be made from any point between the beginning and ending point of the move.

### Penetration
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

A Specialist with Penetration is able to forego attack and damage to bypass an opponent’s armor. Each AP spent on Penetration decreases the target’s armor roll (but not shield roll) and armor mitigation (but not shield mitigation) by 1d10.

### Sadistic Strike
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Specialists with Sadistic Strike enjoy taunting their opponents with, “Quit hitting yourself…” To use Sadistic Strike, a Specialist must be in melee range. When a Sadistic Strike is initiated, the target and the attacker roll opposed Toughness Reactions, with the attacker gaining 1d10 bonus to their roll for each AP spent on Sadistic Strike. If the attacker wins the roll, they may immediately deal damage to the target using the target’s own weapon damage dice. If the target wins, they get to immediately deal their weapon’s damage dice to the attacker instead. Regardless of who wins the opposed reaction, the only damage dealt with this attack is using the damage dice provided by the target’s weapon.

## Defensive

### Bulwark
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

A Specialist with Bulwark may forego attacking to gain increased defense until their next turn. Each AP increases all defense rolls by 1d10 until the Specialist’s next turn. When using Bulwark, the Specialist foregoes the ability to use components which result in damage to a target until their next turn.

### Catch
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

 Catch gives the Specialist the opportunity to catch incoming ranged attacks. Catch may only be used if the Specialist has at least one empty hand. If the Catch attempt is successful, the Specialist catches the missile, and may choose to stow, hold or drop it as part of the Catch action.

Attempting to catch an incoming missile imposes a penalty on the Specialists defensive action. This penalty starts at 40 for 1 AP and is reduced by 5 for each additional AP spent on Catch. At 9 AP, the penalty is negated (0). At 10 AP and above, the Specialist gains a bonus of 5 per additional AP spent on Catch. If the Specialist uses Catch in conjunction with Defense or Parry, the Specialist may not spend more AP on Defense or Parry than they spent on Catch.

### Redirect
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Redirect allows a specialist to redirect an incoming attack. On a successful redirection, the Specialist gains the ability to determine where, exactly, the attack finally lands. Attempting to redirect imposes a penalty on the Specialists defensive action. This penalty starts at 30 for 1 AP and is reduced by 5 for each additional AP spent. At 7 AP, the penalty is negated (0). At 8 AP and above, Redirect gives a bonus of 5 per additional AP spent on Redirect. If Redirect is used in conjunction with Defense or Parry, the Specialist may not spend more AP on Defense or Parry than they spent on Redirect.

Melee attacks subject to redirection instead hit a valid target within melee range of the attacker. The attacker keeps the same attack total including all pertinent modifiers. The new defender may choose to defend against this attack, however they may not again redirect the same attack.

Ranged attacks subject to redirection instead hit a valid target within the remaining range of the original attack, potentially to include the original attacker. The attacker keeps the same attack total including all pertinent modifiers. The new defender may choose to defend against this attack, however they may not again redirect the same attack.

# Master

Master attacks are the strongest attacks Specialists can learn. Only the most dedicated martial Specialists will ever learn master level attacks. A Specialist must have at least 75 points in their primary martial stat to perform master attacks.

## Offensive

### Cripple Limb
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

A Specialist with Cripple Limb is able to disable the limbs of their foes with precision attacks. On a successful hit using Cripple Limb, roll damage as normal. Instead of dealing damage directly, this sets the strength of the Cripple Limb. The target must succeed at an Endurance Reaction versus the strength of this attack. Targets that roll less than half the strength of this attack lose the loss of that limb until they receive healing, whether by magic or first aid. Targets that roll more than half, but less than the strength of this attack lose the use of the limb for a number of rounds equal to the AP spent on this attack.

### Dim Mak
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Specialists with Dim Mak, or “touch of death” may attack certain pressure points in an enemy that cause the enemy’s heart to explode. This attack may not be made with a weapon. The attacker rolls their to-hit as normal. When the defender rolls their defense roll, they substitute their armor’s mitigation in place of their armor. The defender’s evasion and armor bonus from shields remain the same.

On a successful hit, roll 1d10 per AP spent on Dim Mak. Instead of dealing damage, the roll sets the initial strength of the Dim Mak. The defender must roll an Endurance Reaction against the strength of the attack. If the defender rolls less than half the strength, they are slain outright. If the target rolls more than half, but fails to beat the strength of the attack, they survive, but must continue making checks on the attacker's turn until they either succeed or fail or a number of rounds equal to the number of AP spent on Dim Mak elapses. If the defender rolls higher than the strength of the Dim Mak, they overcome it, and no longer need to make checks.

### Disruption
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Specialists with Disruption aim to hinder the focus of their opponents. Disruption may only be used on an opponent’s turn in response to an action which requires focus. To use this attack, the Specialist must hit the target and roll damage as normal, adding 2d10 per AP spent on Disruption. Instead of dealing damage directly, the target must succeed on a Focus Reaction, or lose their Focus.

### Overwhelm
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Overwhelm allows a Specialist to hit an opponent where it hurts most. In addition to dealing normal damage, a successful Overwhelm allows a Specialist the option to damage either the target’s Primary Martial Stat or Primary Magic Stat (attacker’s choice). The amount of damage to the primary stat is equal to the cumulative number of AP spent on the Overwhelm. For example, if a Specialist spends 5 AP on Overwhelm and the attack hits, the target would take 15 damage (1 + 2 + 3 + 4 + 5 = 15) to the chosen primary stat. Primary stat damage heals at the same rate as the target’s Vitality Points, or may be healed by magic.

If a target’s primary stat is dropped below the amount necessary to use a component, the target may not use those components until they regain their primary stat points. For example, a Specialist whose Primary Martial Stat is dropped below 75 may no longer use master level martial components.

### Pierce
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Pierce allows a Specialist to hit multiple targets in a straight line with a single thrown or projectile weapon. Each AP spent on Piercing Shot/Piercing throw is sufficient to allow a thrown or projectile weapon to hit 2 targets, in order from nearest to farthest, in a straight line from the attacker. For example, if a Specialist spends 3 AP on Pierce, the thrown or projectile weapon will hit up to 6 targets. When using this ability, make a single attack roll and a single damage roll. Each target hit by the weapon may defend against it separately. If any target manages to deflect, shield or snatch the weapon, no subsequent targets take any damage. Targets that manage to evade or dodge the weapon do not change the way this attack affects the remaining targets in any way.

### Scatter Shot
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Scatter Shot allows a Specialist to throw or shoot multiple weapons at numerous targets in a spread in front of the Specialist. Essentially, the Specialist grabs a handful of thrown weapons, or loads several projectiles into the same weapon, and makes a single attack against multiple targets within range in a 180 degree arc in front of the Specialist. Each AP spent on Scatter Shot is sufficient to increase the number of possible targets by 3. Each use of Scatter Shot consumes a number of projectiles or thrown weapons equal to 3 times the AP spent. If less ammunition is used, the maximum number of targets is equal to the amount of ammunition used.

### Trick Shot
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Trick Shot allows a Specialist to ricochet projectile or thrown weapons off surfaces. This allows a single projectile or thrown weapon to potentially hit multiple targets, and also to potentially hit targets that are around corners. Each AP spent on Trick Shot is sufficient to add an additional ricochet. For example, if a Specialist spends 1 AP on Trick Shot, the thrown weapon or projectile would bounce off one surface and hit another. If the same Specialist spent 3 AP on Trick Shot, the thrown weapon or projectile would bounce off 3 targets, and finally hit a 4th. Trick Shot or Trick Throw does not extend the range of the projectile, though this component may be used in conjunction with any other component that does extend range for projectiles. Total distance is measured as normal, with the direction changing between each point of contact on a surface until the final target is reached.

### Whirlwind
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Whirlwind transforms a Specialist into a terrifying cyclone of pain and destruction. A Whirlwind attack allows a Specialist to make a series of rapid strikes on any and every target within melee range. Each AP spent on Whirlwind is sufficient to allow the Specialist one attack against all targets within range. All targets that fail to defend take the same amount of damage. Each additional attack uses its own new attack and damage rolls, but in all other respects, behaves as the initial attack. Whirlwind may not be used in conjunction with any attack that requires precision to execute, such as Accuracy, Precision, Riposte, Wrestle, Deception, Pinpoint, Disable, Deadly, Mounted, Sadistic Strike, Cripple Limb, Dim Mak, Overwhelm and Trick Shot. The Keeper decides whether an attack may or may not be used in conjunction with Whirlwind.

## Defensive

### Offensive Defense
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Specialist with Offensive Defense may make offensive actions in reaction to an opponent’s actions. Each AP spent on Offensive Defense allows a Specialist to spend 1 AP on an offensive combat action to use defensively on another creature’s turn. For example, if a Specialist wishes to use 3 AP of Focused Strike against an attacker, they would need to first spend 3 AP on Offensive Defense (for a total of 6 AP). The defender's Offensive Defense occurs after the attacker's attack.

### Rhino Hide
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Rhino Hide allows a Specialist to mitigate additional damage from incoming attacks. In order to learn Rhino Hide, a Specialist must have Armor Training, Evasion Training, Shield Training or Unarmored training. In order to use Rhino Hide defensively, the conditions for the prerequisite training must be in effect. E.G. a Specialist with Armor Training as a prerequisite to Rhino Hide must be wearing armor to use Rhino Hide. Specialists with more than one of the prerequisite trainings only need to meet one of the conditions. So a Specialist with Armor Training and Shield Training may use Rhino Hide if they have either armor or shield, or both armor and shield.

Each AP spent on Rhino Hide allows a Specialist to roll an additional d10 for damage mitigation versus incoming attacks. The Specialist must spend AP on Rhino Hide prior to determining success or failure of the incoming attack.

# Martial Training

### Weapon Training
> **Status:** ✅ CONFIRMED IN PRINCIPLE — applicable Training contributes +1d10 per degree; weapon-specific prerequisites/equipment details still need audit.

Specialists trying to use weapons without training do so at a penalty. Small weapons and wands give an attack penalty of 1d10. Medium weapons and rods give a penalty of 3d10 when wielded with one hand, or a penalty of 2d10 when wielded with 2 hands. Large weapons and staves give an attack penalty of 4d10. A specialist may not use components other than Simple Attack when using an untrained weapon. A specialist with even 1 degree of weapon training with a given weapon no longer takes a penalty when using that weapon and may now use martial and/ or magic components with that weapon.

A specialist may only apply components to attacks made with weapons of equal or better training. For example, a Specialist may only use simple components with a weapon if they only have simple training in that weapon. If the Specialist has intermediate training in a weapon, they may use simple, basic or intermediate martial components with that weapon.

A Specialist with training in wands, rods or staves may apply the weapon’s to-hit and damage to spells they cast while wielding the weapon, but only if the spell’s degree is lower than or equal to the Specialist’s degree of training in that weapon.

A Specialist may approach Weapon Training one of two ways. They may select a specific weapon they like, such as katana or crow bill, then figure out what size it is (in this case, both are medium). Conversely, they may choose between ranged and melee then choose a size, such as small and ranged or large and melee, then figure out weapons that fit into those categories, such as a hand crossbow or a splitting maul respectively. Wands, rods and staves may be considered melee or magical, interchangeably.

All weapons have at least one damage type. The damage types are slashing, piercing, blunt and hacking. For weapons that have more than 1 damage types, such as a sword, which has slashing, hacking, piercing and possibly blunt, a Specialist may choose one damage type in which to train at simple Weapon Training. At intermediate Weapon Training, the Specialist may choose another damage type. Finally, for master Weapon Training, the Specialist may choose a third damage type. In order to deal a different damage type with a weapon than the Specialist has trained for, the Specialist would need to use the Irregular Attack component. For example, if a Specialist has trained to master degree in medium melee with slashing, hacking and piercing, and find themselves needing to deal blunt damage, they could use Irregular Attack to do so.

Weapon training covers all weapons of similar size and damage type which are melee or ranged, as appropriate. For example, a Specialist who chose medium slashing melee weapons could use a long sword, rapier or katana with equal skill, but not an axe, mace or club. Similarly, a Specialist who chose katana and blunt could also still use the club, mace, long sword, etc. as blunt weapons only.

Each degree of Weapon Training gives a Specialist an additional 1d10 on the Specialist’s to-hit rolls made with applicable weapons. A Specialist requires a minimum Toughness score, for melee weapons, or Proficiency score, for ranged weapons, of 15 for simple, 30 for basic, 45 for intermediate, 60 for advanced, and 75 for master. To train with wands, rods and staves, the Specialist needs to meet the prerequisite score in Charisma, Intelligence or Insight to use it as a magic weapon, or Toughness to use it as a melee weapon.

### Favored Weapon
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Specialists who favor a particular weapon may train more extensively in that weapon to derive greater benefits from their training. For example, a Specialist who favors katanas may choose to use katanas exclusively. A Specialist may not take more degrees of Favored Weapon than they have in Weapon Training which is applicable to the appropriate weapon. In the case of the katana, this would be medium melee weapons.

Each degree of Favored Weapon gives the specialist an additional 1d10 to damage only when using the specific named weapon.  Using other weapons still gives the Weapon Training bonus if applicable, but not the Favored Weapon bonus. For example, a Specialist with a katana as their favored weapon would gain their Weapon Training bonus while using a long sword, but would not gain the Favored Weapon bonus.

### Unarmed Training
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

A Specialist with Unarmed Training may treat attacks made without weapons as though they were made with weapons. Unarmed attacks are treated as small, blunt weapons. Unarmed Training also allows a Specialist to take degrees in Favored Weapon (Unarmed).

### Unarmed Piercing/Slashing/Hacking
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

A Specialist with Unarmed Piercing/Slashing/Hacking training may treat their unarmed attacks as though they were made with a piercing, slashing or hacking weapon, as appropriate. A Specialist may not take more degrees of Unarmed Piercing/Slashing/Hacking than they have degrees in Unarmed Training. A Specialist may only make Unarmed Piercing/Slashing/Hacking attacks with components of equal or lesser degree than they have in Unarmed Piercing/Slashing/Hacking. The first degree of Unarmed Piercing/Slashing/Hacking allows the Specialist to choose one of the three damage types to add to their unarmed attacks. At intermediate, they may choose another damage type. At master, the Specialist gains the final damage type, and may treat any unarmed attack as blunt, piercing, slashing or hacking as they see fit.


Dual Wield

Dual Wield training allows a Specialist to use a weapon in each hand. Without Dual Wield training, a Specialist attempting to use two weapons takes a penalty for each weapon to all actions involving weapons. The penalty is 1d10 for small and 2d10 for medium weapons. Thus, attempting to use two small weapons gives a total penalty of 2d10 for all weapon based actions, using a small and medium weapon together gives a total penalty of 3d10 to all weapon based actions, and using two medium weapons gives a penalty of 4d10. Dual wield may be applied to two melee weapons or two ranged weapons, but not one of each.

A Specialist’s degrees in Dual Wield may not surpass the training degrees the Specialist has in their highest trained weapon. For example, if a Specialist’s highest trained weapon is intermediate training in a short sword, the Specialist may train up to intermediate Dual Wield, but may not train advanced or master Dual Wield.

When dual wielding, a Specialist may only apply training up to the lower of the two weapons wielded on attacks. For example, if a Specialist uses a short sword (intermediate) in one hand, and a mace (basic) in the other hand, the Specialist may only apply up to basic Dual Wield (the lower of intermediate and basic). In this case, the Specialist may only apply up to basic components to attacks made while dual wielding.

### Evasion Training
> **Status:** ✅ CONFIRMED DEFENSE PATH — paired with Insight; mutually exclusive with the other defense paths on a given defense roll. Equipment restrictions still apply.

A Specialist may choose to train their bodies to evade potentially harmful attacks. To train in evasion, a Specialist requires a minimum Agility score of 15 for simple, 30 for basic, 45 for intermediate, 60 for advanced, and 75 for master. Each degree of Evasion Training grants the Specialist 1d10 to their evasion roll. This bonus applies whether they wear armor or not.

### Armor Training
> **Status:** ✅ CONFIRMED DEFENSE PATH — paired with Stamina; mutually exclusive with the other defense paths on a given defense roll.

A Specialist may choose to wear armor. Without training in armor, a Specialist gains the benefits of the damage mitigation granted by the armor, but the Specialist takes a penalty to defense equal to the mitigation gained by the armor worn. For example, a Specialist wearing light armor would gain 2d10 mitigation but take a penalty of 2d10 to defense rolls. In addition, a Specialist’s AP per turn is reduced by 1 for each 5-point increment by which their Stamina is lower than the requirement. For example, a Specialist with 13 Stamina attempting to wear light armor (a requirement of 30 Stamina) would take a AP penalty of 4, since they are within the fourth 5-point increment below 30.

A Specialist who is trained in armor has no penalty for wearing that armor, and gains the appropriate bonuses to defense rolls, as well as the mitigation granted by the armor. Armor training requires a minimum Stamina score of 15 for simple, 30 for basic, 45 for intermediate, 60 for advanced, and 75 for master. Each degree of Armor Training a Specialist takes grants them an additional 1d10 to the armor portion of their defensive rolls.

### Armor Conditioning
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Specialists who have taken armor training may also take armor conditioning. Armor conditioning is the process of becoming used to the feel of, and being more comfortable in, armor. A Specialist’s armor conditioning degree may not surpass their degrees in armor training with that armor. For example, a Specialist with intermediate armor training may take up to  intermediate armor conditioning, but may not take advanced armor conditioning without first taking advanced armor training.

Specialists may take Armor Conditioning in cloth, light, medium and heavy armors separately. A Specialist requires a minimum Stamina score of 15 for simple, 30 for basic, 45 for intermediate, 60 for advanced, and 75 for master. Basic through master degrees of armor conditioning reduce the effective weight of armor worn (but not shields carried) by 25% each. This means that a Specialist with master armor conditioning treats their armor worn as though it were weightless. This reduction doesn’t apply to armor that is carried but not worn.

Specialists gain an additional 1d10 to their damage mitigation provided by armor for each degree they have in Armor Conditioning while wearing their chosen type of armor.

### Unarmored Training
> **Status:** ✅ CONFIRMED DEFENSE PATH — paired with Agility; mutually exclusive with the other defense paths on a given defense roll and unavailable while armored.

A Specialist may also choose to not wear armor. Specialists may train in unarmored defense as opposed to armored defense. To train in unarmored defense, a Specialist requires a minimum Agility score of 15 for simple, 30 for basic, 45 for intermediate, 60 for advanced, and 75 for master. Specialists trained in unarmored defense gain no damage mitigation, however they gain 2d10 to their evasion roll for each degree; a total of 10d10 for master rank, while wearing no armor.

### Armored Casting
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Armored Casting is for Specialists who want to wear armor and cast spells. A Specialist may only take Armored Casting in an armor type in which the Specialist has Armor Training. Armored Casting is advanced training for the Specialist so that they, in effect, get used to wearing specific types of armor while casting. Normally, when a Specialist is wearing armor and wants to cast spells, the weight and bulk of the armor being worn interferes with the casting process.

Normally, a Specialist attempting to cast a spell while wearing armor takes a penalty based on the highest degree of magic component used in the spell. This penalty is 1d10 for simple, 2d10 for basic, 3d10 for intermediate, 4d10 for advanced and 5d10 for master. This penalty doubles if the Specialist also lacks the appropriate degree of training in the armor they are wearing. A Specialist with Armored Casting training no longer takes the penalty for spells whose highest degree component is lower than or equal to their degrees of training in Armored Casting. For example, a Specialist with intermediate Armor Training and basic Armored Casting training could cast simple or basic spells without penalty. If this Specialist attempted to cast a spell with an intermediate component, they would take a 3d10 penalty to hit with the spell. If the same Specialist tried to cast an advanced spell, they would take a penalty of 8d10 to hit (4d10 for lacking the proper Armored Casting training, and doubled for lacking the appropriate Armor Training.)

### Shield Training
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Without Shield Training, Specialists suffer an attack and defense penalty of 1d10 for using small shield, 2d10 for medium shields, 3d10 for large shields, and a penalty of 4d10 for attempting to use a tower shield.

A Specialist with even a single degree of Shield Training no longer takes these penalties with the appropriate type of shield. When taking degrees of training, a Specialist chooses from small, medium, large and tower. A Specialist requires a minimum Toughness score of 15 for simple, 30 for basic, 45 for intermediate, 60 for advanced, and 75 for master. Each degree of Shield Training gives the Specialist an additional 1d10 to the shield portion of their defensive rolls.

### Favored Shield
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Specialists who favor a particular shield may train more extensively in that shield to derive greater benefits from their training. For example, a Specialist who favors tower shields may choose to use tower shields exclusively. A Specialist may not take more degrees of Favored Shield than they have in Shield Training which is applicable to the appropriate shield.

Each degree of Favored Shield gives the specialist an additional 1d10 to their damage mitigation rolls provided by the shield only when using the specific shield.

### Shield Attack
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Shield Attack training allows a Specialist to use a shield as though it were a melee weapon. A Specialist may attempt to attack with a shield without training, but the Specialist does so with a penalty of 1d10 for small, 2d10 for medium shields, 3d10 for large shields, and a penalty of 4d10 for tower shields.

A Specialist may not train higher degrees of Shield Attack than they have in Shield Training.

A Specialist with shield attack training gains a bonus on attacks equal to the shield’s defense and a damage bonus equal to its damage mitigation (4d10/1d10 for small, 3d10/2d10 for medium and 2d10/3d10 for large, and 1d10/4d10 for tower). Each degree of Shield Training gives the Specialist an additional 1d10 on to-hit rolls made to attack using the appropriate shield. All attacks made with basic, unmodified shields count as blunt damage. Shields modified with spikes or sharpened edges can deal piercing, hacking, or slashing damage, as appropriate.

### Dual Shield
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Dual Shield training allows a Specialist to use a shield in each hand. Without Dual Shield training, a Specialist attempting to use two shields takes a penalty for each shield to all actions involving shields. The penalty is 1d10 per small shield, 2d10 each for medium shields, 3d10 each for large shields and 4d10 each for tower shields. Thus, attempting to use two small shields gives a total penalty of 2d10 for all shield based actions, using a small and tower shield together gives a total penalty of 5d10 to all shield based actions, and using two tower shields gives a penalty of 8d10. Specialists attempting to make shield attacks with dual shields, who do not have training in Shield Attack suffer these penalties in addition to the penalty for not being trained in Shield Attack. Continuing with the previous example, a Specialist without dual shield training attempting to make a shield attack with two tower shields would suffer 16d10 to attack with both shields. A Specialist may not use Dual Strike with shields without the appropriate training in both Shield Attack and Dual Shield.

Regardless of whether or not the Specialist is trained in Shield Attack, a Specialist with Dual Shield training may choose to use two equipped shields for defense. In order to use components other than Defense with two shields, a Specialist requires degrees in Dual Shield and degrees in Shield Attack equal to or greater than the prospective components. For example, a Specialist wishing to use Stun (intermediate) with dual shields would need to have at least intermediate training in Dual Shields and intermediate training in Shield Attack.

### Double Threat
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Double Threat training allows a Specialist to use a melee weapon in one hand, and a ranged weapon in the other hand. Without Double Threat training, a Specialist may use only the melee weapon or the ranged weapon in the same action, but not both. Double Threat training requires training in each of the weapons to be used. For a weapon to be used with Double Threat, the Specialist must be capable of using the weapon in one hand. For example, a Specialist could use an appropriately sized crossbow with a dagger, but would never be able to use a compound bow (which unquestionably requires both hands to operate) in conjunction with the dagger. Specialists with more than 2 arms may be able to wield a bow with a melee weapon at the Keeper’s discretion. In order to use components with a melee and a ranged weapon, a Specialist requires degrees in Double Threat equal to or greater than the prospective components. For example, a Specialist wishing to use Trip (basic) with a crossbow and a dagger, the Specialist would require at least basic training in the crossbow, basic training in the dagger and basic training in Double Threat.

# Berserking

Specialists may ingest an addictive, toxic drug called “Heift” to enter a berserker rage. The chemical gives temporary benefits, but also has drawbacks, such as withdrawals when the drug isn’t taken, a stupor state when the drug wears off, and possibly even death if too much is taken.

### Taking Heift
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Taking doses of Heift costs 1 AP per dose, as the substance comes in thick, sticky nuggets or cubes. If a Specialist takes a number of doses greater than their Endurance Score divided by 10, rounded down, the dose is lethal. A lethal dose increases the bonuses from the berserker rage state, but automatically ends with the Specialist’s “blood death”, as the acidity of the toxin in their veins melts out through their skin.

 Taking Heift puts the Specialist into a berserker rage the turn after it is taken. The immediate effects of taking Heift are bonus Vitality points and bonus AP. The amount of bonus Vitality points the Specialist gains is equal to their Endurance Score times the number of doses they took. For example, a Specialist with 23 Endurance who takes 2 doses would gain 46 Vitality points for the duration of the drug’s effect, which ends the round after the last AP gained from the drug is spent, at which point their stupor begins. The number of bonus AP a Specialist gains is equal to the number of doses they took times 5. Continuing with the previous example, the Specialist who took 2 doses would gain 10 AP. These AP may be spent in addition to the AP per turn the Specialist gains from their Speed Rating.

### Berserk State
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

While in the Berserk state, Specialists are not capable of the patience or focus is takes to make complicated mental maneuvers such as spells or wielding projectile weapons. For this reason, ranged attacks a Specialist makes while in a Berserk state may only be made with thrown weapons. In addition, on their action, they may only take additional doses of Heift or use the following martial components:


| Simple | Basic | Intermediate | Advanced | Master |
| --- | --- | --- | --- | --- |
| Desperation | Aggressive | Cheap Shot | Charge | Overwhelm |
| Distance | Quick | Dual | Hook Shield | Pierce |
| Simple Attack |  | Mobile |  | Scatter Shot |
| Wrestle |  | Pushback |  | Whirlwind |
|  |  | Stun |  |  |


A Specialist must spend a number of these bonus points each round at least equal to the number of doses taken. Again, using the previous example, the Specialist who took 2 doses of Heift would have to spend at least 2 of his 10 bonus AP each round. Taking subsequent doses increases the remaining bonus AP as well as the minimum AP to be spent per round, in addition to more bonus Vitality points. If the Specialist in the previous example took another dose 2 rounds after their first doses, they would gain another 5 AP to be added to their remaining bonus AP, if any, and now must spend 3 AP per round until the drug wears off. If the Specialist has fewer bonus AP than the requisite number, they simply spend all remaining points. The Specialist in this example would also gain another 23 bonus Vitality points, to be added to any remaining bonus Vitality points left from the first 2 doses. For this Specialist, a third dose also becomes a lethal dose, meaning they die immediately after their stupor ends.

### Stupor
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

When the berserk state ends, a Specialist who has taken doses of Heift goes into a stupor. During the stupor, the Specialist gains negative AP counters equal to the doses they took times 10. For example, if a Specialist took 2 doses of Heift, they would gain 20 negative AP counters as soon as they use the last of the bonus AP from the rage. For each round in which the Specialist has negative AP counters, they must spend a minimum of 1 AP to negate a negative AP counter, though they may spend up to all their AP per round.

If, at any point during the stupor, the Specialist takes additional doses of Heift, they gain additional benefits as normal. This increases the effective dose as appropriate as well. Following the previous example, if a Specialist had taken 2 doses of Heift and entered the stupor, then took another dose, all effective values are calculated as though the Specialist had taken 3 doses of Heift. Thus, they would still need to spend a minimum of 3 AP per round, and if 3 doses is lethal, the Specialist would still die immediately after their stupor ends. At the end of the renewed rage, the Specialist would gain the full number of negative AP counters for 3 doses, regardless of how many counters had previously been negated. Thus, in the given example, the Specialist would gain 30 negative AP counters, regardless of how many they had negated in their previous stupor.

### Lethal Dose
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

If a Specialist takes a lethal dose, they lose the ability to distinguish friend from foe as hallucinations overcome their senses. Such a Specialist has equal chances of hitting any creature or Specialist within range. In this case, the Specialist should determine their attack and roll to hit before determining the target. On a successful hit, the Specialist rolls damage as normal.

A lethal dose always ends with the “blood death” of the Specialist. No amount of healing or temporary hit points prevents it. A Specialist who takes a lethal dose may later be resurrected via the use of a Life spell. In such a case, any withdrawal symptoms don’t begin until 24 hours after resurrection, if the Specialist doesn’t take any further doses.

### Addiction
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

A Specialist who has taken Heift, and fails to continue taking it begins to experience withdrawal symptoms 24 hours after their last dose. These withdrawal symptoms come in stages, starting with physical pain, followed by hallucinations and finally potential death. A Specialist may take a dose at any time to alleviate the withdrawal symptoms.

Any Specialist who has ever taken Heift gains an addiction level. The addiction level of a Specialist is equal to the highest number of doses the Specialist has ever taken at one time. For example, a Specialist who has taken 4 doses of Heift at one time, and has never taken more than that at one time, would have an addiction level of 4, even if 4 doses was a lethal dose.

### Withdrawal
> **Status:** ⚠️ REVIEW / CONVERSION — component/training concept recovered. Static caps, summed values, mitigation references, negative AP, old defense sequencing, or legacy AP math must not be assumed current without review.

Withdrawal symptoms last for a number of weeks equal the Specialist’s addiction level. For example, if the Specialist’s addiction level is 4, their withdrawal symptoms would last 4 weeks.

The first stage of withdrawal symptoms is the physical pain stage. For the entirety of the withdrawal period, any time a Specialist attempts to take actions which require the use of AP, such as a round of combat, the Specialist must succeed on an Endurance Reaction or lose AP equal to the Specialist’s addiction level. The save difficulty is equal their addiction level multiplied by five. For example, if the Specialist has taken 3 doses, their save difficulty would be 15.

The second stage of withdrawal symptoms is the hallucination stage. This stage begins after a number of days equal to the Specialist’s addiction level multiplied by 3. For example, a Specialist with an addiction level of 3 would begin this stage after 9 days. For the remainder of the withdrawal period, the Specialist must now make an Intelligence Reaction against hallucination any time a potentially stressful event occurs. The difficulty of this reaction is equal to 4 time the Specialist’s addiction level. For example, a Specialist with an addiction level of 3 would have a difficulty of 12. Upon failing a save, the Specialist becomes aggressive for a number of rounds equal to their addiction level, and begin attacking anything and everything within range as hallucinations overwhelm their senses. For each round of this aggression, the Specialist will attack the nearest target, whether friend or foe. Roll randomly if more than one target are equal distance. These Intelligence Reaction rolls are in addition to (or can be potentially caused by) the pain saves.

The final stage of withdrawal symptoms is the dying stage. This stage begins after a number of days equal to the Specialist’s addiction level multiplied by 6. For example, a Specialist with an addiction level of 3 would begin this stage after 18 days. During this stage, a Specialist must make Endurance Reaction rolls versus death every 12 hours. The reaction difficulty is equal to the Specialist’s addiction level times 3. For example, a Specialist with an addiction level of 3 must make a reaction with a difficulty of 9. On a failed reaction, the Specialist’s body simply gives out, and they die. During this stage, the Specialist must still make pain and hallucination reactions as normal.

If a Specialist manages to survive their withdrawal period, they are still addicted to Heift, and continue to have an addiction level, though they no longer suffer withdrawal symptoms until such time as they take another dose. A Specialist who has survived the withdrawal is still an addict, albeit a reformed addict.


---

# Chapter 6 — Magic

## Reconstruction status legend

- **✅ CONFIRMED** — established by later explicit decisions and treated as current canon unless deliberately reopened.
- **🔄 SUPERSEDED** — recovered source material that has been replaced by a later decision.
- **⚠️ REVIEW / CONVERSION** — concept or content is useful, but one or more mechanics must be reconciled with the current engine.
- **⬜ NEEDS DEVELOPMENT** — incomplete or absent; substantial design work remains.
- **❗ CONTRADICTION** — two surviving sources or decisions conflict and must not be silently reconciled.
- **💡 SUGGESTION** — design suggestion from this reconstruction pass; not canon unless Mike approves it.

**Authority used in this reconstruction:** newest explicit decisions in the current reconstruction work override older text; CLEAN source files are the baseline for material not subsequently changed. Archival Markdown is treated as a searchable transcription of its CLEAN source, not as independent canon. No discrepancy has been silently fixed.

## 1. Current Magic architecture

**✅ CONFIRMED**

Magic uses the same success-counting d10 engine as Martial and Skills. It does not use a parallel resolution system.

The universal **Critical Die** applies to qualifying Magic resolution rolls: a successful action with a natural 10 on its Critical Die is Crit+; a failed action with a natural 1 on its Critical Die is Crit-. Specific spell or subsystem effects still require their own converted rules.

A spell is assembled from **Energy + Structure (+ optional/modifying Components)**. CLEAN expresses Structure through Target, Duration, Shape, and Optional elements; the exact final vocabulary should be preserved unless an entry is deliberately renamed.

The highest-tier Energy/Structure/Component involved determines the spell's tier for prerequisites and AP ceiling. Modern action ceilings are 3/6/9/12/15.

## 2. Casting Stat and tier prerequisites

**✅ Later primary-Magic Stats:** Charisma / Intelligence / Insight.

**✅ Prerequisites:** 15 / 30 / 45 / 60 / 75 for Simple through Master.

**⚠️ REVIEW:** individual Energies/Structures may call on specific Stats, Skills, or defenses. Those specific interactions survive only after conversion to the modern resolution engine.

## 3. AP, casting time, and multi-turn casting

**✅ Modern rule:** a normal spell/action must be fully paid for using AP available in the current turn. AP does not normally accumulate across turns.

**🔄 CLEAN multi-round casting using negative AP counters is superseded as a default rule.**

**✅ Explicit exceptions are allowed:** a specific Magic Component may permit AP expenditure across turns. This preserves a meaningful special capability without making multi-turn accumulation universal.

**✅ Maintenance is separate:** AP spent on later turns to maintain an effect that has already been enacted is not multi-turn enactment.

**⚠️ Concentration:** remains a maintenance mechanic candidate; CLEAN's escalating 1/2/3... AP schedule should not be assumed final without testing.

## 4. Charged, Conducted, Bestowed

**✅ / ⚠️ Current decisions**

- **Charged:** enacted effect can be held until resolved or dismissed.
- **Conducted:** held through a nonstationary object; losing contact dissipates it. If the object's own melee attack is the delivery vehicle, resolve as a Martial+Magic hybrid; otherwise it behaves like touch-style delivery.
- **Bestowed:** effect is transferred/persists on the carrier; energy/structure remain fixed. The carrier may use the resulting effect according to the Bestowed rules.
- Current working trigger for Conducted/Bestowed attack delivery: **hit or Glancing Blow triggers; miss does not.**

## 5. Counterspelling

**⚠️ REVIEW / REBUILD**

CLEAN contains two broad ideas: counter with an opposing Energy attack or counter with an opposing Energy shield. The concepts are worth preserving, but the exact mechanics are tied to the old attack/defense and mitigation flow.

## 6. Workbook-derived Structure index — formulas intentionally ignored

The source workbook contains extensive calculators. Per explicit instruction, the formulas are **not** treated as rules authority. The following names/tier placements are retained as content evidence:

- **Single/Defined** — Simple
- **Group** — Intermediate
- **Selective** — Master
- **Instantaneous** — Simple
- **Building** — Basic
- **Diminishing** — Intermediate
- **Extended** — Advanced
- **Intensifying** — Master
- **Touch** — Simple
- **Thrown** — Simple
- **Projected** — Simple
- **Ray** — Basic
- **Line** — Basic
- **Spread** — Basic
- **Burst** — Intermediate
- **Emanation** — Intermediate
- **Fog** — Intermediate
- **Mist** — Advanced
- **Cloud** — Advanced
- **Wall** — Advanced
- **Sphere** — Master
- **Ball** — Master
- **Sculpted** — Master
- **Charged** — Simple
- **Delayed** — Simple
- **Worn** — Basic
- **Conducted** — Basic
- **Activated** — Intermediate
- **Arcing** — Intermediate
- **Concentration** — Advanced
- **Bestowed** — Advanced
- **Seeking** — Master
- **Controlled** — Master
- **Mobile Concentration** — Master

## 7. Workbook-derived Energy index — formulas intentionally ignored

The workbook's Energy lookup/mapping contains the following named entries. This is an index only; use the detailed CLEAN Magic descriptions below for actual recovered behavior.

### Elemental

Air, Electricity, Dark, Light, Negative, Positive, Cold, Fire, Water, Acid, Earth, Spirit, Death, Life
### Tiered

Animate I, Charm I, Dispel I, Divination I, Fabricate I, Illusion I, Teleport I, Explode I, Force I, Implode I, Merge I, Protection I, Repulsion I, Thought I, Dispel II, Divination II, Flight I, Mutation I, Precognition I, Teleport II, Temporal I, Animate II, Charm II, Enhancement I, Hinder I, Possession I, Spatial I, Dispel III, Divination III, Explode II, Force II, Implode II, Merge II, Teleport III, Temporal II, Thought II, Decay I, Fabricate II, Flight II, Illusion II, Mutation II, Protection II, Repulsion II, Animate III, Dispel IV, Divination IV, Sound I, Teleport IV, Temporal III, Decay II, Explode III, Force III, Implode III, Merge III, Possession II, Precognition II, Teleport V, Thought III, Animate IV, Dispel V, Divination V, Sound II, Teleport VI, Temporal IV, Decay III, Fabricate III, Flight III, Illusion III, Mutation III, Protection III, Repulsion III, Dispel VI, Divination VI, Explode IV, Force IV, Implode IV, Merge IV, Teleport VII, Temporal V, Thought IV, Animate V, Charm III, Enhancement II, Hinder II, Possession III, Spatial II, Dispel VII, Divination VII, Flight IV, Mutation IV, Precognition III, Teleport VIII, Temporal VI, Explode V, Force V, Implode V, Merge V, Protection IV, Repulsion IV, Thought V, Animate VI, Charm IV, Divination VIII, Fabricate IV, Illusion IV, Teleport IX, Temporal VII
### Primal

Slick, Stick, Drain, Siphon, Disease, Boon, Curse, Destabilization, Manipulate, Poison, Disintegrate, Gravity

## 8. Complete recovered Magic catalog

The catalog below is intentionally exhaustive. Exact AP, potency, target counts, area, duration, static numbers, alternate defenses, old damage formulas, and old multi-round mechanics are **not automatically current**. Each entry is kept so we can convert rather than reinvent.

---

# Magic

Magic is the heart and soul of fantasy; the stuff dreams are made of. When implementing magic in a fantasy world, there are some important questions to ask: How does magic work? Is it ritualistic and formulaic? Does it involve long hours studying musty old tomes under the tutelage of a decrepit old guy with a long, flowing, white beard?

Let’s take a look at some of these questions. For the sake of game mechanics, many games have pre-packaged spells, and a variety of ways to learn them. Some people have a natural talent for magic. Some do study and learn from white bearded wizards. In Boundless, magic works quite differently. Magic is the ability to manipulate energy. For example: fire is energy. Whether it’s larger or smaller, it’s still fire. Magic allows a person to increase or decrease the size and intensity of the fire. Whether through force of will, deep understanding, or purposeful study, some individuals are able to generate, shape, and control energies.

# Building and Casting Spells

Spells in Boundless are essentially unique. Casters have the ability to shape energies they know into various structures on the fly. Some casters like to keep track of spells they’ve used before, so they can be used again with little preparation time involved. We recommend casters keep at least a few such spells available for use in combat, to prevent combat from being slowed down each time a spell is cast.

## Building a Spell

Creating a spell involves 2 parts; the energy/energies to be manipulated, and the delivery method, or structure of the spell. The energy or energies of a spell are chosen from Elemental, Primal, and Tiered energy types. Once the energy has been chosen, the structure must be created. The structure consists of target, duration, and shape. There are also optional structure components available.

## Casting a Spell

Once a spell has been built, it’s ready to be cast. Spell casting may be subject to various restrictions, such as casting time. Prepared spells may also be dropped, or altered based on the needs of the caster.

### Spell Difficulty
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

The spell difficulty of a spell is the same as the highest tier energy or structure Magic component used in the spell. For example, a spell with a Basic energy or structure and a Master energy or structure is considered a Master difficulty spell. A spell is never considered to be higher than Master level difficulty, though it may cost more than 5 AP to cast.

If a spell is combined with a martial component, the spell difficulty does not change. For example, a Basic difficulty spell combined with an Advanced martial component would still be considered a Basic difficulty spell.

### Spell AP Cost
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

The total AP cost of a spell is equal to the cost of the base spell plus the AP cost of each additional optional energy or structure. A base spell consists of a single energy and required structures (target, duration and shape). The AP cost for the base spell is based on the highest tier component used. Simple costs 1 AP, Basic costs 2 AP, Intermediate costs 3 AP, Advanced costs 4 AP and Master costs 5 AP. For example, an Intermediate spell would cost 3 AP to cast. Adding a Basic optional energy or structure component would increase the spell’s AP cost by 2. Thus, an Intermediate spell with a Basic optional component would cost 5 AP to cast. Adding a Simple energy to this spell would increase the AP cost by 1 for a total of 6 AP.

### Casting Time
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Casting spells occurs in two parts. The first part is forming the spell, and the second part is actually casting it. Forming a spell happens at the speed of thought, and takes up no time in game. Casting the spell is a function of AP expenditure. If a Specialist has enough AP in a given round to cast the spell, they may do so on that round. If the spell costs more AP than they have in that round, they may empower the spell over multiple rounds.


### Multi-round Casting
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Spells may be formed that require more AP than a Specialist has in a round. Upon beginning such a spell, the Specialist gains negative AP counters equal to the AP cost of the overall spell. Each round, the Specialist must spend AP on it to maintain focus (at least 1 AP, or up to their full round’s AP). Failure to focus on the spell cancels the casting. Once all negative AP counters for the spell are removed, the spell is cast. Any status effect which prevents a Specialist from spending AP causes an automatic failure to focus. A Specialist attempting to focus on a spell who takes damage or is subject to other potentially distracting factors (such as loud explosions or blinding flashes) must succeed at a Focus Save to maintain focus using their primary casting stat. The difficulty of the focus save is equal to the amount of any damage the Specialist takes plus the AP cost of the overall spell. For example, if the Specialist is casting a spell that costs 6 AP and that specialist takes 10 damage, they must succeed on a difficulty 16 focus save.

### Altering Prepared Spells
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Any prepared spell may be instantly exchanged for any equal or lower tier energy known to the defender for the purpose of countering an incoming spell. Only the energy type is changed. Optional components and structure elements remain the same.

Energies in spells with multiple energy types are exchanged individually. For example, a spell with energies A and B could be exchanged to energies A and C, B and C, or even C and D, so long as the energies being exchanged are of equal or lower tier.

# Simple Components

Simple energies are the lowest hanging fruit, so to speak. When Specialists begin to learn magic energies, they learn the simple energies first. A Specialist must have at least 15 points in their primary casting stat to cast simple spells.

## Energy

### Air (Elemental):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Air energy controls the flow of air. An Air spell can increase or decrease the density of air in a certain space, or can generate fresh, breathable air from nothing. When used to control the flow of air, each AP spent increases or decreases the speed of the wind by 5MPH. When used to generate breathable air, each AP generates 1 minute of breathable air, appropriately sized for the caster. If used as an attack against a target, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. Targets are allowed an opposed toughness check to prevent being pushed back or knocked over.

### Animation 1 (Tiered – Wild):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Wild animation energy causes otherwise inanimate objects to move. The caster can give them the semblance of 1 basic emotion, expressed solely through action. The object may appear happy, sad, annoyed, agitated, etc. An object never explicitly attacks, though a sharp object flailing about in an agitated manner may inadvertently attack any that approach too close, at the Keeper’s discretion. Each AP of Wild Animation is sufficient to animate an object up to 1 cubic foot. Anyone wearing or holding the target object may make a ward check to resist the Animation spell.

### Charm 1 (Tiered – Sleep):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Sleep Charm energy triggers the body’s natural response of being tired. Instead of directly dealing damage to a target, a Sleep Charm spell directly attacks the target’s Fatigue pool. Sleep Charm energy is only effective against living targets. Even instantaneous Sleep spells cause biochemical changes in the target, and last until the target gets an appropriate amount of rest.

### Dark (Elemental):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Dark energy decreases the level of illumination in an area. Dark energy can provide relief from direct sun by providing magical shade, or can rob some creatures of their ability to see by creating pitch blackness. Dark energy is suitable to counter Light spells. A single AP of Dark energy is sufficient to counter the light of a torch (or any smaller light, such as a candle) within the area of the spell. To counter the light of a campfire would require 3 AP. To counter the light of an overcast day would require 5 AP, and to counter the light of a sunny day in the middle of summer would require 10 AP.

Dark energy, in and of itself, is harmless and allows for no defense.

### Dispel 1 (Tiered – Single):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Single Dispelling energy nullifies 1 ongoing magic effect on the target creature or object, chosen at random. A Single Dispel spell used on an object with 3 spells active on it would nullify 1 of the effects, chosen randomly at the Keeper’s discretion. A target that happens to be in the area of an ongoing spell does not count as an object with an active spell on it, but the anchor or target of a spell whose duration is longer than instantaneous does count. When used to dispel an activated spell that would otherwise be triggered by casting this spell, the dispel resolves first, and nullifies the activated spell. For example, if a rock has an extended Light spell, a delayed Fire Burst spell, and an activated Electricity Ball with a trigger of “activated by the first person who touches the rock”, a caster who casts a touch shaped Single Dispel on the rock may not suffer the effects of the activated Electricity Ball. When the caster touches the rock with the dispelling energy, the Keeper determines which of the 3 spells in effect is nullified. If the Electricity Ball is dispelled, it is nullified before it has a chance to be triggered. If, on the other hand, the Keeper determines that the Fire Burst or Light spell is dispelled, the Electricity Ball is activated immediately. The appropriate spell is still nullified, but the caster is subject to the effects of the Electricity Ball. A Single Dispelling energy spell must have at least as many AP as the strongest spell currently in effect on the target, or the dispelling simply fails. Unless a Specialist knows the AP levels of the spells on an object, they have to simply guess at the strongest spell and hope they spend enough AP to dispel an effect.

### Dispel 2 (Tiered – Multiple):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Multiple Dispel energy dispels more than 1 ongoing magic effect. The minimum number of AP required to dispel multiple effects is equal to the AP of the strongest spell currently in effect on the target, multiplied by the number of spells the caster wishes to dispel. For example, if a rock has an extended, 5 AP, Light spell, a delayed, 3 AP, Fire Burst spell, and an activated, 3 AP, Electricity Ball with a trigger of “activated by the first person who touches the rock”, a caster wanting to dispel 2 of the spells would need at least 10 AP of Multiple Dispelling energy; 5, since the strongest spell in effect is 5 AP, multiplied by 2, since the caster wishes to dispel 2 spells (5*2 = 10). To dispel all spells on the aforementioned target with 1 casting, the caster would need to cast a multiple dispelling spell with at least 15 AP.

### Divination 1 (Tiered – Known, Aided, Visual):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Known, Aided, Visual Divination allows the caster to spy on a known target, and receive visual input only, with the aid of a reflective surface. This spell turns any mirror, puddle, or crystal ball into a window to distant events. The caster can see events up to a mile away per AP spent, but gets no other sensory input. Targets get an automatic ward check against this spell.

### Divination 2 (Tiered – Known, Aided):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Known, Aided Divination allows the caster to spy on a known target, and receive visual and audial input with the aid of a reflective surface. This spell turns any mirror, puddle, or crystal ball into a window to distant events. The caster can see and hear events up to a mile away per AP spent, but gets no other sensory input. Targets get an automatic ward check against this spell.

### Electricity (Elemental):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Reduce, Negate, Rebound, Absorb

Electric energy is volatile, white hot, and conducts easily through anything wet or metallic. Electricity can jolt the muscles and central nervous system of living targets. Electricity energy can be used to stun targets or deal lethal damage. When used to stun, targets gain 1 negative AP per AP spent on the spell. When used lethally, targets take 1d10 Vitality damage for each AP spent on the spell.

Your Keeper may allow electricity to be conducted through water, metal, or other appropriate materials without having to pay the additional cost of a conducted spell. In such a case, each movement unit of metal or water, sized appropriately for the caster, should reduce the negative AP gained by 1 or the damage a target takes by 1d10. For example, if a 3 foot tall Specialist casts a 5 AP Electric energy spell on the surface of a body of water and there is a creature 9 feet (3 MU, based on the caster’s size) from the spell’s target, the creature would take 2d10 damage instead of the full 5d10.

### Explosion 1(Tiered – Object):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Object exploding energy causes inanimate objects to burst apart as shrapnel. When this spell is cast, roll for damage as normal. If the damage is insufficient to overcome the structural integrity of the object, the spell fails. If the damage is sufficient to overcome the structural integrity of the object, it bursts apart violently and sends shrapnel nearby. Shrapnel travels in a diameter of 1 movement unit, appropriately sized for the caster, for each cubic foot of the object. Shrapnel from soft objects exploding impacts nearby creatures and objects, but only has a chance of harming very fragile targets. Hard objects exploding send sharp, jagged shrapnel at nearby targets. In this case the caster makes a single ranged attack roll, and each nearby target defends against the attack roll. Any targets hit by the shrapnel take half the damage originally rolled for the target of the Explosion spell. Anyone wearing or holding the target object may make a ward check to resist the Explosion spell.

### Fabrication 1 (Tiered – Repair):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None, Prohibitive

Repair Fabrication energy can mend broken, ripped, torn, or otherwise damaged goods. In order to repair an object, all the pieces of the object must be together when the spell is cast. If any part of the original object is missing, the spell fails. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. The caster can repair up to 1 cubic foot of materials per AP of Repair Fabrication energy, restoring the object’s structural integrity by an amount equal to the strength of the spell, up to the object’s natural maximum structural integrity. Anyone wearing or holding the target object may make a ward check to resist the Repair Fabrication spell.

### Flight 1 (Tiered – Slow Fall):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Slow Fall Flight energy reduces the momentum of a target, which reduces the effective fall height. Each AP of Slow Fall Flight energy reduces the effective fall height by 1 movement units, appropriately sized for the caster, regardless of the duration of the spell. Even an instantaneous Slow Fall Flight spell reduces the effective fall height. A small creature casting a spell using this energy on a larger target would need more AP to reduce the damage of a fall from a similar height. Slow Fall Flight increases the fall time for creatures by 1 action for each cumulative 30 feet of fall distance. For example, if a creature slow-falls 90 feet, instead of taking 2 actions to fall (30 feet the first action and 60 feet the second action), the fall time would take 4 actions. Slow Fall Flight energy doesn’t need duration to reduce the damage from a single fall, regardless of how long that fall takes. If the spell does have duration longer than 1 action, the target enjoys the benefit of the spell for any falling action that takes place within the spell’s duration, such as bounding down tiers of short cliffs. Even if the duration of a Slow Fall Flight spell expires while a creature is falling, the creature falls slowly to the ground as though still under the effects of the spell. This spell reduces the effective fall height of all falling actions of the target by the same height for the duration. Thus, if the target falls a distance farther than the effective height reduction granted by this spell, the target still takes damage as normal for the extra distance.

### Force 1 (Tiered – Wave):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Wave Force energy hits targets like a sudden, strong breeze. Targets hit by a wave of Force must succeed at a Toughness check, or be halted, pushed back, or knocked prone. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. Any creatures caught in the area must make a Toughness check. Creatures with Toughness checks that meet or exceed the strength of the spell are unaffected. Creatures that fail to meet or exceed the spell’s strength are halted if moving, or pushed back 1 movement unit per AP, appropriately sized for the caster, if stationary. Creatures with Toughness checks lower than half the spell’s strength are knocked prone. Unattended objects weighing less than the strength of the spell are pushed 1 movement unit, appropriately sized for the caster, by the spell.

### Illusion 1 (Tiered – Physical):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Physical Illusions change the appearance of an existing, physical object in some way. A Physical Illusion spell can change the color of an object, make an object appear to be made of gold, or even make a creature appear to be another race, though the illusion doesn’t change the size of the creature. Physical illusions are purely superficial. Onlookers have a chance to see through physical illusions. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. Onlookers with Intelligence or Insight scores of 10 or more automatically get to roll a check related to the higher of the 2 stats to disbelieve the illusion. Any onlookers who see the Physical Illusion spell being cast, and who have both Intelligence and Insight scores of 10 or more get to roll 1 check each for Intelligence and Insight. Anybody who physically interacts with an object that is obviously made of a different material than the illusion shows, for example a wooden object appearing to be made of gold, automatically gets to roll a disbelief check with a bonus of 5d10 on their roll. The duration of a Physical Illusion spell is measured in minutes. Each AP of Physical Illusion is sufficient to change the appearance of up to 1 cubic foot of materials.

### Implode 1 (Tiered – Object):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Object Imploding energy crushes inanimate targets violently. When this spell is cast, roll for damage as normal. If the damage is insufficient to overcome the object’s structural integrity, the spell fails. If the damage is sufficient to overcome the structural integrity, it collapses into a ball 1/100th the size of the original object. The implosion of very large objects can create a minor vacuum in the surrounding area, pulling light objects toward it, but creating barely more than a cool breeze for anything weighing more than a pound. Anyone wearing or holding the target object may make a ward check to resist the Implosion spell.

### Light (Elemental):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Light energy increases the level of illumination in an area. Light energy can help people see better in dark areas. Light energy is suitable to counter Dark spells. A single AP of Light energy is sufficient to create light equivalent to a torch (or any smaller light, such as a candle) within the area of the spell. To create the light of a campfire would require 3 AP. To create the light of an overcast day would require 5 AP, and to create the light of a sunny day in the middle of summer would require 10 AP.

Light energy, in and of itself, is harmless and allows for no defense.

### Merge 1 (Tiered – Object):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Merging energy combines targets. Only willing targets can be combined, and any Merge spell attempted on an unwilling target simply fails. Mindless creatures, and creatures of animal intelligence are never considered willing targets, unless they’re being controlled, in which case the controller must be willing. Higher tiers of Merge energy allow a wider variety of targets to be merged, eventually allowing normal, living creatures to be affected. Any target may be combined with other targets from lower tiers as well. For example, a Living Merging spell can merge a living target with an object. In any Merge spell, the largest target to be combined is considered the base of the resulting object or creature. Creatures merged into stationary targets maintain their senses, though they may be unable to move for the duration of the spell. For example, a caster that merges with a large boulder to hide from a goblin raiding party would still be able to see and hear as normal from within the boulder. While merged with the boulder, the caster is immune to damage, so long as part of the boulder remains larger than the caster’s natural size. If the boulder explodes, or is crushed, however, and no piece larger than the caster’s natural size remains, the caster is killed, and her corpse is left in pieces no larger than the largest remaining piece of the boulder.

Object Merging energy combines 2 non-stationary objects into one. For example, an axe could be combined with a maul to create a splitting maul. When casting this spell, the caster must declare the desired result. If the Keeper rules the result is not possible, the caster may opt not to cast the spell. Objects to be combined must be touching when the spell is cast. Each AP of Object Merging energy is sufficient to combine up to 1 cubic foot of objects. Any number of objects may be combined so long as they are all touching at least 1 other object to be combined, and the combined total of the objects remains 1 cubic foot or less per AP of the spell.

### Mutation 1 (Tiered – Resize):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Resize Mutation energy increases or decreases the size of the target. When casting a Resizing Mutation spell on a creature, the creature’s original size is always the basis for calculating AP needed, even if its size has already been altered. Increasing or decreasing a target costs 1 AP per foot of change. When a creature is resized, all its gear is resized with it. The creature’s weight also increases or decreases accordingly. To determine the creature’s new weight, round their original height to the nearest foot and divide their original weight by this number. Add the result for each foot added or subtract the result for each foot reduced. The duration of Resize Mutation energy spells is measured in hours.

### Negative (Elemental):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Reduce, Negate, Rebound, Absorb

Negative energy directly attacks the vitality of living targets, or replenishes the animus of undead targets. Negative energy does nothing to targets that are neither living nor undead. Negative energy is suitable to counter Positive energy spells.

### Positive (Elemental):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Reduce, Negate, Rebound, Absorb

Positive energy directly replenishes vitality of living targets, or attacks animus of undead targets. Positive energy does nothing to targets that are neither living nor undead. Positive energy is suitable to counter Negative energy spells.

### Precognition 1 (Tiered – Feeling):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Feeling Precognition energy is a very basic form of knowing the future in advance. To cast a Feeling Precognition spell, the caster must concentrate on a specific possible action while casting the spell. Once the spell is completed, the caster gets a gut feeling about the topic at hand. For example, if the caster wants to know if it’s a good idea to open a hidden door, the caster may get the feeling of butterflies in her stomach. Ultimately, it’s up to the player to interpret the feeling the caster gets, as described by the Keeper. The Keeper should strive to handle this spell with vaguely positive or negative feelings when resolving this spell. For example, “you feel your heart pounding”, or “you can’t help but smile” are good vague feelings, whereas “you feel an overwhelming sense of dread” is far too specific and definitive. The Keeper may also rule that a higher AP spent results in stronger or more definitive feelings.

### Protection 1 (Tiered – Reduce):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Reduce Protection energy reduces damage from other spells. When this spell is cast, the caster chooses an energy type, and rolls damage as normal. Instead of dealing damage directly, the damage rolled sets the protection rating of the spell. This spell reduces damage from damage dealing spells of the chosen energy type by the protection rating, to a minimum of 1 point, for the duration of the spell. For example, if the caster chooses fire energy, and rolls 23 points, this spell protects the target from up to 23 points of fire spell damage whenever the protected creature would otherwise take fire spell damage. If, during the course of this spell, the protected creature is hit with 15 points of fire spell damage, the protected creature only takes 1 point of damage. If the protected creature is then hit with 27 more points of fire spell damage, the protected creature takes 4 points of damage. Reduce Protection energy has no effect on spells that don’t deal damage directly, or damage sources that can’t be warded against, such as a camp fire or burning building.

### Repulsion 1 (Tiered – Natural):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Natural Repulsion gives natural, living creatures an aversion to the target. Repulsed creatures will try to escape the object of their repulsion. If escape is not possible, they will at least keep their distance, and won’t willingly approach, though they may still attack the object of their repulsion at range. If the object of repulsion corners the subject, the subject will invariably lash out and attack. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. If the strength of this spell is greater than the natural maximum vitality of the target, the target is repulsed by this spell.

### Teleportation 1 (Tiered – Projection):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Projecting Teleportation sends the caster’s spirit out of the caster’s body to a specific location. The caster’s spirit leaves the caster’s body and appears at the desired area, and is an incorporeal, nearly invisible ghost for the duration of the spell. Anything that affects incorporeal beings affects the caster’s spirit. Anything that harms incorporeal beings also harms the caster. If the caster dies in ghost form, the caster’s body also dies, though the caster may be resurrected as normal. Once the spell ends, the caster’s spirit returns to the caster’s body, unless it is somehow prevented from doing so, such as being trapped in a solid force energy sphere. Projection Teleportation’s range is measured in 1-mile units. Each AP of Projecting Teleportation energy increases the range the caster can project by another mile.

### Teleportation 2 (Tiered – Visible):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Visible Teleportation energy instantly sends the target to a visible destination within range. The first AP of Visible Teleportation energy is sufficient to Teleport the caster (regardless of the caster’s weight), or another creature or object, weighing no more than 50 lbs, up to 5 movement units, appropriately sized for the caster. Each additional AP of Visible Teleportation energy increases the amount of distance from the caster this spell may send the target by up to 5 movement units, or increases the weight limit by up to 50 additional lbs. Targets may not be Teleported inside physical objects. The destination of this spell doesn’t need to be on the ground. In fact, the target may be Teleported straight into the air, or into any body of water clear enough to see through, within range.

### Temporal 1 (Tiered – Accelerate):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Accelerate Temporal energy speeds up time around the target. This effectively slows the target as the world around it speeds up. When this spell is cast, roll damage as normal. Instead of dealing damage directly, this spell reduces the target’s Speed stat by the amount rolled for the duration of this spell. This spell may not reduce a target’s Speed stat below 1 point. Successive castings of the same spell overlap, though any difference in duration or potency takes effect separately. For example, if a target with a Speed stat of 53 is subject to this spell, and its Speed stat is reduced by 15 points, the target is left with a Speed stat of 38 for the duration. If, during the first spell’s duration, the same target is affected by a second casting of this spell, and the damage rolled is 33, the target’s Speed stat is reduced by a total of 33 from its original 53 Speed stat, leaving it with a Speed stat of 20 for the duration of the second spell. The target’s AP per round is affected accordingly. Accelerating Temporal spells conflict with Decelerating Temporal spells. If both energies are simultaneously in effect on the same target, the target is subject to the difference in strength of the two.

### Thought 1 (Tiered – Project):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Projected Thought energy sends your thoughts into the target’s mind. These thoughts can be harmless, disturbing, or disruptive. Harmless uses of Projected Thought energy include sending a telepathic message to the target. Harmless Projected Thought requires 1 AP for every 10 words the caster wishes to send. Disturbing uses of Projected Thought energy include sending taunting telepathic messages, grotesque images, or mental white noise. Disturbing Projected Thought requires 1 AP for every 10 words of a taunting telepathic message, or every grotesque image. Disruptive use of Projected Thought energy consists of bombarding the target’s mind with all the caster’s brainwaves. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. Targets get to make a Charisma check against the strength of the spell to ignore the disruptive energy. Any target that fails its check loses its focus, and is unable to perform complex actions.

## Structure

### Instantaneous (Duration):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

An instantaneous spell is really a spell that lacks significant duration. It is resolved in a fraction of time so small it’s difficult to perceive. While the energy only lasts an instant, the result of the effect typically lasts long after. For example, an instant of applying fire energy to a volatile substance or a highly flammable material can still result in a longer lasting flame. The same fire energy, if applied to a clay object, will most likely go unnoticed, while applying it to a creature will likely cause the creature pain.

When used with Concentration:

When an Instantaneous spell is used in conjunction with concentration, its effects occur again each round on the caster’s turn until concentration ends. All other structures must stay the same, but location may be changed as long as it remains within the spells range.

### Projected (Shape):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

To project a spell, the caster gathers energy into a small, semisolid, ball-like object. The object appears to be made of the energy used in the spell, and forms roughly the shape of a ping pong ball. Once formed, the object speeds toward its target as though it had been fired from a bow in 4 movement unit increments, appropriately sized for the caster. Resolve the attack as a martial attack, pitting attack versus defense. If the spell hits, determine effects as normal for magic.

### Single/Defined (Target):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Single target spells affect only the first viable target the spell energy comes into contact with. If the spell is used, and no viable target is contacted by the energy (such as a projectile spell that misses its target, and doesn’t hit another viable target), the spell energy simply fizzles, and AP used to cast the spell are still expended.

Defined target spells are spells that have a shape or area, such as a cloud or sphere, and affect any and all viable targets that come into contact with them.

### Thrown (Shape):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

To throw a spell, the caster gathers energy into a semisolid, ball-like object. The object appears to be made of the energy used in the spell, and forms roughly the shape of a baseball. The caster then throws the spell, just as if it were a thrown weapon, in 2 movement unit increments, appropriately sized for the cater. Resolve the attack as a martial attack, pitting attack versus defense. If the spell hits, determine the effect as normal for magic.

### Touch (Shape):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

A Touch shaped spell is really a spell that lacks shape. It actually represents a minute point in space too small to visually perceive, though the effects may be more noticeable. A Touch spell functions much like zapping somebody with static electricity. The charge jumps a small distance, and the recipient feels the effect. Touch spell energies are conducted through, and therefore bypass, shield and armor to affect the target.

## Optional

### Charged:
> **Status:** ✅ CONFIRMED IN PRINCIPLE — the spell may be held after successful enactment until resolved or dismissed; exact timing/AP language still needs final prose.

A charged spell is prepared, and held at the ready. Upon the spell’s completion, the caster gathers the energy used in the spell, which then visibly crackles around the caster indefinitely until released. A charged spell may be resolved as normal or dismissed at the caster’s discretion.

### Delayed:
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Delayed spells are designed to take effect in the future. When casting a delayed spell, the caster chooses the length of the delay. At the end of the delay, the spell takes effect as normal, assuming it hasn’t been dispelled. If the circumstances of the spell cast change in such a way that the spell would no longer be able to be cast at the specified time, the spell effects of the spell instead occur at such a time as the circumstances would once again allow the spell to take place. For example, if a Delayed fire spell is cast with a delay of 1 hour, and within that hour, the area where the spell was targeted becomes flooded, the fire spell will remain delayed until the flood water recedes.

### Shield:
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

To use a spell as a shield, the caster gathers energy into the shape of a shield held in their off-hand, or the off-hand of the target. Shield spells aren’t particularly useful unless they have a duration longer than instantaneous. Shield spells with a duration longer than instantaneous are weightless, and are wielded just like a shield, moving with the caster or target. Shield spells don’t hinder the movement of the wearer. If the shield spell is a damage spell, melee attackers may take the damage any time the caster successfully blocks an attack within the duration of the spell. Treat this as an attack from the wielder of the shield spell against the defense of the initial attacker. Attackers that don’t need to be within a movement unit to attack don’t take damage from a shield damage spell. Force can also be shaped into a shield spell, and acts like a normal shield. In this case, attackers don’t necessarily take damage, but the shield spell provides 2d10 defense and mitigates damage from attacks as appropriate. Shield spells are subject to penalties just like normal shields if the Specialist lacks shield training. If the Specialist does possess shield training, the minimum stat requirement is based on the caster’s Primary Magic stat instead of their Toughness stat. This means the caster needs a 15 to make a small shield, 30 for a medium shield, 45 to make a large shield and 60 to make a tower shield. Additionally, to make a shield of Force energy, the caster needs to know Wave Force (Tier 1) for a small shield, Kinetic Force (Tier 2) for a medium shield, Solid Force (Tier 3) for a large shield and Animated Force (Tier 4) for tower shield.

# Basic

Basic magic energy is a step up from simple energy. Basic energies are slightly more powerful, but still within reach for fairly new casters. A Specialist must have at least 30 points in their primary casting stat to cast basic spells.

## Energy

### Animation 2 (Tiered – Controlled):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Controlled Animated objects follow 1 basic command for the duration of the spell. Controlled animated objects retain their structural integrity, though they become uniformly flexible, and capable of movement. A Controlled Animated object will do everything in its power, in an attempt to follow the command for the duration of the spell. Stationary inanimate objects, such as trees, can only follow the command if they can do so from their stationary positions. Semi-stationary objects, such as statues with feet that are physically attached to a base, will break loose to follow the command. Loose objects move freely, as appropriate for their size to follow the command. A command to follow must be absolutely basic, such as “attack that target”. Complex commands, such as “hold perfectly still until so-and-so is within range, then attack” are too complicated. In such cases, the Keeper will determine which part of the command is followed, such as “hold perfectly still”, or “attack”. Each AP of Controlled Animation is sufficient to animate an object up to 1 cubic foot. Anyone wearing or holding the target object may make a Ward check to resist the Animation spell.

### Charm 2 (Tiered – Captivate):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Captivating Charm energy causes a creature to be fascinated by the caster. A fascinated creature will focus on the caster, but that may not always be a good thing. Enraged fascinated creatures will attack the caster for as long as they remain fascinated and enraged. Calm fascinated creatures will simply drop whatever they’re doing to watch the caster, though they don’t become completely unaware of their surroundings, and still have a sense of self preservation. This means that even a calm target won’t stand idly by and be robbed or killed, and will fight back if attacked. Fascinated creatures that are already engaged in combat will continue fighting. Fascinated combatants won’t pursue foes that withdraw. Thus, if all opponents withdraw from the combatant, she is now considered a calm fascinated target. Fascinated targets already attacking the caster become calm, unless the caster takes any threatening action. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. In order for the target to resist, the target must overcome the strength rolled with a Charisma check.

### Cold (Elemental):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Reduce, Negate, Rebound, Absorb

Cold energy drains the warmth from targets. Cold energy can rob a creature or a fire of its heat, and can even freeze liquids at higher AP. Intense cold can even freeze the blood in a creature’s veins, causing severe damage. Cold energy is suitable to counter fire spells (note that an ignited target may no longer be under the effects of a fire spell). This temperature decrease affects objects and creatures from the outside first, though prolonged exposure can affect internal temperatures. Each AP of cold is sufficient to lower the temperature of a target area by 1d10 degrees.

### Decay 1 (Tiered – Ruin):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Reduce, Negate, Rebound, Absorb, Prohibitive

Ruinous Decay energy causes objects and structures to deteriorate, as if having aged rapidly. Ruinous energy rusts metal, melts glass, warps wood, and weakens stone. Ruinous energy may only be used on inorganic materials, with the exception of dead plant matter, such as wood that has been cut from a tree and turned into boards. The spell fails if it is used on living plants or creatures, undead creatures, corpses, or freshly cut living plant matter. A touch shaped ruin spell used on an object with multiple connected parts works only on the part touched. For example, if used on a chain, it causes the link touched to rust. If used on a suit of plate mail armor, the specific plate, strap, buckle, or piece of fabric touched rusts, hardens, or weakens, as appropriate. Once a target has been subject to Ruinous Decay, it remains ruined, unless some other type of magic is used to undo the ruin. Each AP of Ruinous Decay energy reduces the structural integrity of the target by 1d10 points. This effectively ages the target by roughly 1 year per AP.

### Dispel 3 (Tiered – Total):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Total Dispelling energy dispels all magical effects currently in place on a target. In order to dispel all magical effects, the caster must spend at least as many AP as the strongest spell, multiplied by the number of spells in effect on the target, or the dispelling simply fails.

### Divination 3 (Tiered – Unknown, Aided, Visual):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Unknown, Aided, Visual Divination energy allows the caster to spy on a target matching a description, and receive visual input only, with the aid of a reflective surface. This spell turns any mirror, puddle, or crystal ball into a window to distant events. The caster can see events up to a mile away, but gets no other sensory input. Each AP of Unknown, Aided, Visual Divination energy allows the caster to see an additional mile away. Targets get an automatic Ward check against this spell.

### Enhancement 1 (Tiered – Mental):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Reduce, Negate, Rebound, Absorb

Mental Enhancement energy alters the way the target’s mind works in such a way as to allow better perception for the duration of the spell. The perception granted by mental enhancement can allow a target to see magical energies, understand or read other languages, sense recent events, see in the dark, track by scent, and so on. Each type of perception above and beyond the natural senses of a creature require 2 AP. The first AP grants a fuzzy perception, and the second makes the perception clear. Natural senses that are already fuzzy in nature can be made clear with a single AP of mental enhancement. A Keeper may say that what you’re asking for doesn’t count as a perception at any time. For example, if you want to perceive how a lock works, your specialist may gain full understanding of the inner workings of locks, but that doesn’t necessarily mean that any given lock will be any easier to pick. In general, Enhancement energies are for revealing information that would otherwise be hidden. Bonuses to skill rolls should be restricted to Boon energy spells. Mental Enhancement energy is suitable to counter Mental Hinder energy spells. When used to counter mental hinder spells, robbed senses return in order of touch, sight, hearing, smell, then taste, followed by any inborn perceptions above and beyond the 5 basic senses.

### Explosion 2 (Tiered – Un-living):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Un-living Exploding energy causes un-living objects, such as corpses, stationary targets including statues and walls, or false-living animated creatures to fly apart as shrapnel. When this spell is cast, roll for damage as normal. If the damage is insufficient to overcome the Natural structure of the object, the spell fails. If the damage is sufficient to overcome the Natural structure of the object, it bursts apart violently and sends shrapnel nearby. Shrapnel travels in a diameter of 1 movement unit, appropriately sized for the object, for each cubic foot of the object. Shrapnel from soft objects impacts nearby creatures and objects, but only has a chance of harming very fragile targets. Hard objects exploding send sharp, jagged shrapnel at nearby targets. In this case the caster makes a single ranged attack roll, and each nearby target defends against the attack roll. Any targets hit by the shrapnel take half the damage originally rolled for the target of the explosion spell. Anyone wearing or holding the target object may make a Ward check to resist the explosion spell.

### Fabrication 2 (Tiered – Shape):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Shape Fabrication energy turns raw materials into a rudimentary finished product. For example, a caster can turn steel ingots and leather strips into a basic sword of the appropriate size. The finished product is roughly equivalent to the same product made by a craftsman new to making such an item. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. If the caster is trained to make the item to be shaped, the caster may make an appropriate skill check, up to the strength of this spell, and not to exceed the caster’s normal skill tier. Materials from another object may be used, but must be made unworked by a separate casting of the spell before they can be reworked into a new item. The caster can work up to 1 cubic foot of materials for each AP of Shape Fabrication energy. Anyone wearing or holding the target object or materials may make a Ward check to resist the Shape Fabrication spell.

### Fire (Elemental):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Reduce, Negate, Rebound, Absorb

Fire energy is intense heat, usually appearing as a spark or a flame. Fire energy can be used to heat, burn, singe, scorch, ignite, or even char a target. Highly flammable substances, such as dry leaves or oil, readily ignite with minimal application of Fire energy. Flammable substances that have been ignited deal damage as a normal, non-magical fire. Fire energy is suitable to counter cold and water spells. It is important to note that a fire spell can only be countered when cast, or during the spell’s duration. Even countering a fire spell during its duration may not extinguish targets that have ignited. This temperature increase affects objects and creatures from the outside first, though prolonged exposure can affect the internal temperature. At 130 degrees, readily flammable targets ignite. Each AP of Fire energy increases the temperature of the target by 1d10 degrees.

### Flight 2 (Tiered – Levitate):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Levitating Flight energy makes targets neutrally buoyant in air. A levitated target carries no momentum, and stops immediately if nothing is pushing on it. It can only move when pushed by external forces. A strong wind can push a levitated target, though it does so at 1 movement unit for every 10 miles per hour of the wind. Creatures can push around a levitated target as though they were pushing a feather. Levitated creatures don’t move automatically, though a levitated creature could potentially find a way to propel itself, such as a sail, wings or even flapping its arms really fast (though this is generally more effective if the creature is holding some sort of object that catches wind). Each AP of Levitation energy is sufficient to levitate up to 25 lbs.

### Force 2 (Tiered – Kinetic):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Kinetic Force energy propels targets at high speeds. Objects or creatures propelled by kinetic force fly in a direction of the caster’s choosing. Each AP spent on this spell increases the weight limit by an amount equal to the caster’s Intelligence Score and increases the velocity of the target by enough to propel it 1 full movement unit appropriately sized for the caster. Creatures propelled by this spell take damage automatically, but only if they hit a stationary object such as a wall or another creature. Objects or creatures propelled by this spell take and potentially deal 1d10 points of damage for each AP of the spell. When attempting to hit a secondary target, the caster must make a ranged attack using their Intelligence score to hit the secondary target with the original target of the spell.

### Hinder 1 (Tiered – Mental):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Reduce, Negate, Rebound, Absorb

Mental Hinder energy robs the target of perceptions, starting with magical perceptions, and working its way down to the 5 basic senses. Each AP of this spell counters 1 mental enhancement already in place, until no mental enhancements remain. Once all mental enhancements are gone, any inborn perceptions above and beyond the 5 basic senses are suppressed. The Mental Hinder spell then begins attacking the normal senses in the order of taste, followed by smell, then hearing, and finally sight. The Keeper may allow the sense of touch to be removed as well, though creatures with absolutely no perception face very real dangers. For example, a creature with no perception whatsoever would have no way of knowing if it were submerged under water, and would drown. Magical mental enhancements removed by this spell simply end. The normal senses and any innate senses remain impaired for the duration of this spell, but return on their own immediately after this spell ends. When used to remove mental enhancement perceptions, each 2 AP of Mental Hindering energy removes one existing perception. Normal and inborn senses each take one potential to dull, and another potential to remove. Mental Hinder energy is suitable to counter Mental Enhancement spells.

### Illusion 2 (Tiered – Mental):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Mental Illusion energy is used to create hallucinations for observers. Mental illusions can be frightening, soothing, tricky, or benign. Once created, an illusion acts like the creature or object it is modeled after. If the illusion is entirely unique and not modeled after anything, the caster determines the basic actions of the illusion when the spell is cast. Only a controlled Mental Illusion will change its behavior after the spell has been cast. When casting a Mental Illusion, roll for damage, as normal. Instead of dealing damage, the result of the damage roll determines the strength of the illusion. Mental Illusions may be of any size chosen by the caster. Onlookers with Intelligence or Insight scores of 10 or more automatically get to roll a check related to the higher of the 2 stats to disbelieve the illusion. Any onlookers who see the Mental Illusion spell being cast, and who have both Intelligence and Insight scores of 10 or more get to roll 1 check each for intelligence and insight.  Creatures that physically interact with a Mental Illusion automatically get a disbelief roll with a bonus of 5d10 (unless the illusion is of a ghost or other incorporeal creature). The duration of Mental Illusions is measured in minutes.

### Implosion 2 (Tiered – Un-living):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Un-living Imploding energy violently crushes un-living targets, including corpses, stationary targets such as statues or walls, or up to false living animated targets. When this spell is cast, roll for damage as normal. If the damage is insufficient to overcome the object’s Natural structure, the spell fails. If the damage is sufficient to overcome the object’s Natural structural, it collapses into a ball 1/100th the size of the original object. The implosion of very large objects can create a minor vacuum in the surrounding area, pulling light objects toward it, but creating barely more than a cool breeze for anything weighing more than 1 lb. Anyone wearing or holding the target object may make a Ward check to resist the implosion spell.

### Merge 2 (Tiered – Un-living):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Merging energy combines targets. Only willing targets can be combined, and any merge spell attempted on an unwilling target simply fails. Mindless creatures, and creatures of animal intelligence are never considered willing targets, unless they’re being controlled, in which case the controller must be willing. Higher tiers of Merge energy allow a wider variety of targets to be merged, eventually allowing normal, living creatures to be affected. Any target may be combined with other targets from lower tiers as well. For example, a Living Merging energy spell can merge a living target with an object. In any merge spell, the largest target to be combined is considered the base of the resulting object or creature. Creatures merged into stationary targets maintain their senses, though they may be unable to move for the duration of the spell. For example, a caster that merges with a large boulder to hide from a goblin raiding party would still be able to see and hear as normal from within the boulder. While inside the boulder, the caster is immune to damage, so long as part of the boulder remains larger than the caster’s natural size. If the boulder explodes, or is crushed, however, and no piece larger than the caster’s natural size remains, the caster is killed, and her corpse is left in pieces no larger than the largest remaining piece of the boulder.

Un-living Merging energy combines 2 non-living objects into one. Corpses, stationary objects such as statues or walls, or up to false living animated targets, as well as non-stationary objects may be combined. For example, a corpse could be combined with a statue, to help preserve the body. When casting this spell, the caster must declare the desired result. If the Keeper rules the result is not possible, the caster may opt not to cast the spell. Targets to be combined must be touching when the spell is cast. Each AP of Un-living Merging energy is sufficient to combine up to 1 cubic foot of un-living targets. Any number of objects may be combined so long as they are all touching at least 1 other object to be combined, and the combined total of the objects remains 1 cubic foot or less per AP of the spell.

### Mutation 2 (Tiered – Reshape):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Reshaping Mutation energy removes, changes, or adds physical features to targets. Reshaped targets maintain the same physical properties as the original. Thus a wooden door with an iron handle could be reshaped into a tower shield, but it would still be made of the same wood and iron. A human target could grow wings, but the wings would be bones covered by flaps of skin, similar to bat wings, since humans don’t have feathers. A creature could grow horns, fangs, or claws, but all are of the same material as the original, or other similar features (horns are made of bone for creatures that don’t naturally have horns). Reshaping Mutation energy does not combine targets, though multiple reshaped targets could be combined. For example, several different pieces of metal could be reshaped into gears, and combined into a clockwork machine. All reshaped targets return to their original shape when the spell expires. Each AP of Reshape Mutation energy is sufficient to reshape a single target of up to 1 cubic foot. The duration of mutation spells is measured in hours.

### Possession 1 (Tiered – Swap):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Swapping Possession energy switches the soul of the caster, or another willing possessor designated by the caster, with the soul of a target. Upon spell completion, the possessor and the target make opposed Charisma checks, with the possessor having a bonus equal to the number of AP of Swapping Possession energy spent on the spell. If the possessor wins, the possessor’s spirit and the target’s spirit swap, and each spirit inhabits the other’s body, and has all the gear the new body had before the switch. All physical abilities of the body remain the same, though all mental abilities match those of the spirit in the body. The duration of Swapping Possession energy is measured in hours. The possessor and the target revert to their own bodies when the spell ends. If either body dies while the spell persists, the swap becomes permanent, even if the dead body is later brought back to life. The table below shows which attributes are considered physical, and which are considered mental. A willing target may forego its Charisma check.

Physical Stats: Agility, Endurance, Equipment, Fortitude Pool Ranks, Looks, Physical Racial Traits, Size, Speed, Stamina, Toughness, Vitality Pool Ranks

Mental Stats: Charisma, Insight, Intelligence, Luck Pool, Magic Components, Martial Components, Mental Racial Traits, Proficiencies, Skills, Unspent XP

### Protection 2 (Tiered – Negate):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Negating Protection energy reduces damage and effects from other spells. When this spell is cast, the caster chooses an energy type. On completion, damage is rolled, as normal. Instead of dealing damage, the amount rolled becomes the protection rating. This spell reduces damage from spells of the chosen energy type by the protection rating, potentially to zero points, for the duration of the spell. For example, if the caster chooses Fire energy, and rolls 23 points, this spell protects the target from up to 23 points of fire spell damage whenever the protected creature would otherwise take Fire spell damage. If, during the course of this spell, the protected creature is hit with 15 points of Fire spell damage, the protected creature takes no damage. If the protected creature is then hit with 27 more points of Fire spell damage, the protected creature takes 4 points of damage.

### Repulsion 2 (Tiered – Unnatural):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Unnatural Repulsion gives unnatural, living creatures, such as abominations and aberrations, an aversion to the target. Repulsed creatures will try to escape the object of their repulsion. If escape is not possible, they will at least keep their distance, and won’t willingly approach, though they may still attack the object of their repulsion at range. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. If the strength of this spell is greater than the Endurance Score of the target, the target is repulsed by this spell.

### Slick (Primal):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Slick energy coats an appropriate area in a flammable, slippery, oily substance. Any spark or open flame coming into contact with an area coated by Slick energy causes the area to ignite. Igniting the substance created by Slick energy causes it to lose its slipperiness. A Slick spell whose shape is touch still covers an area equal to 1 movement unit, appropriately sized for the caster. Slick energy is fairly thick, and will cling to vertical and horizontal surfaces alike; even the underside of a horizontal surface. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. Any creatures attempting to move within the affected area must make a Balance skill check. Creatures with Balance skill checks that meet or exceed the strength of the spell are unaffected. Creatures that fail to meet or exceed the score are prevented from moving, but do not fall. Creatures with Balance skill checks lower than half the spell’s strength that attempt to move through the area slip, and fall prone. Creatures in the area that are actively flying or hovering are not subject to slipping, though they could still be doused in Slick energy, and set alight. Slick energy is suitable to counter Sticky spells.

### Sound 1 (Tiered – Generate):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Generate Sound energy creates noise. The noises created by Generate Sound energy are very basic, only varying by pitch, tone, and volume. Sound generating spells are primarily used to cause distraction, drown out other sounds, or disorient creatures, though sound can be generated at the proper pitch to shatter glass or crystal. As a distraction, a quick, moderate sound can be made, similar to the sound of a snapping twig. Drowning out other sounds is accomplished through the extended use of moderately pitched, loud sound. Disorienting creatures can be accomplished with a sharp blast of very loud sound, similar to an explosion. Very loud generated sounds can temporarily or even permanently deafen listeners, at the Keeper’s discretion. To shatter crystal or glass, the caster must be able to, at high volume, match the frequency of resonance of the object to be shattered. Each AP of Generate Sound energy is sufficient to create or increase a sound up to 1d10 decibels. By its very nature, sound energy travels. For every 10 feet away from a spell that has a target, the decibel level decreases by 1.

For area effect spells using sound energy, the sound is contained within the area of the spell. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. Any creatures maintaining spells, performing delicate skills, or performing complex maneuvers within the affected area must make a Focus check. Creatures with Focus checks that meet or exceed the strength of the spell are unaffected. The concentration of creatures whose Focus checks fail to meet or exceed the strength of the spell is broken. Any creature whose Focus check is less than half the strength of the spell is effectively distracted, as their ears begin ringing.

Distracted creatures gain distraction tokens equal to the AP of the spell. Distracted creatures may only take single AP actions of no higher than simple difficulty while distracted. Every action taken removes a distraction token. Distracted creatures may attempt additional Focus checks to beat the strength of the spell at the cost of 1 AP each. If a subsequent Focus check beats the strength of the spell, all remaining distraction tokens are removed.

### Spatial 1 (Tiered – Area):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Area Spatial energy increases or decreases the room available inside a closeable object or structure. The duration of Area Spatial energy spells is measured in hours. Each AP of Area Spatial energy is sufficient to increase or decrease the internal dimensions of a structure or object by up to 1 cubic foot for 1 hour.

### Sticky (Primal):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Sticky energy coats an appropriate area in flammable, adhesive substance. Any spark or open flame coming into contact with an area coated in Sticky energy causes the area to ignite. Igniting the Sticky energy causes it to lose its adhesiveness. A Sticky spell whose shape is Touch still covers an area equal to 1 movement unit, appropriately sized for the caster. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. Any creatures attempting to move within the affected area must make a Toughness check. Creatures with Toughness checks that meet or exceed the strength of the spell are unaffected. Creatures that fail to meet or exceed the score are prevented from moving, but do not fall. Creatures with Toughness checks lower than half the spell’s strength that attempt to move through the area trip, and fall prone. Creatures that have fallen prone on a sticky surface must succeed at an Escape skill or Toughness check of double the strength of the spell to stand back up. Creatures in the area that are actively flying or hovering are not subject to sticking, though they could still be covered in Sticky energy, and set alight. Sticky energy is suitable to counter Slick spells.

### Teleportation 3 (Tiered – Transpose):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Transposing Teleportation energy causes 2 or more targets to change places. Transposing Teleportation energy works on any viable living or non-living target within range. The first AP of Transposing Teleportation energy is sufficient to switch the caster’s place (regardless of weight) with 1 target weighing no more than 100 lbs., or 2 other targets, the total weight of which can be no more than 100 lbs. Each additional AP increases the maximum weight of targets that can be transposed by 20 lbs. The caster of this spell counts as weightless for determining weight limits. If this spell is successfully cast on more than 2 targets, no target ends up in the same place it started, though which targets go where are determined at random by the Keeper. No target of this spell may end up in an area too small to physically contain it in the posture it is in when this spell is cast. For example, a 5-foot-tall target, standing when this spell is cast, may not end up in a cage that is only 3 feet tall. Attempting to cast this spell to put a target where it won’t fit causes this spell to fail, and the AP spent to be wasted.

### Temporal 2 (Tiered – Decelerate):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Decelerating Temporal energy slows down time around the target. This effectively speeds the target up as the world around it slows down. When this spell is cast, roll for damage as normal. Instead of dealing damage, this spell increases the target’s Speed score by the amount rolled for the duration of the spell. Successive castings of the same spell overlap, though any difference in duration or strength takes effect separately. For example, if a target with 53 speed is subject to a single AP of this spell, and its speed is increased by 5 points, the target effectively has 58 Speed score for the duration. If, during the first spell’s duration, the same target is affected by 2 AP of this spell, and the damage roll is 17, the target’s Speed score is increased by a total of 17 from its original 53 speed, giving it 70 speed, and increasing its Speed Rating to 8 for the duration of the second spell. Accelerating Temporal spells oppose Decelerating Temporal spells. If both energies are simultaneously in effect on the same target, the target is subject to the difference in strength between the 2 spells.

### Thought 2 (Tiered – Communicate):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Communicative Thought energy forms a link between the caster and the target, allowing them to communicate mentally. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. Unwilling targets may roll a Charisma check versus the strength of the spell to prevent the link. Targets of this spell are aware of the spell, and consciously control which thoughts are sent, and will never accidentally send a thought they don’t wish to send. Communication via this spell can be in the form of images, feelings, or words. The caster and target needn’t speak the same language in order to understand one another. Even animal targets are able to communicate clearly with the caster.

### Water (Elemental):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Water energy can generate pure, drinkable water, or affect the flow of a body of water. Each AP of Water energy can generate 1 cup (8 ounces) of pure, drinkable water. When used to affect the current of water, each AP is sufficient to change the speed of an appropriate area of water by 1d10 MPH. A stream can be hastened, slowed, stopped, or even reversed. Still water can be made to flow in any direction. All changes in water flow only affect the area specified by the shape of the spell. Water energy is suitable to counter Fire spells (note that an ignited target may no longer be under the effects of a fire spell).

## Structure

### Building (Duration):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Building duration spells start at low damage and increase in damage with each subsequent round. Starting on the round that the spell is cast, it deals 1d10 damage and gains an additional 1d10 damage each round until it reaches damage dice equal to the amount of AP spent on the spell on the caster’s turn. For example, a 5 AP spell would last 5 rounds and deal 1d10 damage on the first round, 2d10 on the second, and so on up to the fifth round where it would deal 5d10 damage.

When used with Concentration:

When a Building spell is used in conjunction with concentration, the spell starts at 1d10 damage as normal and builds up to damage dice equal to the AP spent. The duration of the spell does not start until concentration is lost, and the number of damage dice does not exceed AP spent. All other structures must stay the same, but location may be changed as long as it remains within the spells range.

### Line (Shape):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

To cast a line shaped spell, the caster focuses the energy used in the spell into a long, narrow shape, resembling a straight tube. The shape of the spell is similar to that of the laser pointer, except that the beam is thicker, and it hits everything within range in the path of the energy, and ignores barriers that don’t completely encompass targets.

### Ray (Shape):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

To cast a ray shaped spell, the caster focuses the energy used in the spell into an ultra-thin beam. The shape of the spell resembles the beam from a laser pointer. A ray shaped spell affects the first target it hits, and is easily blocked by any intervening barriers. An intervening barrier consists of anything not worn or carried by a viable target such as a tree, door, window or wall. If the ray hits a target that isn’t a viable target for the energy used, any AP spent on the spell are wasted. If the target is something like a tree, door, window or wall, the spell takes effect as normal, as long as they are still viable targets. Spells like Charm would not be able to affect the aforementioned examples.

### Spread (Shape):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

To cast a spread shaped spell, the caster focuses the energy used into a sheet of energy with a width that increases steadily as the distance from the caster increases. Spread spells can be directed in 45 degrees (1/8 of a circle, 1 spread increment), 90 degrees (1/4 of a circle 2 spread increments), 135 degrees (3/8 of a circle, 3 spread increments), or 180 degrees (1/2 a circle, 4 spread increments). Spread starts at 1 movement unit and 45 degrees. Each additional AP spent on Spread increases either the movement units by 1 or the spread by 45 degrees. Solid barriers can block a portion, or all, of the spread shaped spell.

## Optional

### Conducted:
> **Status:** ✅ CONFIRMED IN PRINCIPLE — carried through a held object; later decisions govern loss of contact and hybrid delivery. Exact legacy numbers remain review material.

A conducted spell is cast through an object, such as a weapon. For an object to be able to conduct energy, the caster must be able to hold the object in 1 or 2 hands, and the object can’t be stationary. Trees, walls, ground, ceiling and floor count as stationary objects, though sticks, rocks, bricks, and doors aren’t considered stationary. A caster can conduct energy through a weapon, and increase the potential damage of an attack roll. For example, the caster may conduct Fire energy through a staff and use it in a melee attack, or the caster may conduct energy through a length of rope and swing it around, essentially extending their reach. If the attack carries its own melee damage, resolve the attack as a combined Martial and Magic attack. If the attack doesn’t carry any melee damage, it is essentially resolved as a touch shaped spell. If the caster ceases to be in physical contact with the item conducting a spell before the spell is used, the spell dissipates, and any AP spent on the spell are wasted. Ranged ammunition may carry the energy of a conducted spell. Ranged ammunition with conducted energy which is fired and fails to hit a target simply loses the conducted energy at the end of the caster’s turn.

### Worn:
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

To wear a spell, the caster gathers energy tightly around her body, or the body of the target. Worn spells aren’t particularly useful unless they have a duration longer than instantaneous. Worn spells with a duration longer than instantaneous move with a caster naturally like clothing. Worn spells don’t hinder the movement of the wearer. Any equipment worn, but not wielded, is also covered by a worn spell. If the worn spell is a damage spell, melee attackers may take the damage any time they attack within the duration of the spell. Treat this as an attack from the wearer of the spell against the defense of the initial attacker. Attackers that don’t need to be within a movement unit to attack don’t take damage from a worn damage spell. Force can also be shaped into a worn spell, and acts like armor. In this case, attackers don’t necessarily take damage, but the worn spell provides 2d10 defense, regardless of the degree, and damage mitigation from attacks as appropriate. Worn spells don’t cover the eyes, nose, or mouth of the target. Additionally, to wear Force energy, the caster needs to know Wave Force (Tier 1) for cloth armor, Kinetic Force (Tier 2) for light armor, Solid Force (Tier 3) for medium armor and Animated Force (Tier 4) for heavy armor.

# Intermediate

Intermediate energies are a step above basic energies. They take a bit more training to learn, and are only available to more experienced casters. A Specialist must have at least 45 points in their primary casting stat to cast intermediate spells.

## Energy

### Acid (Elemental):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Reduce, Negate, Rebound, Absorb

Acid energy is corrosive. In low concentration, acid burns targets. In high concentration, acid can melt through targets. Extending the duration of an acid spell increases the length of time it burns or melts through targets. Acid energy causes damage by reacting violently on a chemical level, which generates heat, and attacks the Natural structure of objects. When used on objects, Acid energy deals double damage to the Natural structure of objects, though it only does normal damage to living and undead targets. Acid energy never actually causes targets to catch fire, but damages targets in a similar fashion to fire. If Acid energy deals enough damage to overcome the Natural structure of an object, any portion of the object touched by the acid is melted through.

### Animation 3 (Tiered – Commanded):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Commanded animated objects respond to their creator’s commands. Commands may be a bit more complex for commanded animated objects than for controlled animated objects. A commanded animated object can follow an order such as “tidy up”, which may involve a few tasks such as sweeping and dusting, or “hold perfectly still until so-and-so is within range, then attack so-and-so.” Commanded objects always follow the caster’s most recently issued commands. Each AP of Commanded Animation energy is sufficient to animate an object up to 1 cubic foot. Anyone wearing or holding the target object may make a Ward check to resist the animation spell.

### Animation 4 (Tiered – Autonomous):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Autonomous animated objects are seemingly intelligent, but still only follow basic or complex commands. They can follow multiple series of commands, such as “tidy up, then go harvest the carrots in the garden, and attack any intruders.” The autonomous animated object is able to prioritize, as the caster desires, by putting intruders at the top of the list, for example. Autonomous animated objects only follow express orders, and will not go beyond their programming. For example, if told “go hunt a deer,” the automaton will hunt a deer, and stop once it has succeeded. A more specific order, such as “go hunt a deer, then bring the deer back here” is required for the automaton to do more than specifically what it was told. The caster can give the automaton some basic safe guards, like “this is home. Always return home after you’ve carried out your tasks.” All issued commands, within reason, are retained throughout the life of the automaton. The duration units of automatons are measured in days, with a minimum of 1-day duration, even if cast as an instantaneous spell. Each AP of Autonomous Animation energy is sufficient to animate an object of up to 1 cubic foot for a day. Anyone wearing or holding the target object may make a Ward check to resist the animation spell.

### Decay 2 (Tiered – Desiccation):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Reduce, Negate, Rebound, Absorb

Desiccation Decay energy robs targets of their moisture. Living targets subject to desiccation don’t directly take damage, but may begin to suffer dehydration. Each AP of Desiccating Decay energy affects a living target as though it has gone 6 hours without water. A non-living target is treated as though it has spent a full day in direct sunlight. The water taken from targets is not automatically restored after the spell’s duration, though targets suffering dehydration from a desiccation spell can replenish their moisture as normal, by drinking for a creature, by absorbing moisture from the ground for plants, or by being doused or otherwise introduced to moisture for objects. Extensive dehydration doesn’t directly damage targets, though it can weaken or even kill living targets. Desiccation can also dry freshly chopped wood, or driftwood, to make it suitably flammable to build a fire.

### Disease (Primal):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Disease energy causes living targets to become ill. The effects of a disease usually aren’t immediately apparent, as the disease takes time to incubate. Disease energy infects the target with a normal disease. The infection may last beyond the duration of the spell. Even the most basic instantaneous disease spell, delivered via touch, will cause the target to get sick, unless the target manages to resist the disease. Disease energy can also be used to cure an already diseased target. To successfully cure a disease, the caster first diagnoses the disease the patient has, then “infects” the patient with antibodies of at least equal potency. The patient must then go through the normal recovery process for the disease. If the caster misdiagnoses the patient, or simply doesn’t attempt to diagnose the patient, the antibodies are chosen the same way the disease was chosen. Unmodified disease spells have an incubation period of 2 weeks before the symptoms take hold. Each AP of Disease energy is sufficient to either decrease the incubation period by 1 day, to a minimum incubation period of a single day, or increases the severity of the disease symptoms inflicted or cured, as shown in the table below. The number of AP a specialist spends on a Disease spell determines how many symptoms the disease will have. For example, if a specialist used 13 AP, the specialist could choose 1 symptom from the 10-21 AP section and 1 from the 1-3 AP section, or any combination of lower AP symptoms totaling less than or equal to 13.

1-3 AP: Sneezing, coughing, fever, sweating, nausea, rash/inflammation, insomnia, dizziness

4-9 AP: Fatigue, diarrhea, vomiting, pulmonary edema, dementia, skin lesions, cysts/boils, blurred vision

10-21 AP: Hypersensitivity, ataxia, kidney failure, hemorrhaging, dysentery, pneumonia, seizures, hemophilia

22+ AP: Liver failure, heart failure, blindness, hypotonia, encephalitis, necrosis, insanity, systemic infection, coma

### Dispel 4 (Tiered – Targeted):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Targeted Dispelling energy dispels a single spell in place, at the caster’s choice. If the caster knows any of the spells in place on the intended target, the caster need only match the AP of the effect to be dispelled, even if it’s not the strongest spell. If the caster doesn’t know any of the spells in place on the target, the caster chooses a number of AP to use in their Targeted Dispel spell. The Keeper then tells the caster all the energy types less than, or equal to the Targeted Dispel spell in AP, and the caster chooses 1 of the energies to dispel.

### Dispel 5 (Tiered – Multi-target):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

A Multi-targeted Dispel energy spell dispels multiple magical effects currently in place, chosen by the caster. When casting this spell, the caster chooses a number of spells and the maximum AP of spells to be dispelled. The AP of Multi-target Dispelling energy required is equal to the number of spells multiplied by the highest AP to be dispelled. For example, if the Specialist wants to dispel 3 spells, with a maximum AP of 5, they would need to cast a Multi-target Dispel spell with 15 AP. Once the maximum AP and number of spells to dispel has been determined, the Keeper lists all available energies that meet the criteria, and the caster chooses which energies to dispel. If the number of energies available are fewer than the number of spells the caster specified, the Keeper still lists the energies, but all available energies meeting the criteria are dispelled.

### Divination 4 (Tiered – Unknown, Aided):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Unknown, Aided Divination energy allows the caster to spy on a target matching a description with the aid of a reflective surface. This spell turns any mirror, puddle, or crystal ball into a window to distant events. The caster can see and hear events up to a mile away, but gets no other sensory input. Each AP of Unknown, Aided Divination energy allows the caster to see an additional mile away. Targets get an automatic Ward check against this spell.

### Divination 5 (Tiered – Known, Visual):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Known, Visual Divination energy allows the caster to spy on a known target, and receive visual input only, without the aid of a reflective surface. The caster sees the distant events by merely closing his or her eyes. The caster can see events up to 10 miles away, but gets no other sensory input. Each AP of Known, Visual Divination energy allows the caster to see an additional 5 miles away. Targets get an automatic Ward check against this spell.

### Drain (Primal):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Drain energy steals the Vitality points of the target, and gives them to the caster’s Vitality pool. Drain energy only works correctly on living creatures. If used on a non-living creature, the spell simply fails. If used on an undead creature, the spell works in reverse, lowering the Vitality points of the caster, and giving animus to the undead. An undead caster can use drain on a living creature to replenish its animus. An undead may also drain animus of another undead, just as a living caster drains the Vitality points of another living creature. Drain energy is not capable of draining off more Vitality or Animus points than a creature has. For example, if a specialist deals 30 points of damage to a target with only 10 Vitality points remaining, the drain spell would only deal 10 points of damage, and the caster would therefore only gain 10 Vitality points.

### Explosion 3 (Tiered – Undead):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Undead Exploding energy causes undead creatures to fly apart as shrapnel. When this spell is cast, roll for damage as normal. If the damage is insufficient to overcome the remaining Animus pool of the creature, the spell fails. If the damage is sufficient to overcome the remaining Animus pool of the creature, it bursts apart violently and sends shrapnel nearby. Shrapnel travels in a diameter of 1 movement unit, sized appropriately for the creature. Shrapnel from soft creatures exploding impacts nearby creatures and objects, but only has a chance of harming very fragile targets. Hard creatures, such as skeletons exploding send sharp, jagged shrapnel at nearby targets. In this case the caster makes a single ranged attack roll, and each nearby target defends against the attack roll. Any targets hit by the shrapnel take half the damage originally rolled for the target of the explosion spell.

### Force 3 (Tiered – Solid):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Solid Force energy forms a barely visible impenetrable barrier. Solid energy can never be touch, emanation, fog, mist, or cloud shaped. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. Line shaped Solid Force energy pushes any creatures that fail a Toughness check or objects in its path aside. Spread shaped Solid Force pushes creatures that fail a Toughness check, as well as objects, away from the caster. Burst shaped Solid Force energy hurls creatures that fail their Toughness check away from its center. Worn Solid Force energy acts as a sheet of armor, which provides protection equal to the strength of the spell, versus all damage types, but imposes no movement restrictions or penalties. Wall shaped Solid Force energy can be used to create a barrier in a doorway, or other pathway, to prevent travel or attack. Sphere shaped Solid Force energy can be used to protect anything inside, or to hold anything inside captive.

### Implosion 3 (Tiered – Undead):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Undead Imploding energy crushes undead targets violently. When this spell is cast, roll for damage as normal.  If the damage is insufficient to overcome the creature’s remaining Animus pool, the spell fails. If the damage is sufficient to overcome the remaining Animus pool, it collapses into a ball 1/100th the size of the original creature. The implosion of very large creatures can create a minor vacuum in the surrounding area, pulling light objects toward it, but creating barely more than a cool breeze for anything weighing more than a pound.

### Merge 3 (Tiered – Undead):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Merging energy combines targets. Only willing targets can be combined, and any merge spell attempted on an unwilling target simply fails. Mindless creatures, and creatures of animal intelligence are never considered willing targets, unless they’re being controlled, in which case the controller must be willing. Higher tiers of merge energy allow a wider variety of targets to be merged, eventually allowing normal, living creatures to be affected. Any target may be combined with other targets from lower tiers as well. For example, a living merging spell can merge a living target with an object. In any merge spell, the largest target to be combined is considered the base of the resulting object or creature. Creatures merged into stationary targets maintain their senses, though they may be unable to move for the duration of the spell. For example, a caster that merges with a large boulder to hide from a goblin raiding party would still be able to see and hear as normal from within the boulder. While inside the boulder, the caster is immune to damage, so long as part of the boulder remains larger than the caster’s natural size. If the boulder explodes, or is crushed, however, and no piece larger than the caster’s natural size remains, the caster is killed, and her corpse is left in pieces no larger than the largest remaining piece of the boulder.

Undead Merging energy combines un-living objects and/or undead creatures into one. Undead creatures, corpses, stationary objects such as statues or walls, or up to false living animated targets, as well as non-stationary objects can be combined. For example, a controlled zombie, whose controller is willing, could be combined with a spear, to give the zombie’s melee attacks extra piercing damage. Intelligent undead must be willing in order to be targeted with this spell. When casting this spell, the caster must declare the desired result. If the Keeper rules the result is not possible, the caster may opt not to cast the spell. Targets to be combined must be touching when the spell is cast. Each AP of Undead Merging energy is sufficient to combine up to 1 cubic foot of un-living and/or undead targets. Any number of objects may be combined so long as they are all touching at least 1 other object to be combined, and the combined total of the objects remains 1 cubic foot or less per AP of the spell.

### Possession 2 (Tiered – Parasitic):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Parasitic Possession energy puts the soul of the caster, or another willing possessor designated by the caster, into the same body as the target. The possessor senses everything the host body does, even when the possessor isn’t in control of the body. The possessor can attempt to take control of the host body at will for the duration of the spell. Control of the body is determined by an opposed Charisma check, with the victor gaining control of the body. On any action the possessor is in control of the body, the host may attempt another Charisma check to regain control of its own body, though a willing target may simply allow the possessor to maintain control. The possessor may relinquish control of the body at any time. The possessor may take purely mental actions, including casting a spell, even when not in control of the body. This spell is often used by a caster whose own body has died, in order to find a suitable corpse to possess. When the spell ends, the possessor returns to its original body, if its own body remains intact. If the possessor’s own body has died, the possessor also dies when the spell ends. The duration of Parasitic Possession energy is measured in days. Each AP of Parasitic Possession energy gives the possessor a bonus of 1d10 point on their opposed Charisma rolls to control the body. The table below shows which attributes are considered physical, and which are considered mental.

Physical Stats: Agility, Endurance, Equipment, Fortitude Pool Ranks, Looks, Physical Racial Traits, Size, Speed, Stamina, Toughness, Vitality Pool Ranks

Mental Stats: Charisma, Insight, Intelligence, Luck Pool, Magic Components, Martial Components, Mental Racial Traits, Proficiencies, Skills, Unspent XP

### Precognition 2 (Tiered – Foresight):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Foresight Precognitive energy allows the caster to see a glimpse of the future. To cast a Foresight Precognition spell, the caster must concentrate on a particular possible action while casting the spell. Once the spell is completed, the caster sees the immediate results of the action through caster’s own eyes. The caster sees events lasting as long as the duration of this spell. One AP of Foresight Precognitive energy is sufficient to see the immediate result of a particular action, though many casters use more AP to prevent counterspelling.

### Sap Energy (Primal):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Reduce, Negate, Rebound, Absorb, Prohibitive

Sap Energy drains targets of a small amount of AP and invigorates the caster in return. This spell bestows negative AP counters equal to the AP spent on this spell on any target hit. These negative AP counters last for the duration of the spell. Targets may remove negative AP counters at a cost of 1 AP each. For each target hit by this spell, the caster gains an additional 1 AP at the start of their next turn. For each target with remaining negative AP counters at the start of the caster’s turn, they gain an additional 1 AP on their following turn.

A target can only be hit by a single instance of this spell from the same caster within the duration of the spell. Sap Energy spells with durations longer than instantaneous do not bestow additional negative AP counters to previously affected targets in subsequent rounds, though any new target that would be subject to the spell may still gain negative AP counters.

 Sap Energy only works correctly on living creatures. If used on a non-living creature, the spell simply fails. If used on an undead creature, the spell works in reverse, giving the target AP counters, and giving the caster negative AP counters. An undead caster can use Sap Energy on a living creature or on another undead creature as normal.

### Teleportation 4 (Tiered – Known):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Known Teleportation energy takes the caster or other target to anywhere the caster knows within range. For this spell to work, the caster needs to have been to the desired destination at least once. The first AP of Known Teleportation energy is sufficient to teleport the caster (regardless of weight) or other target weighing no more than 150 lbs. up to 10 miles. Each additional AP is sufficient to increase the weight limit by another 50 lbs. or to increase the maximum distance by 5 miles.

### Teleportation 5 (Tiered – Summon):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Summoning Teleportation energy brings specific, known creatures or items to the caster’s location. In order for this spell to work, the caster needs to have touched the creature or object to be summoned. Summoning Teleportation energy works across any distance. If the shape of this spell is touch, the summoned creature or item appears in the caster’s hand, if it’s small enough, or adjacent to the caster otherwise. The first AP of Summoning Teleportation energy is sufficient to summon a creature or object weighing no more than 50 lbs. Each additional AP of Summoning Teleportation energy increases the weight limit by 25 lbs.

### Teleportation 6 (Tiered – Conjure):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Conjuring Teleportation energy brings the nearest creature or item of a type specified to the caster. Conjuring Teleportation energy works across any distance. If the shape of the spell is touch, the conjured creature or object appears in the caster’s hand, if it’s small enough or adjacent to the caster otherwise. The caster may specify that it be the nearest creature or item that is not visible to the caster. For example, if the caster has a dog as a pet or companion, and the caster wants to summon a dog, the caster may specify that the dog summoned not be the caster’s dog. Conjured targets have no particular disposition towards the caster. Hostile conjured targets may attack the caster. The first AP of Conjuring Teleportation energy is sufficient to retrieve a creature or item weighing no more than 100 lbs. Each additional AP increases the weight limit by 50 lbs.

### Temporal 3 (Tiered – Halt):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Halt Temporal energy stops time around the target. The target is free to act for the duration of this spell. While under the effects of this spell, the target is unable to harm or move anything that is frozen in time. Any equipment the target is wearing, holding or wielding is also free to act, even if the target releases or drops such an item. Any spells a creature casts while targeted by Halt Temporal energy occur as normal, though they still don’t harm any creatures or objects frozen in time, unless they have durations that last beyond the duration of the Halt Temporal energy.  For example, if time is halted for 5 actions, a 3-action cloud shaped Fire energy spell cast while time is halted on the last action of halted time would last 2 more actions after the time halt ends. Spells lasting beyond the end of halted time affect targets normally once time resumes. The maximum number of actions this spell can last is equal to the number of AP spent on Halt Temporal.

### Temporal 4 (Tiered – Loop):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Looping Temporal energy causes a short series of events to recur. When this spell is cast, the specified number of events after completing this spell recur a number of times specified by the duration of this spell. The Keeper should track the specified number of actions after this spell ends, so the events can be replayed. Each AP is sufficient to make 1 action repeat for the duration of the spell.

### Thought 3 (Tiered – Read):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Read Thought energy forms a link between the caster and the target, allowing the caster to pry information from the target’s mind. For the duration of this spell, the caster can read all the surface thoughts of the target. In order to get specific information from the target, the topic must be brought up to the target, whether simply by the target thinking about it, the topic being brought up in conversation, or by interrogating the target. Unconscious targets have no surface thoughts. If the target of this spell becomes unconscious, the spell ends. If the spell is cast on an unconscious target, it fails. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. The target may attempt a Charisma check to negate this spell’s effects.

## Structure

### Burst (Shape):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

To cast a burst shaped spell, the caster focuses energy into a tight ball which, when released, causes the energy to expand outward violently from the point of origin. The effect typically appears to be an explosion of the type of energy used in the spell. The explosion fills an area equal to a sphere with a diameter of 1 movement unit for each AP of the spell. The duration of a burst shaped spell may only be instantaneous.

### Diminishing (Duration):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Diminishing duration spells start at high damage and decrease in damage with each subsequent round. Starting on the round that the spell is cast, it deals 1d10 per AP spent on the spell and loses 1d10 each subsequent round until it reaches 1d10 on the caster’s turn. For example, a 5 AP spell would last 5 rounds and deal 5d10 on the first round, 4d10 on the second, and so on until the fifth round where it would deal 1d10.

When used with Concentration:

When a Diminishing spell is used in conjunction with concentration, the spell starts at d10 equal to AP spent as normal and continues to deal that number of d10 per round as long as concentration is maintained. After concentration is lost, the spell takes effect as normal for the Diminishing duration. All other structures must stay the same, but location may be changed as long as it remains within the spell’s range.

### Emanation (Shape):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

To cast an emanation shaped spell, the caster gathers energy tightly around her body, or the body of the target. Once gathered, the energy radiates outward for the duration of the spell, or bursts outward if the duration is instantaneous. The spell radiates or bursts to fill an area 1 movement unit in diameter for each shape increment, but does not harm the caster, or the target of the spell if cast on a target. For targets larger than 1 movement unit, appropriately sized for the caster, the minimum shape increments must be large enough to encompass the target. For example, if a horse takes up 2 movement units, the spell would have to be a minimum of 2 shape increments to benefit the horse. Any viable target within range is subject to the effects on each of the spell’s duration increments for the duration of the spell. Solid barriers block the radiating energy.

### Fog (Shape):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

To cast a fog shaped spell, the caster suspends the spell’s energy in the air. The fog is heavy, and will roll down hills, or seep through cracks in the floor at a rate of 1 movement unit, appropriately sized for the caster, per round. A fog shaped spell with no duration acts as a larger area burst shaped spell, but deals less damage. The energy in a fog shaped spell is spread thin, so the spell only deals half normal damage to anything within the area. A fog shaped spell starts as a spherical area with a diameter measured in increments of 2 movement units, but immediately begins to spread out and settle. Each full round after the fog is created, the fog settles 1 movement unit, and its size changes, with its height cut in half and its diameter doubled, so long as it has room to spread. A fog shaped spell is lighter than water, and will settle onto water. A fog shaped spell cast under water will rapidly rise to the surface at a rate of 4 movement units per round. As the fog rises to the surface, the height of the fog is cut in half, and the diameter doubled for each movement unit traveled. Any wind, magical or otherwise, pushes the fog along at a rate equal to half the wind’s speed.

### Group (Target):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Group targeted spells affect all viable targets within a group, so long as each member of the group is touching another member of the group, such as a group of Specialists holding hands or a pile of arrows. All viable targets that are in some way connected to the initial target are affected. If group targeting is used in conjunction with an area effect spell, all members of any groups that come into contact with the energy are affected. Casting a group spell increases the overall AP cost of a spell by 1AP per target beyond the first.

## Optional

### Activated:
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Activated spells are cast as normal, but don’t take effect until a specific condition, or set of conditions is true. For example, a spell could be set to be triggered the first time an undead creature comes within range. Activated spells may be anchored to creatures, objects, or even to a particular place. Spells anchored to creatures or objects move with their anchor until the spell is resolved. Spells anchored to a place don’t move. Duration may be specified for activated spells, though the spell still does not occur until the trigger condition is met. If 2 or more spells with the same effect are placed on the same anchor, and with the same trigger, the spells overlap, and only the strongest effect takes place, though each spell has a chance to be dispelled separately.

Casting activated spells is strenuous. A Specialist may only have one activated spell in existence at a time. Casting a second activated spell cancels out the first. A Specialist may only cast an activated spell using as many AP as they have for a single round of combat.

### Arcing:
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Arcing spells consist of wild currents of energy. The energy shoots out, and visibly arcs across multiple targets. Arcing spells hit a number of targets beyond the initial target equal to the AP spent on the spell. Each additional target must be within a number of movement units, appropriately sized for the caster equal to the AP spent on this spell. The spell arcs from the initial target to the nearest target, and so on, until the appropriate number of targets has been hit. If two or more targets are equal distance from the current target, the Keeper determines randomly which is hit by the next arc. This spell will not arc to a target that has already been a target of this spell. Arcing spells may only have defined or selective as their target. Defined arcing spells jump around, hitting friend and foe alike. Selective target spells hit only friends or only foes.

# Advanced

Advanced energies are a step above intermediate energies. Advanced energy is only available to those with extensive magic training. A Specialist must have at least 60 points in their primary casting stat to cast advanced spells.

## Energy

### Animation 5 (Tiered – False Life):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

False Life Animation energy gives objects the ability to reason with basic intelligence. A false living object will act as any friendly human of average intelligence would toward its creator. The false living object will do the best it can to please its creator, and will follow most commands very well. If asked to do something that endangers itself, however, it may hesitate, or even rebel. Along with its intelligence, a false living object gains a sense of self-preservation. If the object has a mouth-like orifice, the false living object can speak. If it can’t speak, the false living object attempts to communicate through action, and expressions of emotion. The duration of False Life Animation energy is measured in days, with a minimum of 1-day duration, even if cast as an instantaneous spell. The first AP is sufficient to animate an object of up to 1 cubic foot, and give the object an Intelligence score of 1d10. Each AP past the first increases the size of the object that can be animated by an additional cubic foot, or increases the animated object’s maximum possible Intelligence score by an additional 1d10. The animated object’s Intelligence score can never exceed the caster’s own Intelligence score. For example, if a caster with a 23 Intelligence score wanted to create a false living object with a 23 Intelligence score out of a 2-cubic foot object, it would require 4 AP: 1 for the first cubic foot and 1d10 points of intelligence, 1 more for the second cubic foot, 1 more for the next 1d10 points of intelligence, and 1 more for the final 1d10 points of intelligence. Anyone wearing or holding the target object may make a Ward check to resist the Animation spell.

### Boon (Primal):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Boon energy boosts a creature’s abilities for the duration of the spell. A Boon spell with an instantaneous duration applies to the next appropriate action made by the target. Boon energy can increase any ability score, skill check, attack roll, defense roll, magic roll, or ward roll, chosen by the caster of the Boon spell. Boon energy is suitable to counter Curse spells. Each AP of Boon energy is sufficient to raise any stat or roll by 1d10 points.

### Charm 3 (Tiered – Influence):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Influence Charm energy alters the target’s perception of others. The duration of influence is measured in hours. The caster can sway a creature’s disposition toward friendly or unfriendly. The target’s disposition change may be towards the caster, or it may be towards another target designated by the caster. For instance, the caster may shift a troll’s disposition toward a locked door to hostile, so the troll will attack the door. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. If the target fails to resist the spell, add the strength to, or subtract the strength from the target’s disposition as appropriate. Influenced creatures maintain their sense of self-preservation. Though an influenced creature may be hostile toward an obviously stronger foe, it may not attack if attacking would be suicidal.

### Curse (Primal):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Curse energy hampers a creature’s abilities for the duration of the spell. A Curse spell with an instantaneous duration applies to the next appropriate action made by the target. Curse energy can decrease any ability score, skill check, attack roll, defense roll, magic roll, or ward roll, chosen by the caster of the Curse spell. Curse energy is suitable to counter Boon spells. Each AP of Curse energy is sufficient to lower any stat or roll by 1d10 points (to a minimum of 1).

### Decay 3 (Tiered – Rot):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Reduce, Negate, Rebound, Absorb

Rot Decay energy makes organic tissue die and putrefy from the outside in. The tissue of living creatures affected by Rot Decay energy dies and turns rancid starting at the surface, and spreading 1 centimeter in each direction (including inward) for each AP of the spell cast. Living creatures subject to Rot Decay spells also take 1d10 points of necrotic damage for each AP of the spell. The flesh around a touch shaped Rot Decay spell rots in a spherical radius around the point of contact in terms of width and depth. A creature surrounded by Rot Decay energy is eaten alive from the outside in, starting with skin, followed by fatty tissues, followed by muscles, followed by internal organs, and ending with bone marrow. At the Keeper’s discretion, internal organs may be targeted first, bypassing skin, fat, and muscle. Rotting plant matter, other than fruit, whether living or formerly living, begins to liquefy, and grows mold and fungus. Rotting fruit ferments, and becomes alcohol. A Rot Decay spell used on a corpse or undead works the same as it does on a living target, but corpses and undead don’t feel pain from the rot, though the putrefaction of their flesh may cause them to smell worse than they did to begin with. Rotted areas of targets aren’t restored automatically after the duration of the spell, and remain rotted, unless magic is used to restore the rotted areas.

### Destabilization (Primal):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Destabilization energy causes targets to shake violently. Destabilizing energy can shatter glass, reduce clay pitchers to dust, or even cause earthquakes. When used on an area, anything within the area that can be considered an object, including the ground, may be affected. Destabilizing energy can only be used on objects. A creature may be targeted by Destabilizing energy only if the creature also counts as an object. In order to affect an object, the destabilization must deal enough damage to overcome an object’s Structural Integrity. Destabilization causes cracks and fissures to appear in targets. An instantaneous Destabilization spell instantly shatters small objects, such as a window or a clay pot, but doesn’t produce noticeable effects on the ground or a wall right away. Larger objects or areas shake violently for a number of rounds equal to the cubic feet of the object or area affected. Each AP of Destabilization energy is sufficient to affect up to 1 cubic foot of material.

### Dispel 4 (Tiered – Choice):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Chosen Dispel energy nullifies all harmful spells in place, or all beneficial spells in place. When a Chosen Dispelling spell is cast, the caster chooses whether to dispel all beneficial effects on the target, or to dispel all harmful effects on the target. A Chosen Dispelling spell requires a minimum number of AP equal to the AP of the strongest spell, multiplied by the number of spells to be dispelled. Whether a spell is considered harmful, beneficial, or benign can vary, depending on the situation. When this spell is cast, the Keeper tells the caster what energies are present, and the caster decides which energies should be considered harmful, which should be considered benign, and which should be considered beneficial.

### Divination 6 (Tiered – Known):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Known Divination energy allows the caster to spy on a known target, and receive visual and audial input, without the aid of a reflective surface. The caster sees and hears the distant events by merely closing his or her eyes. The caster can see and hear events up to 10 miles away, but gets no other sensory input. Each AP of Known Divination energy allows the caster to see an additional 10 miles away. Targets get an automatic Ward check against this spell.

### Earth (Elemental):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Reduce, Negate, Rebound, Absorb

Earth energy can cause the growth of plants, or generate dirt, sand, rock, or sharp, jagged stone. An Earth spell can speed the growth of a plant by roughly a month, or more with your Keeper’s approval, for each AP. An Earth spell can also generate 1 lbs. worth of dirt, sand, rock, or sharp, jagged stone for each AP.

### Enhancement 2 (Tiered – Physical):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Reduce, Negate, Rebound, Absorb

Physical Enhancement energy alters the way the target’s body works in such a way as to allow unusual physical prowess for the duration of the spell. The physical prowess granted by the spell may allow a target to climb or balance at their full walk or run speed, allow a target to jump vast distances, squeeze through an incredibly tight space, hold their breath for very long periods of time, and so on. Physical Enhancement energy should be limited to slightly altering the physiology of a target, but not changing physical features. For example, a creature’s muscles may become more spring-like, and their bones become less dense to allow for incredible leaps, but growing wings should be limited to Mutation spells. A Keeper may say what you’re asking for doesn’t count as an enhancement at any time. For example, if you want to be able to stick your finger into a lock in an attempt to pick it, the Keeper may say you can slide your finger into the keyhole of the lock, but that the ability doesn’t confer any bonuses toward picking the lock. Each AP of Physical Enhancement energy confers an additional modification to the target’s physical prowess. Physical Enhancement energy is suitable to counter Physical Hinder spells.

### Explosion 4 (Tiered – Unnatural):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Unnatural Explosion energy causes unnatural creatures to fly apart as shrapnel. When this spell is cast, roll for damage as normal. If the damage is insufficient to overcome the remaining Vitality pool of the creature, the spell fails. If the damage is sufficient to overcome the remaining Vitality pool of the creature, it bursts apart violently and sends shrapnel nearby. Shrapnel travels in a diameter of 1 movement unit, appropriately sized for the creature. Shrapnel from soft creatures exploding impacts nearby creatures and objects, but only has a chance of harming very fragile targets. Hard creatures exploding send sharp, jagged shrapnel at nearby targets. In this case the caster makes a single ranged attack roll, and each nearby target defends against the attack roll. Any targets hit by the shrapnel take half the damage originally rolled for the target of the explosion spell.

### Fabrication 3 (Tiered – Duplicate):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Duplicate Fabrication energy can be used to create an exact replica of any creature or object. The duplicate of any living thing is always lifeless. For example, a duplicate of a living creature is considered a corpse. Aside from being lifeless, duplicates are exact copies of the original, including any flaws the original had. The caster must be able to physically touch the object to be duplicated while this spell is being cast. Duplicate Fabrication energy requires 1 AP for each cubic foot to be duplicated. This spell can only be used to duplicate objects made with normal materials. Attempts to duplicate objects with special materials simply fail. Anyone wearing or holding the target object may make a Ward check to resist the Duplicate Fabrication spell.

### Flight 3 (Tiered – Hover):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Hover Flight energy lifts the target off the ground with a cushion of air. Hovering objects lift off the ground, and glide laterally with ease, though they do carry momentum and inertia. A heavy hovering object moving in 1 direction should be given plenty of room to slow down, lest it slam into the first object or creature in its path. Hovering creatures move laterally with only the effort of thought. A hovering creature can start moving, stop moving, or change direction as quickly as they can think it. When cast on a creature other than the caster, the caster must decide if the target or the caster will have control of direction. Once this decision is made, it can’t be changed for the duration of the spell, though a more powerful version of the spell could shift the control. Hovering creatures and objects float above solid and liquid surfaces. A hovering creature could float over lava without sinking into it; however the creature still takes damage from the intense heat. Each AP is sufficient to make an object or creature weighing up to 25 lbs. hover.


### Force 4 (Tiered – Animated):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Animated Force energy forms a 3-dimensional shape, and moves as the caster desires. For the duration of the spell, the caster can move, reshape, and otherwise control the Animated Force energy as she sees fit. Animated Force can recreate basic gestures easily, though anything involving fine motor skills is impossible. Activities that would require fine motor skill are determined by your Keeper. Each AP of Animated Force energy is sufficient to create an animated object up to 1 cubic foot.

### Hinder 2 (Tiered – Physical):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Reduce, Negate, Rebound, Absorb

Physical Hindering energy robs the target of physical prowess, and fine motor skills. This spell first removes any magical physical enhancements, followed by innate physical bonuses, followed by normal movement and speech. Once all magical and innate enhancements are gone, the target appears to suffer from advancing stages of drunkenness, starting with slowed reaction time, followed by slurred speech, then blurred vision, then stumbling, and finally unconsciousness. Magical physical enhancements removed by this spell simply end. Targets put into a stupor or reduced to unconsciousness by this spell remain in that state for the duration of the spell. Normal motor skills, and any innate physical prowess returns once this spell ends. Each AP of Physical Hindering energy removes 1 existing physical enhancement. Each AP beyond that removes 1 innate physical bonus. Beyond that, each AP causes the next stage of apparent drunkenness, as listed above. Physical Hinder energy is suitable to counter Physical Enhancement spells.

### Illusion 3 (Tiered – Invisibility):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Invisibility Illusion energy hides the target from sight. Invisible creatures and objects are still physically there, and can still be felt, heard, smelt, and possibly tasted, as normal. Onlookers may still be able to locate invisible targets based on the other senses, or even sight. For example, an invisible creature walking in sand or snow still leaves footprints. A creature that bumps into an invisible creature or object can feel it. Creatures with acute senses of smell or hearing may be able to smell invisible creatures, or hear the creature’s breathing or heartbeat. When this spell is cast, the target, along with the target’s gear, becomes invisible. Anything the target was not wearing or holding when the spell was cast remains visible, unless hidden completely inside another part of the invisible creature’s gear or body. For example, if an invisible creature picks up an apple, the apple is still visible. If the invisible creature takes a bite of that apple, the portion of the apple that is completely in the creature’s mouth becomes invisible, though the remainder of the apple remains visible. Likewise, a pen picked up by the invisible creature would remain visible, unless the creature put the pen into a sack or the pocket of an invisible garment. Any invisible gear the creature drops or puts down immediately becomes visible again. Creatures and objects can’t be made partially invisible. Each AP of Invisibility Illusion energy is sufficient to make a creature or object up to 1 cubic foot invisible.

### Implosion 4 (Tiered – Unnatural):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Unnatural Implosion energy crushes unnatural targets, such as abominations and aberrations, violently. When this spell is cast, roll for damage as normal. If the damage is insufficient to overcome the creature’s remaining Vitality pool, the spell fails. If the damage is sufficient to overcome the remaining Vitality pool, it collapses into a ball 1/100th the size of the original creature. The implosion of very large creatures can create a minor vacuum in the surrounding area, pulling light objects toward it, but creating barely more than a cool breeze for anything weighing more than a pound.

### Manipulation (Primal):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Manipulation energy is used for operating mechanisms. The most basic use of Manipulation spells is the locking and unlocking of doors. When used at range, a Manipulation spell allows the caster to do things they could normally do with their hands for the duration of the spell, such as opening or closing doors, writing with a pen, or carrying a candle. Each AP of Manipulation energy allows a Specialist up to 1d10 on a skill check (not to exceed their own skill level) at range, or increases the amount of weight the caster can manipulate by 1 pound. Manipulation energy can only be used on objects and mechanisms.

### Merge 4 (Tiered – Unnatural):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Unnatural Merge energy combines targets. Only willing targets can be combined, and any merge spell attempted on an unwilling target simply fails. Mindless creatures and creatures of animal intelligence are never considered willing targets, unless they’re being controlled, in which case the controller must be willing. Higher tiers of Merge energy allow a wider variety of targets to be merged, eventually allowing normal, living creatures to be affected. Any target may be combined with other targets from lower tiers as well. For example, a Living Merging spell can merge a living target with an object. In any merge spell, the largest target to be combined is considered the base of the resulting object or creature. Creatures merged into stationary targets maintain their senses, though they may be unable to move for the duration of the spell. For example, a caster that merges with a large boulder to hide from a goblin raiding party would still be able to see and hear as normal from within the boulder. While inside the boulder, the caster is immune to damage, so long as part of the boulder remains larger than the caster’s natural size. If the boulder explodes, or is crushed, however, and no piece larger than the caster’s natural size remains, the caster is killed, and her corpse is left in pieces no larger than the largest remaining piece of the boulder.

Unnatural Merge energy combines un-living objects, undead creatures, and/or unnatural living creatures into one. Unnatural creatures, such as abominations and aberrations, undead creatures, corpses, stationary objects such as statues or walls, or up to false living animated targets, as well as non-stationary objects can be combined. For example, a homonculus could be combined with a pile of arrow heads to give the homunculus a piercing bite attack. Unnatural targets must have better than animalistic intelligence, and be willing in order to be targeted with this spell. When casting this spell, the caster must declare the desired result. If the Keeper rules the result is not possible, the caster may opt not to cast the spell. Targets to be combined must be touching when the spell is cast. Each AP of Unnatural Merge energy is sufficient to combine up to 1 cubic foot of objects, un-living, undead, and or unnatural living targets. Any number of objects or creatures may be combined so long as they are all touching at least 1 other object to be combined, and the combined total of the objects remains 1 cubic foot or less per AP of the spell.

### Mutation 3 (Tiered – Reformation):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Reformation Mutation energy changes the chemical makeup of the target. The most common and effective uses of Reformation Mutation energy are strengthening or weakening objects or body parts, and changing liquids into other liquids. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell.  Reforming the skin of a creature can make the skin tougher, to absorb more damage, or weaker, to be damaged more easily. When used to make the tissue of a creature stronger or weaker, roll for damage as normal. Instead of dealing damage directly, the result of the roll sets the strength of this spell. The target creature’s effective natural Vitality pool or Animus pool is increased or decreased by an amount equal to the strength of this spell for the duration of the spell. This spell can never reduce a creature’s natural Vitality pool or Animus pool to zero. When used to make objects and structures stronger or weaker, the object’s Natural Structure is increased or decreased by an amount equal to the strength of this spell for the duration of the spell. This spell can never reduce an object’s Natural Structure to zero. When used to reform the chemical composition of liquids, this spell can change any liquid known to the caster into any other liquid known to the caster. Throughout the duration of the spell, the remade liquid acts as though it were the new liquid, though any effects revert to normal when the spell ends. For example, if the caster turns poison into wine, anybody drinking it may get drunk off the wine. Once the Reforming Mutation spell ends, the wine reverts to poison. If the liquid hasn’t already passed through the system of the drinker, it immediately affects the drinker as though they had just imbibed an equal amount of the original poison. Similarly, if the caster turns water into wine, anybody drinking it may get drunk off the wine, but when the spell ends, the wine reverts to water, and the drunkenness immediately stops. When used to reform liquids, each AP of Reformation Mutation energy is sufficient to change up to 1 pint of liquid. The duration of Reformation Mutation energy is measured in hours.

### Possession 3 (Tiered – Master):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Master Possession energy gives the caster full control of a host body. If the host body is alive, the host’s soul is severed from the body, effectively killing the host. If the host body is not living, the body must be in good enough condition to sustain a soul. Mortally wounded corpses require healing, at least to the point that the body would have 1 Vitality point. Attempting to possess the body of an undead creature simply kills the possessor, though the undead can be made into a normal corpse through the use of Positive energy or a Life spell. Master Possession energy spells are permanent. Once a body has been mastered via possession, the body is considered to be the possessor’s own body. The physical stats of the new creature are those of the body, while the mental stats are those of the possessor. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. If the strength of the spell is greater than the Endurance Score of a corpse, the caster may possess the body. If the strength of the spell is double or more of the Endurance Score of a living target, the caster may possess the target’s body. If the strength of the spell is less than the Endurance Score of either a corpse or a living target, the spell fails. The table below shows which attributes are considered physical, and which are considered mental.

Physical Stats: Agility, Endurance, Equipment, Fortitude Pool, Looks, Physical Racial Traits, Size, Speed, Stamina, Toughness, Vitality Pool Ranks

Mental Stats: Charisma, Insight, Intelligence, Luck Pool, Magic Components, Martial Components, Mental Racial Traits, Proficiencies, Skills, Unspent XP

### Protection 3 (Tiered – Rebound):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Rebound Protection energy reflects damage and effects from other spells back toward their source. When this spell is cast, the caster chooses an energy type. On completion, damage is rolled as normal. Instead of dealing damage, the amount rolled becomes the protection rating. This spell reflects damage and effects from spells of the chosen energy type up to the protection rating for the duration of the spell. The protected creature still takes any damage beyond the protection rating. For example, if the caster chooses Fire energy, and rolls 23 points, this spell reflects up to 23 points of Fire spell damage whenever the protected creature would otherwise take Fire spell damage. If, during the course of this spell, the protected creature is hit with 15 points of Fire spell damage, the protected creature takes no damage, and the full 15 points are reflected back toward their source. If the protected creature is then hit with 27 points of Fire spell damage, the first 23 points of damage are reflected back toward their source, and the protected creature takes the remaining 4 points of damage. Unless otherwise protected from the reflected energy, the caster of the damaging energy spell always takes the reflected damage. Rebound Protection spells don’t protect against natural sources of damage, such as a campfire.

### Repulsion 3 (Tiered – Undead):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Undead Repulsion energy gives undead creatures an aversion to the target. Repulsed creatures will try to escape the object of their repulsion. If escape is not possible, they will at least keep their distance, and won’t willingly approach, though they may still attack the object of their repulsion at range. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. If the strength of this spell is greater than the natural Animus pool of the target, the target is repulsed by this spell.

### Sound 2 (Tiered – Manipulate):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Manipulate Sound energy changes existing sounds. A manipulate sound spell can silence, muffle, change, or amplify sounds. For example, the spell could silence a speaker, or change the words coming out of a speaker’s mouth, though the speaker may become bewildered when she hears the wrong words coming out of her mouth. A Manipulate Sound spell can increase a whisper to the volume of normal speech, or into a deafening roar. The sound to manipulate needn’t be audible to be manipulated. There is always ambient sound. One AP of Manipulate Sound energy is sufficient to change a sound into another sound of equal volume. To increase or decrease the volume requires an additional AP for each 10 decibels difference. By its very nature, sound energy travels. For every 10 feet away from a spell that has a target, the decibel level decreases by 1. For area effect spells using sound energy, the sound is contained within the area of the spell.

When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. Any creatures maintaining spells, performing delicate skills, or performing complex maneuvers within the affected area must make a Focus check. Creatures with Focus checks that meet or exceed the strength of the spell are unaffected. The concentration of creatures whose Focus checks fail to meet or exceed the strength of the spell is broken. Any creature whose Focus check is less than half the strength of the spell is effectively distracted, as their ears begin ringing.

Distracted creatures gain distraction tokens equal to the AP of the spell. Distracted creatures may only take single AP actions of no higher than simple difficulty while distracted. Every action taken removes a distraction token. Distracted creatures may attempt additional Focus checks to beat the strength of the spell at the cost of 1 AP each. If a subsequent Focus check beats the strength of the spell, all remaining distraction tokens are removed.

### Spatial 2 (Tiered – Dimensional):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Dimensional Space energy creates an extradimensional pocket with a 2-dimensional entrance. Extradimensional pockets from this spell can be anchored to the fabric of reality itself, or can be anchored to the entrance of an item, such as a bag or a chest. The entrance to the extradimensional pocket can only be seen from directly in front of it, though a creature or object passing through the entrance still goes into the extradimensional space. A space anchored to an item opens and closes as the item does. A space not anchored to an item can be opened or closed from inside. Initially, a space not anchored to an item has a doorway large enough for the caster to fit into it. The opening of the door can be as tall and/or as wide as the entire side of the internal dimension. A creature must be able to fit through the door to enter an extradimensional space. The duration of Dimensional Space energy is measured in hours. The first AP of Dimensional Space energy purchased creates a 9-cubic movement unit extradimensional pocket, appropriately sized for the caster. Each additional AP increases the length, width, and height of the pocket by 1 movement unit each.

### Teleportation 7 (Tiered – Swap):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Swap Teleportation energy switches the place of the caster or other target with a known creature or item, or the nearest creature or item of a specified type. This spell works like Summoning or Conjuring Teleportation energy, except that the destination of the summoned or conjured creature or item is the spot where the caster or other target was standing, and the caster or target is teleported to wherever the summoned or conjured creature or item was when the spell was cast. For example, if the caster has a statue in the caster’s likeness, the caster could swap places with that statue. If the statue is in roughly the same pose as the caster, or the caster accompanies this spell by a puff of smoke, onlookers may be fooled into thinking the caster was turned to stone, at the Keeper’s discretion. In reality, the caster would be standing wherever the statue was stored. If either of the creatures or items to be swapped can’t physically fit into the destination area, the spell fails. The first AP is sufficient to swap the caster (regardless of weight), or another target weighing no more than 100 lbs., with another creature or item weighing no more than 100 lbs. Each additional AP increases the maximum weight of a swapped target by 100 lbs.

### Temporal 5 (Tiered – Revise):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Revise Temporal energy rewrites a short segment of history. When this spell is cast, the caster specifies an action, or series of actions to be revised. The actions to be revised must be together in sequential order. Once this spell is completed, the results of the selected actions are rerolled. For example, if a foe killed an ally, this spell could force the foe to reroll the damage, potentially resulting in lower damage, and preventing the death of the ally. This spell revises only the specified actions. Any actions that have taken place since the revised actions are unaffected. Though casting this spell would normally cause a paradox in most cases, the history revision is minor, so all creatures involved in the revision are aware of the original and current timelines, and no paradox results.

The first AP of Revise Temporal energy is sufficient to revise the single action immediately prior to beginning this spell. Attempting to revise more actions, or revise actions further back increases the required AP. Each AP of Revising Temporal energy after the first is sufficient to increase the maximum number of actions earlier than this spell by 1, or increase the number of consecutive actions to be revised by 1. For example, to revise the single action that took place 3 actions before this spell would require 3 AP of Revising Temporal energy. To revise the 2 actions that occurred immediately prior to this action instead would require 3 AP. To revise 2 consecutive actions that occurred 3 actions prior to this spell (the action 3 actions before, and the action 2 actions before) would require 4 AP; 3 AP to affect the single action 3 actions before the spell, and another potential to affect the action that followed it. Cost calculations should always be ordered by the number of actions back, then the number of additional actions.

### Thought 4 (Tiered – Alter):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Alter Thought energy makes minor revisions to a target’s memories, subverts the attempts of others to read the caster’s mind, or gives casters a bonus equal to the strength of this spell on their Charisma check against mind reading spells. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. When used to alter the thoughts of a target, the target may make a Charisma check against the strength of the spell to prevent its effects. If the target fails their check, this spell allows the caster to change minor details in the target’s memory. The Keeper determines how minor a particular memory is. For example, the eye color of a friend of the target may be considered minor. All the memories of a person’s spouse, on the other hand, are fairly significant. When used in this manner, the caster may change a memory, or simply erase the memory. Each AP of Alter Thought energy used to alter or erase a target’s memory is sufficient to alter or erase 1 minor detail.  When used to subvert attempts to read the caster’s mind, the caster simply alters the details the caster is thinking of while the caster’s mind is being read, to give the reader false information. The minimum number of AP of Alter Thought energy required to subvert attempts to read the caster’s mind is equal to the number of AP of the mind reading spell.

## Structure

### Cloud (Shape):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

To cast a cloud shaped spell, the caster suspends the spell’s energy in the air. The cloud is lighter than air. A cloud shaped spell with no duration acts as a larger area burst shaped spell, but deals less damage. The energy in a cloud shaped spell is spread thin, so the cloud only deals ¼ of the normal damage to anything within the area. A cloud shaped spell starts as a spherical area with a diameter measured in increments of 4 movement units, appropriately sized for the caster, but immediately begins to spread out and rise. Each full round after the cloud is created, the cloud rises 1 movement unit, and its size changes, with its height cut in half and its diameter doubled, so long as it has room to spread. A cloud shaped spell cast under water will rapidly rise to the surface at a rate of 4 movement units per action. As the cloud rises to the surface, the height of the cloud is cut in half, and the diameter doubled for each movement unit. Any wind, magical or otherwise, pushes the cloud along at a rate equal to half the wind speed.

### Extended (Duration):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Extended duration spells continually deal damage over the course of the spells duration. An extended duration spell deals 1d10 damage per AP spent on the spell each round on the caster’s turn, for a number of rounds equal to the AP spent on the spell. For example, a 5 AP extended duration spell would deal 5d10 damage on the caster’s turn each round for 5 rounds.

When used with Concentration:

When an Extended spell is used in conjunction with concentration, it deals damage equal to the AP spent for each round concentration is maintained. The duration of the spell does not start until concentration is lost. All other structures must stay the same, but location may be changed as long as it remains within the spells range.


### Mist (Shape):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

To cast a mist shaped spell, the caster suspends the spell’s energy in the air. The mist is neutrally buoyant in air, and will essentially stay in place for the duration of the spell, unless acted on by outside forces such as wind. A mist shaped spell with no duration acts as a larger burst shaped spell, but deals less damage. The energy in a mist is spread thin, so the spell only deals 1/4 of the damage to anything within the area. A mist shaped spell starts as a roughly spherical area with a diameter measured in increments of 3 movement units, appropriately sized for the caster, and remains roughly the same shape, unless changed by outside forces, for the duration of the spell. A mist shaped spell is lighter than water, and will not sink into water. A mist shaped spell cast under water will rapidly rise to the surface at a rate of 4 movement units per action. As the mist rises to the surface, the height of the mist is cut in half, and the diameter doubled for each movement unit.  Any wind, magical or otherwise, pushes the mist along at a rate equal to the wind speed.

### Wall (Shape):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

To cast a wall shaped spell, the caster focuses energy into a semisolid sheet roughly 1 inch thick, in increments of 1 movement unit squares, appropriately sized for the caster. Walls needn’t be the same height or width, so long as the sections of the wall are built with 1 movement unit squares. The squares can even be formed into a tunnel or a box. Any viable target that comes into contact with the wall shaped spell feels the effects of the energy used in the spell. A creature passing through the wall shaped spell foregoes their ability to ward the effects of the spell, and is subject to the full effect of the spell whenever the effects occur, so long as they are in contact with the wall. Seeking spells can veer around wall shaped spells, unless enough wall shaped spells are in place to form a completely encompassing barrier. With the exception of Solid Force and Earth energies, spells that deal with solid matter are ineligible to be shaped as walls.

Wall shaped Earth energy spells can be used to create walls of hovering, dirt, sand, rock, or sharp, jagged stone. A wall of jagged stone causes damage to those trying to push their way through.

## Optional

### Bestowed:
> **Status:** ✅ CONFIRMED IN PRINCIPLE — transferred/persistent effect; later decisions govern carrier use and trigger behavior. Exact legacy numbers remain review material.

A bestowed spell is cast upon a creature or object, and acts as a charged spell cast by the creature or object. Unlike a conducted spell, the energy of the spell doesn’t dissipate if the object loses contact with the caster. Instead, the energy remains in the object until the object comes into contact with a viable target. Casters that aren’t confident in their ability to hit a target with the object should consider using a selective target. A creature carrying a bestowed spell is treated as having a charged version of the spell. The creature may use the spell as a counterspell, if the energy type is appropriate to do so, or may use the spell as an attack. Once cast, the structural components and energy type of the spell don’t change.

### Concentration:
> **Status:** ⚠️ REVIEW — maintaining an already enacted effect may consume AP; this is explicitly distinct from spending AP across turns to enact an action.

A concentration spell lasts for as long as the caster is able to maintain concentration on the spell. When a concentration spell is cast, the Specialist spends the full amount of AP on the spell as normal for the first round. For each subsequent round on the caster’s turn, the Specialist must spend additional AP to maintain concentration on the spell. The caster must spend 1 AP on the first subsequent round, 2 on the second subsequent round, and so on. The caster may use any remaining AP for movement if they so choose. If the caster is attacked while concentrating they must choose whether to defend against the attack or maintain concentration. If they choose to maintain concentration any damage mitigation provided by armor still applies.

When the caster takes damage, the caster is forced to make an Endurance check to maintain concentration. If the Endurance check exceeds the damage dealt, the caster maintains concentration. Otherwise, the casters concentration is broken, and any duration longer than instantaneous begins. See individual duration descriptions for further information about usage with concentration.

The caster may choose to drop the concentration at any time.

# Master

Master level energy is the strongest of all magic. Only the most dedicated casters ever reach this level of magical prowess. A Specialist must have at least 75 points in their primary casting stat to cast master spells.

## Energy

### Animation 6 (Tiered – Undeath):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Undeath Animation turns corpses into undead creatures. Creatures such as skeletons, zombies, mummies and others can be created. The more powerful the monster, the more AP of Undeath Animation are required. Undeath Animation has no duration. Once an undead creature is created, it lasts until it is destroyed. Animated undead are not under the control of the caster by default, though the caster could subsequently cast a dominate spell to control the undead. The initial Animus pool of the undead created is 1d10 for each AP spent on the spell. For the types of undead available, refer to the following table:

5-10 AP: Skeleton

11-15AP: Zombie

16-20 AP: Mummy

20+ AP: Vampire

### Charm 4 (Tiered – Dominate):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Dominate Charm energy has the potential to sway a creature’s disposition towards another creature or object so strongly that the creature may become reckless. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. If the target fails to ward the spell, add the strength to, or subtract the strength from the target’s disposition as appropriate. Dominated targets don’t automatically or immediately become suicidal, though the Dominating Charm spell may cause them to engage in actions that will undoubtedly be suicidal. For example, an obsessed creature will ignore its own safety to help the object of its obsession, and a recklessly hostile creature will fight to the death against any odds. An obsessed creature will follow any orders from the object of its obsession, including orders that will obviously result in death, such as “dive head first off that cliff.”

### Death (Elemental):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Death energy directly attacks the lifeforce of living creatures. Death energy only kills living targets. When used on undead creatures, Death energy works the way Life energy works on a living target. When this spell is cast, roll damage as normal. If the damage is sufficient to overcome either the Endurance Score or remaining Vitality Pool of the target, the target is slain outright. If the damage is insufficient to overcome the Endurance Score and remaining Vitality Pool of the target, this spell simply fails. If this spell is used on an undead creature, the creature’s Animus pool is fully restored. When used on the corpse of a formerly undead creature, if the strength of the spell is greater than the target’s natural Animus pool, the undead creature is restored to their undeath with full animus. Death energy is suitable to counter Life spells.

### Disintegrate (Primal):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Disintegrate energy destroys the covalent bonds between atoms in molecules. Disintegrate spells typically disintegrate entire creatures or objects, though a caster can choose only to disintegrate any portion of the target the energy touches. In order for a Disintegrate spell to work, the damage of the spell must overcome the current remaining Vitality pool of a living creature, the Animus pool of an undead creature, or the natural Structural Integrity pool of an object.

### Dispel 7 (Tiered – Prevent):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Prevent Dispel energy inhibits magic on various scales. A Preventative Dispelling spell cast on a creature prevents that creature from casting spells for the duration. When cast on a creature, the duration is measured in actions. A Preventative Dispelling spell cast on an area prevents all magic within the area. In this case, casters inside the area can’t cast spells at all, and casters outside the area can’t cast spells into, or through the area. When cast on anything other than a creature, the duration of a Preventative Dispelling spell is measured in hours. Any magic effects in place on an item are dispelled if the item is taken into a Preventative Dispelling area. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. The minimum AP is sufficient to prevent all magic for the duration of a Preventative Dispelling spell, though another Dispel spell used to dispel this spell must defeat the strength of this spell, such as a caster trying to dispel a Preventative Dispelling spell from a fellow caster.

### Divination 7 (Tiered – Visual):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Visual Divination energy allows the caster to spy on a target matching a description, and receive visual input only, without the aid of a reflective surface. The caster sees the distant events by merely closing his or her eyes. The caster can see events up to 10 miles away, but gets no other sensory input. Each AP of Visual Divination energy allows the caster to see an additional 10 miles away. Targets get an automatic Ward check against this spell.

### Divination 8 (Tiered – True):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

True Divination allows the caster to see, hear, smell, feel, and taste the surroundings of a distant place as though she were actually there. Without other means, the caster can’t directly interact with the distant event, though the caster can choose to feel things, or pass through them. The initial range of True Divination is 100 miles. Each additional AP of True Divination energy extends the range by another 100 miles.

### Explosion 5 (Tiered – Living):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Living Explosion energy causes living creatures to fly apart as shrapnel. When this spell is cast, roll for damage as normal. If the damage is insufficient to overcome the remaining Vitality pool of the creature, the spell fails. If the damage is sufficient to overcome the remaining Vitality pool of the creature, it bursts apart violently and sends shrapnel nearby. Shrapnel travels in a diameter of 1 movement unit, appropriately sized for the target. Shrapnel from soft creatures exploding impacts nearby creatures and objects, but only has a chance of harming very fragile targets. Hard creatures exploding send sharp, jagged shrapnel at nearby targets. In this case the caster makes a single ranged attack roll, and each nearby target defends against the attack roll. Any targets hit by the shrapnel take half the damage originally rolled for the target of the explosion spell.

### Fabrication 4 (Tiered – Produce):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Produce Fabrication energy seemingly creates raw materials from nothing, and shapes them into a finished product. This energy only conjures up normal materials. Special materials can be shaped with this energy, but the caster needs to have the special material physically within their possession to work it. In reality, the raw materials are drawn from the nearest source of raw materials available, regardless of distance. Produce Fabrication energy can’t make complex working machines, though it can make the components for such machines, including springs, wheels, gears, etc. Produce Fabrication energy requires a minimum of 1 AP for each cubic foot of the finished product. Products generated through this spell are the same quality as would be made by a novice. If the caster is trained in the appropriate crafting skill, they may increase the maximum quality by 1d10 for each AP spent on the spell, up to a maximum of their applicable skill.

### Flight 4 (Tiered – Soar):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Soar Flight energy lets a creature move any direction, other than through objects, at will. A soaring creature carries momentum and inertia, and is still treated a weighted creature, though it can move through the air with ease. A soaring creature requires a minimal amount of concentration to fly. Distraction won’t cause a soaring creature to fall, though unconsciousness, stunning, dazing, or any other condition that prevents the creature from conscious thought will. Soar Flight energy may be cast on objects. An object targeted by this energy moves as the caster desires for the duration of the spell. All weight limits still apply. Each AP of Soaring Flight energy grants flight to a creature or object weighing up to 25 lbs. Anyone wearing or holding the target object may make a Ward check to resist the Soaring Flight spell.

### Force 5 (Tiered – Immobilize):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Immobilize Force energy simply holds targets still, as if frozen in a block of ice. Objects under the effects of an Immobilizing Force spell are unable to be moved or damaged. Creatures under the effects of an Immobilizing Force spell become frozen in space. Immobilized creatures can’t take any action for the duration of the spell, nor can they be harmed. Immobilized creatures are able to think, but not cast spells. An immobilized caster may maintain concentration on a spell while immobilized, unless they get distracted, such as by bright flashes of light or loud noises. Immobilized targets don’t age or grow hungry, thirsty, or tired while immobilized. Anything the target was doing the instant it was immobilized is resumed immediately when the immobilization wears off. For example, a falling creature that became immobilized a few feet before hitting the ground would hit the ground as if it had never been immobilized once the spell ended. Each AP of Immobilizing Force energy is sufficient to hold up to 1 cubic foot.

### Gravity (Primal):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Gravity energy deals with the natural attraction between objects. A Gravity spell can make a target heavier or lighter, or shift the direction of gravity for the target. Each AP of Gravity energy is sufficient to increase or decrease the G-force on a target by 1. If the direction of gravity is changed, the first AP changes the direction, and AP beyond that increase the G-force. The minimum G-force a target can experience is 0. Reducing the G-force of a traveling object to 0 doesn’t stop the object, though it does make it weightless. This means a caster that is already falling at speeds of several miles per hour will continue to fall if reduced to 0 G’s. Reversing the direction of gravity for the same target, however, will slow their descent until their speed reaches 0, at which point they will begin “falling” the other direction. If timed properly, a caster could use this spell to prevent fall damage by first reversing gravity, then reducing it to 0 at the apex of the fall. Multiple uses of gravity spells could be used to simulate high speed flight, though doing so presents several risks.

### Illusion 4 (Tiered – Imperceptibility):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Imperceptibility Illusion energy removes the caster, or another object or creature designated by the caster, from the senses of the target. An imperceptible creature can’t be sensed by the target by any means for the duration of the spell. An imperceptible creature may still be harmed by the target. If the target gets injured by the imperceptible creature, the target doesn’t feel the injury itself, though the effects of the injury will most likely be readily apparent. For example, if the imperceptible creature cuts the target, the target doesn’t feel the cut, though it would be able to feel the blood trickling down, and would be able to see the blood. Targets with 20 points of Intelligence or Insight may become suspicious when an imperceptible target interacts with them, though they typically attribute any such interaction to phantoms or poltergeists. Any object the imperceptible creature manipulates also becomes imperceptible to the target, as long as the creature holds it. Even the minimum AP of Imperceptibility Illusion energy is sufficient to make the caster or 1 object or creature imperceptible to 1 target, though some casters use additional AP to prevent dispelling.

### Implosion 5 (Tiered – Living):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Living Implosion energy crushes living targets violently. When this spell is cast, roll for damage as normal. If the damage is insufficient to overcome the creature’s remaining Vitality pool, the spell fails. If the damage is sufficient to overcome the remaining Vitality pool, it collapses into a ball 1/100th the size of the original creature. The implosion of very large creatures can create a minor vacuum in the surrounding area, pulling light objects toward it, but creating barely more than a cool breeze for anything weighing more than a pound.

### Life (Elemental):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Life energy breathes the vital spark into the corpses of formerly living creatures. When used on undead targets, Life energy works the way Death energy works on a living target. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. If the strength of the spell is greater than the Endurance Score of the corpse, the corpse is brought back to life with full vitality. If used on a living creature, the creature’s Vitality pool is fully replenished. Only willing targets may be brought back to life. When used on undead creatures, if the strength of the spell is sufficient to overcome their natural Animus pool, the undead creature is reduced to a corpse. Life energy is suitable to counter Death spells.

### Merge 5 (Tiered – Living):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound, Prohibitive

Living Merge energy combines targets. Only willing targets can be combined, and any merge spell attempted on an unwilling target simply fails. Mindless creatures and creatures of animal intelligence are never considered willing targets, unless they’re being controlled, in which case the controller must be willing. Higher tiers of Merge energy allow a wider variety of targets to be merged, eventually allowing normal, living creatures to be affected. Any target may be combined with other targets from lower tiers as well. For example, a living merge spell can merge a living target with an object. In any merge spell, the largest target to be combined is considered the base of the resulting object or creature. Creatures merged into stationary targets maintain their senses, though they may be unable to move for the duration of the spell. For example, a caster that merges with a large boulder to hide from a goblin raiding party would still be able to see and hear as normal from within the boulder. While inside the boulder, the caster is immune to damage, so long as part of the boulder remains larger than the caster’s natural size. If the boulder explodes, or is crushed, however, and no piece larger than the caster’s natural size remains, the caster is killed, and her corpse is left in pieces no larger than the largest remaining piece of the boulder.

Living Merge energy combines un-living objects, undead creatures, unnatural, and/or natural living creatures into one. Natural living creatures, unnatural creatures, such as abominations and aberrations, undead creatures, corpses, stationary objects such as statues or walls, or up to false living animated targets, as well as non-stationary objects can be combined. For example, a caster could merge their arm with a whip, for extra reach. Living targets must have better than animalistic intelligence, and be willing, in order to be targeted with this spell. When casting this spell, the caster must declare the desired result. If the Keeper rules the result is not possible, the caster may opt not to cast the spell. Targets to be combined must be touching when the spell is cast. Each AP of Living Merging energy is sufficient to combine up to 1 cubic foot of objects, un-living, undead, natural living and/or unnatural living targets. Any number of objects and/or creatures may be combined so long as they are all touching at least 1 other target to be combined, and the combined total of the targets remain 1 cubic foot or less per AP of the spell.

### Mutation 4 (Tiered – Transmute):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Transmute Mutation energy permanently changes the chemical makeup of objects or liquids. Transmuted products are suitable for chemical research, or consumption if appropriate, and act in all ways as the real thing. However, transmuting does have some significant drawbacks. Not least of these drawbacks are forgery detectors; agents that patrol marketplaces looking for people trying to sell transmuted materials. Selling a transmuted material, in most places, is a more serious crime than selling a forgery. Transmuted gems are forevermore ruined as magical conduits. Any transmuted gem, even if transmuted back to the original gem type, shatters if used to conduct magical energy. Any liquid can be transmuted into any other liquid the caster knows. For example, the caster could turn water into wine, wine into water, poison into water, sea water into lamp oil, etc. Casters can only transmute things into their most basic, natural form, though they can be used by apothecaries and alchemists in other concoctions. Any poison or chemical with at least 1 transmuted component is treated as a transmuted substance. Each AP of Transmuting Mutation energy is sufficient to transmute up to 1 cubic centimeter of materials. Anyone wearing or holding the target object may make a Ward check to resist the Transmute Mutation spell.

### Poison (Primal):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Poison energy is used for the introduction or removal of toxins. Poisons are similar to disease, except that they act much faster, typically within hours, minutes, or even seconds. Poisons only work on living creatures. Poison energy afflicts the target with a normal poison. The toxin may last beyond the duration of the spell. Even the most basic instantaneous poison spell, delivered via touch, will cause the target to get sick, unless the target manages to resist the toxic effects.  Poisons cause various effects including weakness, impairment, paralysis, suffering, or even death. As with disease, a caster must diagnose the poison type, and create an antitoxin at least equally potent, to successfully counter the toxin. Attempting to cast an antitoxin spell without proper diagnosis carries the risk of not only failing, but introducing further toxin into the system of the patient. Unmodified Poison spells have a toxification period of 1 day before the symptoms take hold. Each AP of Poison energy is sufficient to either decrease the toxification period by 1 hour, to a minimum toxification period of a single action, or increases the severity of the poison symptoms inflicted or cured, as shown in the table below. The AP of a Poison spell determines how many symptoms the toxin will have. For example, if a Specialist used 13 AP, the Specialist could choose 1 symptom from the 10-21 AP section and 1 from the 1-3 AP section, or any combination of lower AP symptoms less than or equal to 13.

1-3 AP: Confusion, unconsciousness, pain, mild allergic reaction, nausea, diarrhea

4-9 AP: Disabled, immobilized, slowed, deafened, weakened, stiffness, moderate allergic reaction

10-21 AP: Blindness, paralysis, seizure, ataxia, suffocation, hemorrhaging, severe allergic reaction, sleep

22+ AP: Berserk, petrified, anaphylaxis, death

### Precognition 3 (Tiered – Prophecy):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Prophecy Precognition energy gives the caster insight into future events. The insight gained by Prophecy Precognition energy is often vague and confusing. Experiences often bombard the caster in rapid succession with no readily distinguishable reference to timeframe. Some images may be from the very near future, while others may be millennia away. After the spell is completed, the player may gain important insights that otherwise escape the party. The Keeper determines the appropriate images the player sees, and the overall message the player takes away from that. The message may be cryptic, or very clear, at the Keeper’s discretion. The minimum AP of Prophetic Precognitive energy is sufficient to have a premonition, though many casters use more AP to prevent counterspelling.

### Protection 4 (Tiered – Absorb):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: None

Absorb Protection energy reduces damage from other spells, and replenishes the protected creature’s Vitality pool. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. The strength of the spell determines the protection rating. This spell reduces damage from spells of the chosen energy type by up to the protection rating, potentially to zero points, and replenishes the protected creature’s Vitality pool by an amount equal to the damage reduced, for the duration of the spell. For example, if the caster chooses Fire energy, and rolls 23 points, this spell absorbs up to 23 points of Fire spell damage whenever the protected creature would otherwise take Fire spell damage. If, during the course of this spell, the protected creature is hit with 15 points of Fire spell damage, the protected creature takes no damage, but gains 15 Vitality points. If the protected creature is then hit with 27 more points of Fire spell damage, the protected creature absorbs the first 23 points into their Vitality pool, and takes the remaining 4 points of damage.

### Repulsion 4 (Tiered – False):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

False Repulsion energy gives false living animated creatures an aversion to the target. Repulsed creatures will try to escape the object of their repulsion. If escape is not possible, they will at least keep their distance, and won’t willingly approach, though they may still attack the object of their repulsion at range. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. If the strength of this spell is greater than the natural Structural Integrity pool of the target, the target is repulsed by this spell.

### Spirit (Elemental):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Reduce, Negate, Rebound, Absorb

Spirit energy deals with the soul. Spirit energy is often called “ectoplasm”. Spirit energy can disrupt a soul’s connection with its body, reattach a soul to its body, or even harm a ghost as though it were a solid object. Spirit energy doesn’t deal damage to the living. Instead, it directly attacks the spirit. To cleave a soul from its body, the caster must deal more than the target’s Endurance Score or remaining Vitality Pool in Spirit energy based damage. Cleaving a soul from the body does not cause automatic death. Instead, the body continues to function, but goes into a completely vegetative state, similar to a coma. Left untended, a vegetative body will eventually die of starvation or dehydration. A single AP of Spirit energy is sufficient to reattach a ghost to its body, provided the body is available, and still alive. If the body is no longer alive, other means must be taken to rekindle the life force of the body. Spirit energy may also be used as an attack against ghosts and other incorporeal beings. When used to attack incorporeal creatures, Spirit energy deals maximum (10 points per AP spent on Spirit energy) damage on a successful hit.

### Teleportation 8 (Tiered – Unknown):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Unknown Teleportation energy sends the caster or other target to any area within range, even if the caster is unfamiliar with it. The destination can be chosen by specifying features, such as a waterfall or palm trees, or the destination can be chosen by specifying a direction and distance. If the destination is chosen by specifying features, the caster or target is teleported to the nearest place that closely matches the description. If the caster specifies impossible conditions, such as a house on a bed of lava, the Keeper determines which of the specified criteria are met, in this case sending the target to the nearest house or the nearest bed of lava. This spell can send the target to a specific place, but only if the caster has been given a detailed and accurate description of the destination. For example, if the destination is the cargo hold of the ship La Maison du Mer, the spell works, so long as the description of the cargo hold was accurate, and the cargo hold is still intact. If, on the other hand, La Maison du Mer lies in pieces at the bottom of the ocean, the Keeper decides if this spell takes the caster to the nearest similar cargo hold of a ship, or to the cargo hold of La Maison du Mer at the bottom of the ocean. If the destination is specified by direction and distance, the target will appear at that spot, so long as the spot specified isn’t inside solid matter. If the specified location is inside solid matter, the target appears in the nearest area that is not in solid matter. The destination of an Unknown Teleportation spell may or may not be safe. For example, the caster can purposefully teleport a target above a group of jagged rocks, or the caster may accidentally specify a direction and distance that places the target just outside the wall of a sheer cliff. The minimum AP of this spell is sufficient to teleport the caster (regardless of weight) or another target weighing no more than 200 lbs. Each additional AP increases the weight limit by 200 lbs.

### Teleportation 9 (Tiered – Portal):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Portal Teleportation energy creates a 2-way wormhole between 2 points, both of which are the origination and destination simultaneously. The caster needn’t be familiar with either point. The destination can be chosen by specifying features, such as a waterfall or palm trees, or the destination can be chosen by specifying a direction and distance. If the destination is chosen by specifying features, the destination of the portal appears in the nearest place that closely matches the description. If the caster specifies impossible conditions, such as a house on a bed of lava, the Keeper determines which of the specified criteria are met, in this case putting the destination portal close to the nearest house or the nearest bed of lava. This spell can create a destination portal in a specific place, but only if the caster has been given a detailed and accurate description of the destination. For example, if the destination is the cargo hold of the ship La Maison du Mer, the spell works, so long as the description of the cargo hold was accurate, and the cargo hold is still intact. If, on the other hand, La Maison du Mer lies in pieces at the bottom of the ocean, the Keeper decides if this destination portal appears in the nearest similar cargo hold of a ship, or to the cargo hold of La Maison du Mer at the bottom of the ocean. If the destination is specified by direction and distance, the destination portal will appear at that spot, so long as the spot specified isn’t inside solid matter. If the specified location is inside solid matter, the destination portal appears in the nearest area that is not in solid matter. The destination of a Portal Teleportation spell may or may not be safe. For example, the caster can purposefully put the origination portal under a foe, and the destination portal above a group of jagged rocks, or the caster may accidentally specify a direction and distance that places the destination portal just outside the wall of a sheer cliff.  Creatures on either side can see through the portal to the other side clearly. A creature can even stick its head through and look around before deciding whether or not to step through the portal. The portal created by this spell works just like a doorway. When this spell is cast, the Keeper may allow the caster to specify that the portal simply shunts any creature or object that is partway through the portal to whichever side the majority of the creature or object is on when it closes, or the caster can specify that if a creature or object is partway through the portal, the portion of the creature or object on each side stays on that side, meaning the creature or object is sliced in 2 or more pieces. The Keeper may also specify that something else happens to a creature or object partway through the portal when it closes, for example, it may end up partway between the 2 sides of the portal, closer to the side the majority of the creature or object was on when it closed. The first AP of Teleportation Portal energy is sufficient to create a portal with an opening 1 movement unit in diameter, appropriately sized for the caster. Each additional AP increases the maximum size of the portal by up to 1 movement unit. This spell has no range limitations. If there is a difference in pressure between the 2 sides of a portal, the Keeper decides whether or not the higher-pressure side bursts forth into the lower-pressure side, or the Keeper may allow the player to decide.

### Temporal 6 (Tiered – Suspend):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Suspend Temporal energy removes the target from the time stream temporarily. The target of this spell reappears on the caster’s action in the same location and orientation it was in when this spell was cast after the spell’s duration. If any creature or object occupies the space where the creature was suspended when it reappears, the suspended creature instead reappears in the nearest unoccupied space. The first AP of Suspending Temporal energy is sufficient to suspend the caster (regardless of weight) or another target, weighing no more than 100 lbs, for the duration of the spell. Each additional AP increases the maximum weight limit of the target by 100 lbs.

### Temporal 7 (Tiered – Erase):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Erase Temporal energy removes a target from the fabric of reality. Erasing anything from time has the potential to cause a huge paradox. Your Keeper may determine that a particular figure is simply too powerful, or too integral to the world to be erased. The absolute minimum number of AP required to erase a target is the total sum of all the ranks the target has in all categories. Before this spell is cast, the Keeper determines how important to the timeline the specified target is. Very prominent figures, such as kings and mayors, who are well known to many, are considered to be very important. Lesser known targets, such as peasants or livestock aren’t considered to be particularly important. The Keeper may add additional ranks to the minimum rank requirement for very important targets. If this spell succeeds, the target is removed from existence. The results of any actions the creature has taken remain in place, and reality is revised only slightly. If the target was a leader or dictator, the next likely candidate fills the target’s place, and all actions attributed to the target in the past are now attributed to the replacement. The replacement may have a different mindset, and future actions may be of a different nature, though nobody questions the change, and only the caster recalls the original events. Any offspring of the target are likewise removed from reality, though the replacement may have children. The number of AP required to cast this spell is determined by your Keeper.

### Thought 5 (Tiered – Control):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Protection: Negate, Rebound

Control Thought energy alters the target’s perception of others. The caster can sway a creature’s disposition toward friendly or unfriendly. The target’s disposition change may be towards the caster, or it may be towards another target designated by the caster. For instance, the caster may shift a troll’s disposition toward a locked door to hostile, so the troll will attack the door. When this spell is cast, roll damage as normal. Instead of dealing damage directly, the damage rolled sets the strength of the spell. If the target fails to ward the spell, add the strength to, or subtract the strength from the target’s disposition as appropriate. Influenced creatures maintain their sense of self-preservation. Though an influenced creature may be hostile toward an obviously stronger foe, it may not attack if attacking would be suicidal.

## Structure

### Ball (Shape):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

To cast a ball shaped spell, the caster gathers energy into a semisolid, spherical area with a diameter measured in increments of 1 movement unit, appropriately sized for the caster. The ball shaped spell fills a diameter measured in 1 movement unit increments. Anything inside, or in contact with the ball shaped spell feels the effect of the energy used in the spell. A creature purposefully entering the ball shaped spell foregoes its ability to ward the effects of the spell, and is subject to the full effect of the spell whenever the effects occur. Unless the ball shaped spell is solid and opaque, the ball is noticeably different than a sphere-shaped spell, even from the outside.

### Intensifying (Duration):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Intensifying duration spells hit hard and only get worse from there. An intensifying spell lasts a number of rounds equal to the AP spent on the spell. On the first round, it deals 1d10 for each AP spent on the spell and gains one additional d10 each subsequent round of the spells duration on the caster’s turn. For example, a 5 AP intensifying spell would deal 5d10 on the first round, 6d10 on the second and so on until the fifth round where it would deal 9d10 damage.

When used with Concentration:

When an Intensifying spell is used in conjunction with concentration, the spell starts at 1d10 for each AP spent and builds by 1d10 for each subsequent round concentration is maintained. The spell will continue to intensify for a number rounds equal to AP spent after concentration is lost. All other structures must stay the same, but location may be changed as long as it remains within the spells range.

### Sculpted (Shape):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

To cast a sculpted spell, the caster forms energy into a shape of the caster’s choosing. The caster may choose to make the shape hollow or semi-solid, though the cost is always determined as though the shape is solid. For example, a 1-foot diameter sphere would cost the same to shape as a 1-foot diameter ball, a hollow 1-foot cube, or a solid 1-foot cube. A Sculpted spell can match the size and shape of any object the caster can imagine, limited only by the caster’s AP. Sculpted spells are measured in 1 movement unit increments, appropriately sized for the caster.

### Selective (Target):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

Selective targeting allows the caster of a spell to specify recipients of any effects of the spell from within a group, or within the area of a spell. For example, if a Specialist casts a selective Positive energy spell in an area, the Specialist may stipulate that only members of their party benefit from the effects. Conversely, if several of a Specialist’s party members have tackled an opponent, and are holding said opponent down, the Specialist may cast a spell on the whole group, and specify that only the foe is affected.

### Sphere (Shape):
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

To cast a sphere-shaped spell, the caster focuses energy into a semisolid bubble, roughly 1 inch thick, in a diameter measured in 1 movement unit increments, appropriately sized for the caster. Any viable target that comes into contact with the sphere-shaped spell feels the effects of the energy used in the spell. A creature purposefully entering the sphere-shaped spell foregoes its ability to ward the effects of the spell, and is subject to the full effect of the spell whenever the effects occur. Seeking spells can’t penetrate a sphere. Unless the sphere-shaped spell is solid and opaque, the sphere is noticeably different than a ball shaped spell, even from the outside. A sphere-shaped spell is considered to be a completely encompassing barrier.

## Optional

### Controlled:
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

To cast a controlled spell, the caster determines the effects of the spell, and the spell’s effects come into being within 1 movement unit of the caster, appropriately sized for the caster (in such a way that the caster won’t be harmed by the spell, if the spell is harmful). From there, the caster can move the effects of the spell with a thought on his or her turn. The spell moves as the caster desires, including horizontally and vertically, but is blocked by solid objects. A controlled spell must have a duration longer than instantaneous. The Speed Rating of the spell is based on the caster’s Intelligence or Insight score (whichever was used as the primary Magic stat). For the duration of the spell, the caster may move the effect of the spell up to its Speed Rating on his or her action. Controlling the spell is a passive action, and can be done in conjunction with other actions, including casting other spells.

### Seeking:
> **Status:** ⚠️ REVIEW / CONVERSION — preserve the magical concept and tier placement as evidence; audit AP, potency, range, targets, durations, fixed numbers, and any legacy resolution language against the modern engine.

To cast a seeking spell, the caster gathers energy into a small, semisolid, ball-like object. The object appears to be made of the energy used, and forms roughly the shape of a ping pong ball. Once formed, the ball speeds toward the target as though it had been fired from a bow in 2 movement unit increments, appropriately sized for the caster. The seeking spell will make course corrections of up to 90 degrees for each 2 movement units it flies, as needed. A Seeking spell can’t turn 90 degrees within a corner connecting 2 sections of a hallway if each is only 1 movement unit wide, for example. The spell can hit any known target that isn’t completely encompassed by a barrier. Even a thin sheet of glass can prevent a seeking spell from reaching its target. A target inside a completely closed room, surrounded by a sphere-shaped spell of Solid Force energy, or even completely enclosed in a sphere made of shaped glass can’t be hit by a seeking spell. In such a case, the spell will hit an intervening barrier as close to the target as it can.


---

# Chapter 7 — Creatures & Traits

## Reconstruction status legend

- **✅ CONFIRMED** — established by later explicit decisions and treated as current canon unless deliberately reopened.
- **🔄 SUPERSEDED** — recovered source material that has been replaced by a later decision.
- **⚠️ REVIEW / CONVERSION** — concept or content is useful, but one or more mechanics must be reconciled with the current engine.
- **⬜ NEEDS DEVELOPMENT** — incomplete or absent; substantial design work remains.
- **❗ CONTRADICTION** — two surviving sources or decisions conflict and must not be silently reconciled.
- **💡 SUGGESTION** — design suggestion from this reconstruction pass; not canon unless Mike approves it.

**Authority used in this reconstruction:** newest explicit decisions in the current reconstruction work override older text; CLEAN source files are the baseline for material not subsequently changed. Archival Markdown is treated as a searchable transcription of its CLEAN source, not as independent canon. No discrepancy has been silently fixed.

## 1. Current Creature Type philosophy

**✅ CONFIRMED architecture**

Creature Types such as Dragon, Humanoid, Elemental, Ghost, Demon, Goblin, etc. are **classifications/collections/descriptions of Traits**. The Type itself has no separate point cost. The Traits that make the Specialist qualify for the Type **do have their normal mechanical costs**.

A Specialist must possess a substantial portion of the listed/associated Traits to reasonably adopt that Creature Type. The exact mechanical threshold for "substantial portion" remains **⚠️ REVIEW**.

There are no racial set bonuses merely for completing a Type. Capabilities come from the underlying Traits.

## 2. Trait economy and permanence

**✅ / ⚠️ current framework**

- Tiered Trait costs generally follow **3 / 6 / 9 / 12 / 15** for Simple / Basic / Intermediate / Advanced / Master.
- Some Traits are fixed-cost rather than tier ladders.
- Negative Traits are genuine hindrances/narrative complications. At creation they grant points that can be spent elsewhere. If gained during play, they do not grant points.
- Players cannot voluntarily remove/downgrade Traits to reclaim points or use Traits as a point bank. Gameplay may alter a Trait; if gameplay reduces a previously purchased positive Trait, it may later be purchased again.
- **❗ Creation-pool conflict:** later working material uses a 100-point pool including Stats and Traits, while CLEAN Specialist Basics uses 100 Stat points plus starting Advancement Points. This remains unresolved.

## 3. Anatomy and natural combat

**✅ Current anchors**

- Natural weapons are weapon profiles and are alternatives to manufactured weapons for an attack unless a Component explicitly combines them.
- Natural weapons are tiered; appropriate Training may apply.
- Natural armor does not stack with worn armor; worn armor overrides it.
- Extra Limbs: current working cost +9 for +2 limbs; repeatable. Extra limbs do not directly multiply actions; AP remains the activation resource.
- Less Limbs: current working negative Trait -9.
- Tentacles: Basic 6, prerequisite Pseudopod in later work.
- Torso/body-plan options include Cephalothorax; spider-style builds should use body plan + limbs rather than a bespoke race exception.

## 4. Skins

**✅ Current framework**

A Specialist may possess multiple skins for appearance/utility, but only one designated **Dominant Skin** grants the combat benefit chosen at creation. Natural skin armor does not stack with worn armor.

Recovered/current skin concepts include Barbed→Quills, Bark, Elemental, Crystalline (Full/Partial), Exoskeleton, Feathers, Hairless, Hirsute, Mucus→Adhesive, None, Photosynthetic, Scales, Secretion branches, Shell, and Thick Hide.

Known exclusion examples from later work:

- Hairless excludes Feathers, Hirsute, Bark, Elemental, Crystalline, Photosynthetic, Scales.
- Hirsute excludes Bark, Crystalline, Elemental, Photosynthetic, Scales, Slime, Shell.

**⚠️ REVIEW:** complete prerequisites/exclusions and exact mechanical benefits.

## 5. Wings, flight, Size, and movement Traits

**⚠️ REVIEW with strong current direction**

- Wing progression: Vestigial → Hover → Glide → Full Flight, sequential.
- Earlier working total investment for Full Flight was 45 points.
- Exact flight/movement values depend on the final Size→MU chart.
- Wingless Flight may require Incorporeal; advanced wing prerequisites such as Lightweight were discussed but not fully locked.
- Size itself is tiered in both larger and smaller directions and affects MU; exact chart remains open.

## 6. Senses

**✅ architecture:** sensory Traits use fixed assigned costs/tiers rather than every sense having a five-step generic ladder. Exact senses and exclusions require entry-level review.

## 7. Unnatural Hunger

**✅ latest correction / ⚠️ full Trait wording still needs pass**

Unnatural Hunger must **not modify AP**. Speed remains the sole AP source.

Current starvation penalty: **-1d10 to all rolls per tier per day of starvation**. Feeding/recovery details should be taken from the already-developed Trait text and reconciled during the Trait pass; any CLEAN/Integrated AP penalty is superseded.

**💡 Balance flag:** the literal stacking rate can become very severe quickly. Preserve it as the current decision, but stress-test it before final publication prose.

## 8. Example creature constructions from later decisions

- Giant Spider: Cephalothorax + Extra Limbs ×2 for eight appendages; do not use an arbitrary arm-removal workaround; fangs/bite purchased normally.
- Ghoul: Unnatural Hunger (living flesh) + Putrid negative Trait.
- Harpy: Wings + tiered Beak.
- Goblin: tiered Fangs.
- Plant creatures are not automatically rooted.

## 9. Recovered creature-type and Trait catalog

The following CLEAN WIP is **evidence, not a set of mandatory race packages**. Descriptions and trait associations are useful for defining what qualifies as a Creature Type. Any baked-in package costs, unique subsystems, or assumptions that conflict with the modular Trait framework must be converted.

---

# Creatures


No fantasy setting would be complete without fantastic and magical creatures roaming the world. We have attempted to keep our mythological creatures as historically accurate as possible. Not all the creatures below are mythological, as there are creatures in reality that have the potential to be fascinating and/or dangerous encounters as well.


While there are a vast number of creatures available in history, we didn’t feel they all have a place within this game. Some creatures are either too obscure or too specific for our purposes. We have especially tried to avoid any creature that could be described as “the” whatever, such as Medusa. Keepers are welcome to use unique creatures, but we discourage you from using them more than once.


# Creatures Types

Below are the creatures in Boundless. While they are intended to be playable, make sure to obtain Keeper approval before you begin to roll your Specialist with a certain creature type.

## Changelings

### Description
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

A changeling is any creature or object used to replace any living child.

Some changelings are replicas of children, carved from enchanted, living wood. The enchantments that give these changelings life are short-lived, and the “child” appears to become sickly and die shortly after the switch is made.


Some changelings are actually troll or fae children, swapped with another child for various reasons, typically to prevent in-breeding, or because being raised by the new parents is looked upon as “luxurious”. If undetected, these children either grow up thinking they are genuine members of their new family, or they remember their true nature, and will return to their original family later in life.


Some changelings are elderly fae, nearing the end of their lives. These changelings are exchanged so the elderly fae can live out their final days being pampered by their “new parents”.


Any changeling that lives more than a short while will act as any child would in its place for as long as it stays with its new parents.

### Available creature traits
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Shape-shifter

Fae

Elemental (Earth/ Wood)


## Dwarfs

### Description
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

All dwarfs are wise, industrious crafters. Dwarfs are typically gruff and abrasive in their interactions with other creatures, and show respect only to beings they deem worthy of high praise, typically beings which humans would describe as “angelic” or “godly”. Dwarfs happily do the bidding of these “angelic” or “godly” creatures without asking for anything in return. There are two types of dwarf.


Earth dwarfs live deep underground near sources of molten rock. These dwarfs use the heat of the molten rock to forge strong metals, and mysterious artifacts. Earth dwarfs tend to have little hair and dark, leathery skin, due to their perpetual proximity to intense heat. These dwarfs have trouble seeing in normal lighting conditions, preferring instead the bright illumination provided by molten rock. For this reason, earth dwarfs rarely venture away from their sources of molten rock. Some earth dwarfs live in volcanoes as well. While volcanoes can be tall, like mountains, the dwarfs inhabiting them are still considered earth dwarfs, and are not to be confused with their cold-weather cousins, the mountain dwarfs.


Mountain dwarfs live underground, high up in the mountains. Due to the very cold nature of their homes, mountain dwarfs tend to be heavyset, having a lot of body fat to insulate their warmth, and very hairy, and often sport long, thick beards. Just like earth dwarfs, mountain dwarfs are craftsmen, though they tend to avoid intense heat, as it may cause avalanches. Instead, they work with more malleable metals, such as gold and silver. Mountain dwarfs also develop the ability to see in complete darkness. While their eyes can adjust to normal lighting conditions, the process takes a while leaving the mountain dwarf effectively blinded during the transition. In very hot seasons, when the mountain snow melts, mountain dwarfs often venture outside and cold-forge items from iron. Cold-forged iron weapons are feared by most fae creatures.

### Available creature traits
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Stat bonus: Stamina and Proficiency

Stat penalty: Looks and Charisma

Hirsute (Mountain dwarf) – aesthetic, automatic

Hairless (Earth dwarf) – aesthetic, automatic

Night vision – automatic

Thick hide (Mountain dwarf) – automatic

Stout – automatic


## Ghouls

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Ghouls are demons, appearing to be gaunt, pale, hairless humans. Ghouls subsist on a diet of human flesh and bones. While they prefer fresh corpses, they aren’t terribly picky, and are known to eat the remains of long-dead, rotten corpses. Ghouls live underground, typically in the desert, and always near a source of corpses, such as recent battlefields, or cemeteries. Ghouls are known to shape-shift into hyenas to hunt. Though sunlight isn’t harmful to ghouls, they tend to avoid sunlight, as their coloring is more suited to hunting at night. Ghouls have long claws, and maws full of long, sharp, jagged teeth. Ghouls use their claws and powerful muscles for digging, tunneling, ripping open coffins, and tearing the living into pieces, either in defense or offense. Ghouls also have large mouths, and powerful jaws, capable of biting through and chewing bone and flesh alike.

### Available creature traits
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Unnatural hunger (dead and/or rotting flesh) –automatic

Ghastly – automatic

Putrid – automatic

Demonic – automatic

Night vision

Claws – automatic

Toothy maw – automatic

Shape-shifter (hyena)

Non-tasting (No taste) – automatic


## Goblins

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Goblins are ugly creatures that are anything but likeable. They range from the size of young children to full grown adult humans. At best, goblins are mischievous, and at worst, they are malevolent. The term “goblin” doesn’t refer to a particular species, but instead is used to refer to any of the more unfriendly fae. The fae kingdom deals in dichotomy, meaning for every good type of faerie, there is a similar, often grotesque version. Some goblins are known to steal human children, and replace them with changelings. If these stolen children are of a mischievous nature, they are typically raised to become goblins themselves. If the children are pure and innocent, they are usually either corrupted, to be raised as goblins, or they’re consumed by the goblins in one fashion or another.

### Available creature traits
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Ghastly – automatic

Putrid

Size

Fae – automatic

Stat penalty: Looks and Charisma

Claws

Toothy maw


## Harpies

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Harpies are medium sized creatures with the heads and torsos of beautiful women, and the wings, tails, and feet of large birds of prey. The word “harpy”, roughly translated, means “snatcher”.

Harpies, as a species, have adapted survival techniques that involve luring and seducing human or humanoid males into mating with them. Not all harpies are evil or malevolent by nature, though all are fierce when threatened. Harpies are loathed by hunters, as the harpies tend to release captured animals from snares and other traps.

### Available creature traits
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Wings – automatic

Hover – automatic

No arms/hands – automatic

Gender – Female – automatic

Stat bonus: Looks, Charisma

Claws

Feathers - aesthetic

Light-weight


## Imps

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Imps are small, ugly creatures that feed on laughter, either the laughter of others or their own laughter. Imps are lonely, having a tendency to make friends by playing jokes on them. Any friend the imp makes doesn’t stay a friend very long though, as the imp continues to play jokes and pranks on their new friends. While the jokes imps play aren’t particularly malicious or harmful, they are often very annoying. Some imps have wings, while others don’t. Some imps are capable of shapeshifting into small animals, such as toads, weasels, or cats. Only winged imps can shapeshift into winged creatures, though a winged imp may assume the form of a non-winged creature.

### Available creature traits
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Demonic – automatic

Size (Tiny) – automatic

Light-weight

Stat penalty: Looks

Winged

Shape-shifter (small animals)

Prehensile tail

Unnatural hunger (laughter) – automatic


## Kelpie

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Kelpies, or water horses, appear as white, grey, or black ponies. Kelpies lure victims away, drag them underwater, and devour them. Most children are easily lured by the appearance of kelpies, as children mistake them for ponies, and want to go for a ride. Once the child touches the kelpie, the kelpie’s skin becomes adhesive, instantly bonding to the child. The adhesive is so strong, only severing the attached part will free a victim from the kelpie. Kelpies can choose to make their skin adhesive or non-adhesive at will. To lure men, kelpies are known to shapeshift into beautiful women to entice them.  Regardless of the form a Kelpie takes, its mane, or hair, always appear to be dripping wet, and may appear to have seaweed in it.

### Available creature traits
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Four legs – automatic

Tail – automatic

Unnatural hunger (humanoids) – automatic

Amphibious – automatic

Shape-shifter (humanoid)

Mucus – adhesive (skin) – automatic


## Kappa

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Kappa are small, humanoid creatures with the shells and beaks of turtles, and webbed fingers and toes, with skin colors ranging from blue to yellow to green. Kappa are generally tricksters, though some may be friendly, and others may be fiendish, depending on their mood at the time. Kappa have small divots in their heads, called the sara, which holds water from their home whenever they’re on land. It is said that tricking a kappa into emptying this sara is the easiest way to defeat him. If this sara is emptied, the kappa is paralyzed, and begins to dry out. Even a dried-out kappa may be restored to life by placing water from his home in the sara. In the water, kappa swim as quickly and nimbly as fish and able to hold their breath for extended periods of time.


Kappa are fond of wrestling and other shows of strength and skill. It is said kappa can’t resist a challenge, and when challenged, will follow the challenge to the letter. It is also said that Kappa are insistent upon being courteous, and will return any gesture of respect shown them. Kappa are also known for drowning and devouring small children, or opponents that lose challenges. The only food kappa enjoy more than small children is cucumber.

### Available creature traits
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Size (small) – automatic

Beak – automatic

Shell (turtle) – automatic

Webbed hands/feet – automatic

Unnatural hunger (children, cucumber) – automatic


## Knockers

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Knockers, also known as tommyknockers, are small, grizzled humanoid figures. They are typically found in mines, and usually wear miniature versions of mining gear. Knockers got their name from the knocking sound they make on the walls of mines just before cave-ins. Some believe the knockers do this as a warning. Others believe they do this with malicious intent, and cause the cave-ins. Regardless of whether the knocking is viewed as a warning or an attack, miners keep a wary ear out in the tunnels for the knocking, and dread the sound of it.

### Available creature traits
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Size (small) – automatic

Stat penalty: Looks

Fae – automatic


## Kraken

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Kraken, also known as giant squid, are sea dwelling creatures that typically live in the deepest depths of the oceans, and surface on rare occasion either to feed, or to respond violently to disturbances. Kraken can grow to be massive, with tentacles capable of crushing seagoing vessels, and beaks capable of biting through them.

### Available creature traits
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Invertebrate – automatic

Beak – automatic

Tentacles, eight – automatic

Size (gigantic) – automatic

Water breathing – automatic

Night vision – automatic

Imposing – automatic

Mindless


## Kirin/Qilin

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Kirin are very similar to Qilin, but with a few differences; primarily the body of the Qilin is that of an ox, whereas the body of a Kirin is that of a deer. Kirin and Qilin both have the head of a dragon. Kirin has the tail of an ox, while Qilin has the tail of a lion. Kirin have deer like antlers on their heads, while Qilin have only a single antler-like horn. Both Kirin and Qilin have manes that appear fiery, and are covered in scales which resemble the scales of a snake or fish.


Despite their physical differences, Kirin and Qilin are nearly identical in their actions. Both have the ability to walk without trampling grass or flowers underfoot, and both live on diets devoid of meat. They can also exhale blasts of flame, and have a roar as loud as thunder.


Kirin and Qilin are also closely associated with sages, and exemplary people. It is said a Kirin heralded the birth of Confucius, carrying a scroll stating a baby to be born would exemplify all that is good in men. Late in Confucius’ life, he was informed that an “elk” had been injured, and when he went to help the animal, he discovered that it was actually a Kirin that had been mortally wounded. Because of this story, it is believed that only those with pure hearts can see Kirin or Qilin for what they truly are.

### Available creature traits
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Four legs – automatic

Horns – automatic

Scales – automatic

Tail – automatic

Imposing


## Leprechaun

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Leprechauns come in two sorts; trouping and solitary. Trouping leprechauns wear green finery, whereas their solitary brethren wear red. Leprechauns typically appear as small middle-aged to elderly men no larger than a young child. Leprechauns enjoy revelry, and are known to party much of the time. They also enjoy pranks, and have a reputation for being tricksters. Leprechauns are neither wholly good, nor wholly evil, but are somewhere between. Leprechauns are capable of becoming invisible at will, and are very hard to spot.


Leprechauns are known for having a secret crock of gold, which they hide at the end of a rainbow. If a Leprechaun is ever captured, they can grant the one who captured them a single wish. Rumors say they can grant three wishes, but this is likely based on the story of a king who fell asleep on the beach, and awoke to find himself being dragged into the ocean by three leprechauns, each of whom granted the king a wish in exchange for their freedom. The captor of a leprechaun may, instead of a wish, demand the leprechaun’s crock of gold, though such an action will forever put the captor and all descendants of the captor at odds with leprechauns, who will forever go out of their way to make life miserable for the family, until such time as all the gold is back where it rightfully belongs.

### Available creature traits
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Size (small) – automatic

Fae – automatic


## Manticore

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Manticores are odd creatures with the bodies of red lions, the head of a man with three rows of sharp teeth, and the tail of a scorpion. Some accounts of Manticores would claim them to have wings, though this is likely due to their ability to leap great distances. Very old Manticores grow horns like those of a goat. Manticores can shoot barbs from their tails, which are coated in a potent paralytic poison. When Manticores eat their prey, they devour them in their entirety, including clothing and equipment, which it digests thoroughly. Manticores also have a loud, trumpet-like roar. Manticores prefer their food to be living, and will ignore undead prey, unless provoked.

### Available creature traits
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Size (large) – automatic

Toothy maw – automatic

Four legs – automatic

Claws – automatic

Tail – automatic

Venomous (tail) – automatic

Wings – scalable

Imposing


## Merfolk

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Merfolk are aquatic fae, with tails of fish from the waist down, and humanoid features from the waist up. While they are capable of breathing in air, they don’t like being out of water too long in their aquatic form, though they have a sea-skin which they can remove to appear human. If their sea-skin is ever misplaced or stolen, they will spend the rest of their lives looking for it.


Merfolk emotions are foreign to surface dwellers, and often difficult to understand. Mermen are notoriously ugly, and avoid the surface altogether. Mermaids, on the other hand, are notoriously beautiful, and very curious of the surface. Some mermaids are simply curious, and benign, and find surface dwellers beautiful compared to mermen. As a result, some mermaids fall in love with surface dwellers. Other mermaids are angry and vengeful of surface dwellers encroaching on the sea, and do whatever they can to cause the death of seafarers. Some simply lure fishermen into the water, and drown them, while others are able to cause violent sea storms capable of capsizing entire ships.

### Available creature traits
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Fae – automatic

Stat bonus: Looks (female)

Stat penalty: Looks (male)

Gills – automatic

Amphibious

No legs (fish tail) – automatic

Scales (waist down) – automatic


## Phoenix

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Phoenix are large, brightly colored birds of prey. Their cry is melodious, like a song sung by a choir. A phoenix has very oily, golden feathers. When viewed in the light, the iridescent nature of the phoenix oil makes the phoenix appear to be aflame. The strong magical nature of the phoenix makes them aware when a very powerful artifact is created by the earth or mountain dwarfs. Phoenix are strongly attuned to all artifacts, and protect them at all costs. A phoenix lives roughly 500 years, during which time it is capable of gliding perpetually. A phoenix only ever touches down if provoked, such as by a great tragedy, or by an artifact being tampered with. At the time of the phoenix’s death, it bursts into flames, and violently explodes, reducing anything in a 30 foot radius to ash, and sending a mushroom cloud into the sky. Once the mushroom cloud and smoke subside, the egg of a new phoenix rests in the center of the crater, and hatches within minutes. The egg of a phoenix is nearly impossible to steal, as it hatches before the area round it is cool enough for most creatures to survive.


Phoenix are intelligent, and are capable of being reasoned with, or even tricked. The tears of a phoenix can cure any ailment, be it poison, disease, or even death, but the tears only work for the specific ailment and person for which the phoenix weeps, and only when applied directly from the eyes of the phoenix. If the tears touch anything else, they lose their purity, and no longer work.

### Available creature traits
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Elemental (fire) – automatic

Wings – scalable – automatic

Feathers – automatic

Beak – automatic

Claws – automatic


## Pixie

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

## Satyr

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

## Sandman

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

## Siren

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

## Skin Walker

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

## Succubus

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

## Tree Folk

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

## Troll

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

## Wendigo

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

## Werewolf

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

## Will O’ Wisp

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

## Wyvern

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

## Zombie

### Description:
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.


Angels – positive elementals. These beings are always intelligent, and seen as having feathered wings. Their actual appearance varies, depending on the spell elements that they have access to. For example, a very weak positive elemental that had access only to the positive element might be seen as a softly glowing young child with large feathered wings. A strong positive elemental that had access to the fire element as well as the positive element could be seen as a middle aged man, with fire for hair, feathered wings, and a large flaming sword. The more powerful that a positive elemental is, the more imposing they appear, and the more spell elements they have access to.

Demons – negative elementals. These beings are always intelligent, and seen as having bat wings. Their actual appearance varies, depending on the spell elements that they have access to. For example, a very weak negative elemental that had access only to the negative element might be seen as a twisted figure, with legs of a goat and large bat-like wings. A strong negative elemental that had access to the fire element as well as the negative element could be seen as a large scaled creature with a flaming mane, large bat-like wings, and a large flaming whip. The more powerful that a negative elemental is, the more imposing they appear, and the more spell elements they have access to.

Basilisk – a large snake-like lizard. These reptiles have a “crown” of spines around the crest of their head. [killing glare, poisonous breath]

Centaur – Has the torso of a human, and the body of a horse.

Chimera – A lion possessing the head of a goat and a tail of a snake. [fire breathing]

Cockatrice – a large chicken-like creature, with the body of a small dragon. [petrification gaze/ touch/breath, power still active after death]

Succubus – supernatural being that can look like an attractive female of any species. They seduce men, and in the act of reproduction, drain vitality from their victims.

Incubus – supernatural being that can look like an attractive male of any species. They seduce women, and in the act of reproduction, drain vitality from their victims.

Goblin – Small mischievous creatures. Goblins can be from a few inches tall to 5’ tall, with varying colors of green skin. Goblins are a minor type of Faerie creature with no innate magical abilities.


Elves –

Dwarves -

Halflings

Humans

Gnomes

Satyr

Animen

Trolls

Goblins

Harpy (Harpies) – Essentially large bird-like creatures with the heads and torsos of beautiful women. Capable of speech, lure men to reproduce, they always give birth to female Harpies. While capable of true flight, Harpies only hover in combat, and can attack with their claws. Harpies are capable of spell-casting as well.

Zombies (Magical/Disease/Curse) – Cursed zombies (Voodoo) don’t infect others, they have had their souls removed. They are mostly still intelligent, but unable to assert control over their own actions as they are under the control of the one who cursed them. Magical/Disease zombies move slowly and work solely on instinct. The Disease zombies natural attacks infect their opponents so that unless cured, upon death they are re-animated as the same type of zombie that infected them.

# Creature Traits

The various creature traits available in Boundless are listed below. As always, if it’s not on the list, ask your Keeper to work with you to implement it.

## Creature trait list

The table below lists all traits available in Boundless. Items listed as vestigial may be taken as a useless version of the trait, such as vestigial wings.

Traits may be beneficial or detrimental to general campaigns, aquatic campaigns, or both. Traits listed as beneficial cost Exp. to purchase. Traits listed as detrimental “give” extra Exp. for Specialist creation. All such points must be spent on creation, and may not be banked toward future abilities.

Scalable items may be improved upon with further expenditure of Exp.

| Trait | Prerequisite | Vestigial | Beneficial | Detrimental | Scalable |
| --- | --- | --- | --- | --- | --- |
| Amphibious gills | Gills/water breathing | No | Both | No | No |
| Beak | None | No | No | General | No |
| Claws | None | No | General | No | No |
| Cycloptic | None | No | No | Both | No |
| Deaf | None | No | No | Both | No |
| Elemental1 | None | No | Both | No | Yes |
| Emotionless | None | No | No | Both | No |
| Exoskeleton | None | Yes | Both | No | Yes |
| Extra arms | None | Yes | Both | No | Yes |
| Extra legs | None | No | Both | No | No |
| Fangs | None | No | Both | No | No |
| Feathers2 | None | Yes | General | Aquatic | Yes |
| Fins | None | Yes | Aquatic | No | No |
| Ghastly | None | No | No | Both | Yes |
| Gills/Water breathing3 | None | No | Aquatic | General | No |
| Hairless | None | No | No | No | No |
| Heavy | None | No | General | Aquatic | No |
| Hirsute | None | No | General | Aquatic | No |
| Horns | None | Yes | Both | No | Yes |
| Hover4 | Wings or Wingless flight | No | Both | No | No |
| Imposing | None | No | Both | No | Yes |
| Incorporeal5 | None | No | No | Both | No |
| Incorporeal touch | Incorporeal | No | Both | No | Yes |
| Invertebrate | None | No | Aquatic | General | No |
| Light-weight | None | No | General | Aquatic | No |
| Mindless | None | No | No | Both | No |
| Mucus | None | No | Yes | No | No |
| Multi-optic1 | None | Yes | Both | No | Yes |
| Night vision | None | No | Both | No | Yes |
| Non-tactile | None | No | Both | No | No |
| Non-tasting | None | No | No | Both | No |
| Poisonous | None | No | Both | No | Yes |
| Prehensile tail | Tail | Yes | Both | No | Yes |
| Putrid | None | No | No | Both | Yes |
| Resistance1 | None | No | Yes | No | Yes |
| Scales | None | Yes | Both | No | Yes |
| Scent | None | No | Both | No | Yes |
| Scentless | None | No | No | Both | No |
| Shapeless | Invertebrate | No | Aquatic | General | No |
| Shape-shifter | None | No | Both | No | Yes |
| Shell | None | No | Both | No | Yes |
| Sightless/blind | None | No | No | Both | No |
| Size1 | None | No | Both | No | Yes |
| Speechless | None | No | No | Both | No |
| Stat bonus | None | No | Both | No | Yes |
| Stat penalty | None | No | No | Both | Yes |
| Stout | Heavy | No | Both | No | No |
| Sunlight allergy | None | No | No | Both | No |
| Tail | None | Yes | Both | No | No |
| Telepathic | None | No | Both | No | Yes |
| Tentacles | None | Yes | Aquatic | No | Yes |
| Thick hide | Heavy | No | Both | No | Yes |
| Toothy maw | None | No | Both | No | No |
| Tusks | None | Yes | Both | No | No |
| Undead | None | No | No | Both | No |
| Unnatural hunger | None | No | No | Both | No |
| Venomous | None | No | Both | No | Yes |
| Weakness1 | None | No | No | Yes | Yes |
| Webbed fingers/toes | None | No | Aquatic | No | No |
| Wingless flight | Incorporeal | No | Both | No | Yes |
| Wings | None | Yes | General | Aquatic | Yes |
| 1 Scalable, but must be fully scaled at Specialist creation. | 1 Scalable, but must be fully scaled at Specialist creation. | 1 Scalable, but must be fully scaled at Specialist creation. | 1 Scalable, but must be fully scaled at Specialist creation. | 1 Scalable, but must be fully scaled at Specialist creation. | 1 Scalable, but must be fully scaled at Specialist creation. |
| 2 Beneficial aquatic for penguins only. | 2 Beneficial aquatic for penguins only. | 2 Beneficial aquatic for penguins only. | 2 Beneficial aquatic for penguins only. | 2 Beneficial aquatic for penguins only. | 2 Beneficial aquatic for penguins only. |
| 3 Gills/water breathing is considered beneficial on land if paired with amphibious gills. | 3 Gills/water breathing is considered beneficial on land if paired with amphibious gills. | 3 Gills/water breathing is considered beneficial on land if paired with amphibious gills. | 3 Gills/water breathing is considered beneficial on land if paired with amphibious gills. | 3 Gills/water breathing is considered beneficial on land if paired with amphibious gills. | 3 Gills/water breathing is considered beneficial on land if paired with amphibious gills. |
| 4 Only incorporeal creatures may hover in aquatic environments. | 4 Only incorporeal creatures may hover in aquatic environments. | 4 Only incorporeal creatures may hover in aquatic environments. | 4 Only incorporeal creatures may hover in aquatic environments. | 4 Only incorporeal creatures may hover in aquatic environments. | 4 Only incorporeal creatures may hover in aquatic environments. |
| 5 Incorporeal is considered beneficial if paired with incorporeal touch. | 5 Incorporeal is considered beneficial if paired with incorporeal touch. | 5 Incorporeal is considered beneficial if paired with incorporeal touch. | 5 Incorporeal is considered beneficial if paired with incorporeal touch. | 5 Incorporeal is considered beneficial if paired with incorporeal touch. | 5 Incorporeal is considered beneficial if paired with incorporeal touch. |


## Creature trait descriptions

Listed below are descriptions and information about using the various creature traits in Boundless.

### Amphibious gills
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Amphibious gills allow a creature to breathe equally as well in air or water. Amphibious gills work for either salt water or fresh water. If your keeper allows it, you may take this trait twice; once for salt water, and once for fresh water.

### Beak
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

A beak takes the place of lips and nose on the face of some creatures. Beaks make it difficult to talk in many cases, and as such, are a detriment. Beaks may be used to peck instead of a bite.

### Claws
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Claws are sharp, hard protein growths at the end of fingers and/or toes. Specialists with claws may train in their use like any other weapon, either as slashing or piercing.

### Cycloptic
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Cycloptic creatures are those with but a single eye.

### Deaf
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Deaf creatures are those that lack the ability to hear, or have suffered extensive hearing damage (such as from listening to their music too loud).

### Elemental
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Elemental creatures are those comprised partly or entirely of elemental substance and/or energy, such as fire or water.

### Emotionless
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Emotionless creatures are unable to feel any sort of sympathy or remorse. Creatures that are sentient and emotionless find it impossible to connect with other creatures on any level.

### Exoskeleton
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Exoskeletons are hard dermal plates that encompass a creature and keep its shape, instead of internal bones found in mammals. Exoskeletons may be scaled to provide increased damage reduction, but are always treated as plate mail. Specialists may take armor training ranks for their exoskeleton. Without armor training, Specialists take the normal untrained armor penalty.

### Extra arms
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Extra arms are exactly that… Additional appendages, typically in pairs, and each having hands at the end. Extra arms may be vestigial, or may be scaled up to match the Toughness and Proficiency scores of the primary arms.

Vestigial arms have a Toughness and Proficiency scores of 0. Each additional rank increases the maximum Toughness and Proficiency score of a set of extra arms by 10. Multiple sets of extra arms are tracked separately, each having their own individual ranks.

### Extra legs
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Extra legs are exactly that… Additional appendages, typically in pairs, on which a creature may walk. Unlike extra arms, extra legs are considered natural, and are all used for ambulation. Creatures with extra legs find it difficult or impossible to walk on only two of them.

### Fangs
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Fangs are elongated, sharp canine teeth. Creatures with canines excel at biting and draining blood or tearing flesh of other creatures. Specialists may train with fangs as piercing and/or slashing weapons.

### Feathers
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Feathers are found on aviary creatures instead of fur or hair. Typically, they’re light-weight and hollow. Creatures with feather may go through a molting phase from time to time.

### Fins
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Fins may be vestigial, or they may replace arms/legs/hands/feet. Vestigial fins have no effect on land creatures, but those that replace appendages make movement difficult. In aquatic environments, fins aid in propulsion and guidance.

### Ghastly
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Ghastly creatures are very ugly or frightening. Weak-willed creatures may panic and/or run away when met with a ghastly visage.

### Gills/Water breathing
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Gills and water breathing allow creatures to extract their air from aquatic environments in order to breathe. Creatures with gills are unable to breathe in open air environments, unless they are amphibious.

### Hairless
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Hairless creatures are those that have little or no bodily hair. Generally hairless creatures come from hot environments. Hairless creatures often have thick hides, helping to protect them from the environment.

### Heavy
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Heavy creatures are those that have dense skin, muscle and/or bones. Heavy creatures are more difficult to knock over, but excel at knocking over other creatures. Heavy creatures get a bonus of 10 to all rolls involving Wrestling and Tripping Attack, as well as defensive actions versus Tripping Shot/Throw attacks.

### Hirsute
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Hirsute creatures are covered in hair or fur. Many hirsute creatures can withstand temperatures others would consider extreme by virtue of their natural coat. Keepers may require Specialists to choose cold or hot weather as their natural environment. Hirsute creatures get a bonus of 10 on rolls to protect against temperature conditions of their native environment.

### Horns
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Horns are calcium or protein growths which protrude from under the skin of creatures. Horns may be single, such as a rhinoceros, or come in pairs, like those of a ram. Specialists with horns may train in them as blunt or piercing weapons.

### Hover
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Hovering is the ability of a flying creature to stay aloft without forward momentum.

### Imposing
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Imposing creatures are those of great stature or repute, which can strike fear into the hearts of onlookers. Imposing creatures get a bonus of 10 per rank to opposed Charisma rolls (but not the Charisma score or charisma based skill checks).

### Incorporeal
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Incorporeal creatures are those that lack physical form. Incorporeal creatures are able to pass through solid objects as easily as corporeal creatures pass through air. For incorporeal creatures, movement in any direction is equally easy, as they don’t rest on solid surfaces. Incorporeal creatures are blocked by magical barriers, and can be harmed by magical energies.

### Incorporeal touch
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Incorporeal touch allows incorporeal creatures to summon up their will and interact briefly with the physical world. Interacting with the physical world is strenuous for incorporeal creatures, and drains their Magic pool. Each rank of Incorporeal touch decreases the magic point cost for each second of interaction with the physical world. At 1st rank, Incorporeal touch costs 45 magic points per second to use, 35 points per second at 2nd rank, 25 at 3rd, 20 at 4th, 15 at 5th, 10 at 6th, 8 at 7th, 6 at 8th, 4 at 9th, and a minimum of 2 points per second at 10th rank. (The costs are the equivalent of working backwards from high advanced to middle simple in point costs.)

### Invertebrate
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Invertebrate creatures are those that have no spines (and generally no bones to speak of). Examples of invertebrate creatures are octopi, jellyfish, and clams.

### Light-weight
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Light-weight creatures are those with less dense tissues and bones. Generally, they’re more buoyant than other creatures. Some are able to jump higher, walk across snow without sinking into it, and float on water with ease, walk across rice paper without tearing it, and many other great feats. Many aviary creatures are also light-weight, helping them to stay airborne with ease.

### Mindless
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Mindless creatures are those that lack the ability to think and reason. Even animals often have the ability to think and reason to some extent. Automata and other animated creatures, such as zombies, are mindless. Mindless creatures lack the ability to flee from threats, and generally fight until they are destroyed.

### Mucus
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Mucus producing creatures generate mucus either constantly or at-will. Mucus may be adhesive causing creatures and/or objects to stick firmly to it as in the case of a Kelpie or slick causing things to be difficult to grasp when coated.

### Multi-optic
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Multi-optic creatures are those that have multiple sets of eyes, generally in pairs. Multi-optic Specialists get a bonus of 10 on all Search and Spot checks for each pair of eyes beyond the first.

### Night vision
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Night vision allows creatures to see in conditions of poor illumination. At 60,000 lux and below, creatures without night vision begin to have difficulty seeing. Each rank of night vision decreases the minimum lux a creature needs to see normally by 5,000 (55,000 lux at 1st rank, 50,000 at 2nd rank, and so on.)

### Non-tactile
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Non-tactile creatures are unable to feel physical stimuli such as hot, cold, pressure and pain. Non-tactile creatures are in constant danger, and generally learn quickly to recognize signs of danger by means other than nerve endings.

### Non-tasting
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Non-tasting creatures lack the ability to taste. While this may be helpful in certain rare cases, it is generally dangerous, as non-tasting creatures can’t discern when something they’re eating has rotted, or is poisonous.

### Poisonous
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Poisonous creatures are toxic for other creatures to eat. Such creatures either have toxic flesh, or secrete a layer of toxic mucous on their skin.

The ranks of poisonous determine how many symptoms the toxin will have. For example, if a Specialist has 13 ranks, the Specialist could choose 1 symptom from the 10-21 rank section and 1 from the 1-3 rank section, or any combination of lower rank symptoms less than or equal to 13. The symptoms chosen may change when a new rank is purchased, but once purchased, the symptoms remain the same until the next increase in rank.

Symptom progression for higher potency of poison should be logical, unless otherwise approved by your Keeper.

| 1-3 Ranks | Confusion, unconsciousness, pain, mild allergic reaction, nausea, diarrhea |
| --- | --- |
| 4-9 Ranks | Disabled, immobilized, slowed, deafened, weakened, stiffness, moderate allergic reaction |
| 10-21 Ranks | Blindness, paralysis, seizure, ataxia, suffocation, hemorrhaging, severe allergic reaction, sleep |
| 22+ Ranks | Berserk, petrified, anaphylaxis, death |

### Prehensile tail
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Prehensile tails are tails with the ability to grab, hold, lift, and otherwise assist their owner in various tasks, almost like an additional arm.

Vestigial prehensile tails have a Toughness and Proficiency scores of 0. Each additional rank increases the maximum Toughness score by 10 and the maximum Proficiency score by 5. The tail’s maximum Proficiency score may never exceed ½ of the owner’s Proficiency score.

### Putrid
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Putrid creatures are those that emit foul odors constantly. Putrid creatures can range in foulness from mild to debilitating. Putrid creatures may be aware of their odor, but aren’t affected by it.

Putrid creatures may attempt to sicken others with their putrescence. At first rank, the odor gives a bonus of 10 to sicken creatures within 1 movement unit who fail an opposing Endurance roll. Each rank increases the range of the odor by 1 movement unit, appropriately sized for the putrid creature, or increases the bonus to the creature’s opposed Endurance roll to sicken others by 10.

### Resistance
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Resistance causes creatures to take less damage from the specified source. Each rank of resistance adds 10% to a creature’s resistance. Creatures with 100% resistance to a damage type are immune to that damage type. Resistances often come with equal, but opposite weakness counterparts.

### Scales
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Scales are small, hard, overlapping plates that grow out of a creature’s skin. scales may be scaled to provide increased damage reduction, but are always treated as scale mail. Specialists may take armor training ranks for their scales. Without armor training, Specialists take the normal untrained armor penalty.

### Scent
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Scent, also known as hyperosmia, is an acute sense of smell. Creatures with the scent ability can detect even subtle changes in odor. Creatures with the Scent ability get a penalty of 10 per rank on opposed Endurance rolls versus putrid creatures. Other than that, creatures with scent may be able to track other creatures, or even be able to use their nose in place of their eyes if they become blinded.

### Scentless
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Scentless creatures are unable to smell anything. They are immune to the odor of putrid creatures and all other smells.

### Shapeless
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Shapeless creatures lack a single, specific physical shape. A shapeless creature can squeeze through any opening larger than any solid body parts or gear they may have (for example, an octopus’s beak).

### Shape-shifter
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

A shape-shifter is a creature that has the ability to change its appearance. Each rank of shape-shifter grants a creature an additional shape into which it may shift, or the ability to shift into an additional size larger or smaller than itself.

### Shell
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

A shell consists of one solid plate, or several interlocked plates which cover a large portion of a creature’s body. Shells may be scaled to provide increased damage reduction, but are always treated as plate mail. Specialists may take armor training ranks for their shell. Without armor training, Specialists take the normal untrained armor penalty.

### Sightless/blind
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Sightless or blind creatures are those that lack, or have suffered severe damage to their optic organs. Sightless and blind creatures are unaffected by all visual stimuli, and are immune to light and darkness. Though such traits may seem beneficial, living without sight is still quite difficult. Sightless and blind creatures are forced to interact with the world vie their other senses.

### Size
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Some creatures are larger or smaller than average humanoids. Being larger or smaller has its advantages. Smaller creatures are harder to see, and harder to hit with attacks, while larger creatures are often very strong and imposing.

### Speechless
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Speechless creatures are those that lack the ability to form words. Some speechless creatures are able to communicate in other ways, and may still make noises.

### Stat bonus
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

A stat bonus is a racial bonus typically enjoyed by members of many species, such as toughness for many large creatures, and speed for many small creatures. Stat bonuses increase the maximum possible starting stat of a creature by 5. Each stat bonus also grants an additional 5 points to spend on starting stats.

### Stat penalty
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

A stat penalty is a racial penalty generally suffered by members of many species, such as speed for many large creatures, and toughness for many small creatures. Stat penalties decrease the maximum possible starting stat of a creature by 5, to a minimum of 5. Each stat penalty also reduces the initial stat points to spend by 5.

### Stout
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Stout creatures are those with dense musculature, capable of withstanding fatigue. While Stout creatures don’t actually get a bonus to their Strength, the gear they wear counts as though it were 10 lbs. lighter than it actually is (minimum of 0).

### Sunlight allergy
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Creatures with sunlight allergies have various reactions from exposure to sunlight, ranging from temporary blindness, to combustion, to petrification. Most sunlight allergic creatures avoid the sun at all costs.

### Tail
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Tails are long protrusions, extending past the base of the spine. Tails may be vestigial, normal, or prehensile.

### Telepathic
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Telepathic creatures are able to communicate with other creatures mentally. The first rank of telepathy allows the telepathic creature to send (but not receive) messages within 10 movement units, appropriately sized for the telepathic creature. Additional ranks may add the ability to receive return messages, or increase the range by 10 movement units.

### Tentacles
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Tentacles are long, slender appendages, generally equipped with suction cups. Tentacles have the ability to grab, hold, lift, and otherwise assist their owner in various tasks, almost like an arm. Tentacles usually replace arms and/or legs.

At rank 1, then tentacles have a Toughness score of 10 and Proficiency score of 5. Each rank increases the maximum Toughness score by 10 and the maximum Proficiency score by 5. A tentacle’s maximum Proficiency score may never exceed ½ of the owner’s Proficiency score.

### Thick hide
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Thick hides are exceptionally thick skin, which is tough to pierce. Thick hide reduces all physical damage taken by 1 point for each rank.

### Toothy maw
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Toothy maw is a large mouth filled with many teeth. Usually the teeth are long and sharp, or jagged. Specialists may train with toothy maw as piercing or slashing weapons.

### Tusks
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Tusks are bone-like protrusions from a creature’s mouth. Specialists may train with tusks as a piercing attack.

### Undead
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Undead is the state of being animated, though not living. Most undead are easy to spot, as they often show signs of decay, lack body heat, and have gray skin. Some undead lack flesh altogether. Undead are healed by negative energy, and hurt by positive energy.

### Unnatural hunger
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Unnatural hunger is the craving for sustenance that most would find appalling. Generally, the hunger is for blood of the living, flesh of fresh corpses, and other macabre things. Failure to indulge this hunger can lead to temporary insanity until the hunger is satiated.

### Venomous
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Venomous creatures have venom sacs which product toxic substances. These creatures generally either administer the toxin through a bite, via fangs, or through a spray or spitting the toxin out of their mouth. Other, more strange methods of envenomation exist, such as the horny toad’s ability to squirt the toxin out of their tear ducts.

The ranks of poisonous determine how many symptoms the toxin will have. For example, if a Specialist has 13 ranks, the Specialist could choose 1 symptom from the 10-21 rank section and 1 from the 1-3 rank section, or any combination of lower rank symptoms less than or equal to 13. The symptoms chosen may change when a new rank is purchased, but once purchased, the symptoms remain the same until the next increase in rank.

Symptom progression for higher potency of poison should be logical, unless otherwise approved by your Keeper.

| 1-3 Ranks | Confusion, unconsciousness, pain, mild allergic reaction, nausea, diarrhea |
| --- | --- |
| 4-9 Ranks | Disabled, immobilized, slowed, deafened, weakened, stiffness, moderate allergic reaction |
| 10-21 Ranks | Blindness, paralysis, seizure, ataxia, suffocation, hemorrhaging, severe allergic reaction, sleep |
| 22+ Ranks | Berserk, petrified, anaphylaxis, death |

### Weakness
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Weakness causes creatures to take increased damage from the specified source. Each rank of weakness adds 10% to a creature’s weakness. Weakness often come with equal, but opposite resistance counterparts.

### Webbed fingers/toes
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Webbed fingers and/or toes have a flap of skin connecting the digits, which help to propel creatures through water. Webbed fingers and/or toes negates a creature’s swim speed penalty, so long as the webbed digits are exposed. Covering the webbed digits, such as by wearing gloves or boots which cover the webbed digits prevents this negation.

### Wingless flight
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Wingless flight is the ability to gain altitude without the use of wings. Without the aid of a spell, only incorporeal creatures are capable of wingless flight. The first rank of wingless flight allows a creature to slow fall, as per the Slow Fall Flight energy. The second rank allows a creature to glide. The third rank allows a creature to soar at its base movement speed.

### Wings
> **Status:** ⚠️ REVIEW — recovered creature/trait material. Use as anatomy/capability evidence; current modular Trait rules and later explicit decisions take precedence over legacy race-package mechanics.

Wings are appendages designed for flight. Wings are either feathered, such as a bird, or webbed, such as a bat. Wings can take the place of arms, or can extend out of the back as additional appendages. The first rank of wings are vestigial. The second rank allows a creature to slow fall, as per the Slow Fall Flight energy. The third rank allows a creature to glide. The fourth rank allows a creature to soar at its base movement speed.

Creatures with wings must maintain forward momentum of at least one movement unit per turn to stay aloft, unless they also have the hover trait. Winged creatures must move 1 movement unit per 45 degrees while turning.

# Building Creatures

## 10. Additional CLEAN creature-layout notes

---

Fae

Seelie Court

Gnome

Leprechaun

Unseelie Court

Goblin

Boggart

# Creature Types

## Goblin

### Description

Stuff about the goblin

### Available creature traits

Goblins can purchase a crooked nose for one racial rank.

3 negative traits (crooked nose, gimpy leg, small lungs)

-100 points

-200 points

-300 points

4 positive traits (wings, glide, slow fly, fly)

100 points (wings)

200 points (glide)

300 points (slow fly)

400 points (fly)

# Creature Categories

## Undead

Here’s what all undead possess.

### Mindless undead

Here’s some about only mindless undead.

### Intelligent undead

Here’s some about only intelligent undead.

## Fae

Here’s what all fae possess

### Seelie

Here’s what only seelie court fae have

### Unseelie

Here’s what only unseelie fae have


Traits

Wings – feathered (angels, fae, harpies)

Wings – webbed (demons, bats)

Horns – single point (animals, demons)

Horns – multiple point/antlers (moose)

Sharpened nails – (feline, demon)


Creating a creature entails choosing from the available traits, and building the race. The more traits taken from any given creature category, the more likely the creature is to be considered a member of that category. For example, a human with webbed wings, single point horns, and sharpened nails would be considered demonic. If that same creature had 3 traits that were common to another creature category, such as fae, the maker of the creature could choose from fae or demonic.

## 11. Additional CLEAN creature-trait notes

---

Creature type

Draconic

Elemental

Fae

Giant

Ooze

Plant

Undead

Head

Antennae

Ears

Large/ Small

Animalistic

Elongated

None

Eyes

None

Cycloptic

Multi-faceted

Multi-optic

Ommatophore

Gills/ water breathing

Amphibious gills

Aquatic gills

Horns

Multi-point

Single point

Mouth

Beak

Bill

Chelicerae (spider)

Elongated

Fangs

Toothy maw

Venomous

None

Proboscis

Tentacles

Tongue

Long

Prehensile

Forked

None

Tusks

Nose

None

Slitted

Trunk

Prehensile trunk

Skin

Barbed

Quills

Bark

Elemental (choose one)

Crystalline

Full

Partial

Exoskeleton

Feathers

Hairless

Hirsute

Mucus

Adhesive

None

Photosynthetic

Scales

Secretion

Corrosive

Pheromones

Poison

Slime

Spores

Shell

Thick hide

Limbs

Claws

Fewer arms/ legs

No arms/ legs

Webbed fingers/ toes

Fins

Extra arms/ legs

Extra head(s)

Feet

Claws

Hooves

Talons

Pincers

Tail

Paddle tail

Prehensile tail

Spiked

Spinneret

Stinger, fixed

Barbed

Retractable

Tentacles

Pseudopod

Wings

Flight

Glide

Hover

Vestigial

Appearance

Displacement

Ghastly

Imposing

Size

Increased

Decreased

Body

Deadly allergy

Elemental (Choose one)

Sunlight

Silver

Incorporeal

Incorporeal touch

Invertebrate

Shapeless

Amorphous

Poisonous

Putrid

Scentless

Shapeshifter

Mimicry

Stat modifiers

Bonus

Penalty

Torso

Cephalopod

None

Unconventional

Gastropod

Multiple (Centaur)

Cephalothorax

Weight

Heavy

Stout

Lightweight

Wingless flight

Senses

Sight

Blind

Night vision

Sound

Deaf

Keen hearing

Taste

Non-tasting

Touch

Non-tactile

Smell

Scent

Speech

Speechless

Unnaturally loud

Mental

Emotionless

Mindless

Telepathic

Unnatural hunger


---

# Chapter 8 — Crafting, Materials, Equipment, Quality & Durability

## Reconstruction status legend

- **✅ CONFIRMED** — established by later explicit decisions and treated as current canon unless deliberately reopened.
- **🔄 SUPERSEDED** — recovered source material that has been replaced by a later decision.
- **⚠️ REVIEW / CONVERSION** — concept or content is useful, but one or more mechanics must be reconciled with the current engine.
- **⬜ NEEDS DEVELOPMENT** — incomplete or absent; substantial design work remains.
- **❗ CONTRADICTION** — two surviving sources or decisions conflict and must not be silently reconciled.
- **💡 SUGGESTION** — design suggestion from this reconstruction pass; not canon unless Mike approves it.

**Authority used in this reconstruction:** newest explicit decisions in the current reconstruction work override older text; CLEAN source files are the baseline for material not subsequently changed. Archival Markdown is treated as a searchable transcription of its CLEAN source, not as independent canon. No discrepancy has been silently fixed.

## 1. Current state

**⬜ NEEDS DEVELOPMENT / ⚠️ RECOVERABLE FOUNDATION**

Crafting was never fully completed in the modern engine. The recovered material establishes material categories, combustibility/elemental relationships, Skill dependencies, quality, durability, and various old tier concepts, but the success-counting conversion is incomplete.

Crafting should be rebuilt **after the Skill threshold system is locked**, because object creation, quality, repeated progress, and failure consequences depend on Skill resolution.

## 2. Quality

**⚠️ REVIEW / CONVERSION**

CLEAN commonly treats Quality as the highest successful numerical total produced while creating the object and then uses that number as a later target. That cannot survive unchanged after abandoning summed die faces.

**💡 Suggested design direction, not canon:** Quality should likely become either a success-count band, a tier + margin value, or a persistent rating derived from accumulated crafting successes. Do not choose among these until Skill thresholds are settled.

## 3. Durability

**⚠️ REVIEW / CONVERSION**

CLEAN gives Durability two jobs: object health/breakage and damage mitigation. Because the armor/mitigation ecosystem is still under review, these responsibilities must be separated conceptually before finalizing Durability.

A likely clean division would be object Durability = structural health, with armor mitigation handled by the armor system if mitigation survives. **This is a suggestion, not canon.**

## 4. Materials

Recovered material categories include Cloth, Wood, Hide, Metal, and Stone, with Elemental Properties and tiered material entries. These are useful source data even though the final crafting checks are incomplete.

## 5. Complete recovered Crafting and Materials chapter

---

# Crafting and Materials

While there are likely to be merchants throughout the lands, many Specialists will enjoy crafting their own gear. Some will craft items to sell, to make a living outside of adventuring. Others may craft to save on the cost of buying. Still others will craft to take advantage of the improved quality of the items they make. This section covers how various materials affect crafted items and general guidelines for obtaining and working with those materials.

# Combustibility

Many materials are combustible, and may be set on fire with prolonged exposure to heat. In game terms, this means a single blast of intense heat damage or prolonged exposure to damage from a heat source will cause those materials to ignite. For example, oil or tinder exposed to a flame readily ignites. Other materials, such as firewood take a bit more damage to ignite. Treated wood, such as the walls of a cabin are even tougher to burn. Some materials, such as stone or metal are not likely to burn regardless of how much heat damage they take.

To ignite a material or object requires continuous exposure to a source of heat until the appropriate level of heat damage has been sustained. For example, a material with a combustion point of 15 would begin to burn if it was hit with a fire spell that dealt 15 or more damage, even if the spell was instantaneous. That same material would begin to burn with continued exposure to lower amounts of heat damage, such as being dropped in a campfire for several turns. Exposing that material to repeated instantaneous fire damage of smaller amounts would not cause it to ignite. For example, hitting it twice in a row with 14 points of fire damage would not ignite the material.

# Materials

The following is a list of materials, including their general type (wood, metal, etc), properties such as elemental resistances, whether or not it is combustible, whether it is an insulator or conductor for electricity, other special notes, and finally examples of the material separated by quality degrees.

## Cloth

Cloth is a supple fabric consisting of woven strands of fiber.

Mitigation: 1d10

Elemental Immunity: None

Combustible: Yes – 15 fire damage per quality degree

Electricity: Neither insulator nor conductor

Simple: Burlap

Basic: Wool

Intermediate: Canvas

Advanced: Linen

Master: Silk

## Wood

Material generic info

### Elemental Properties

Immune: None

Combustible: Yes

Electricity: Neither insulator nor conductor

### Simple


### Basic


### Intermediate


### Advanced


### Master

## Hide

Material generic info

### Elemental Properties

Immune: None

Combustible: Yes

Electricity: Neither insulator nor conductor

### Simple


### Basic


### Intermediate


### Advanced


### Master

## Metal

Material generic info

### Elemental Properties

Immune: None

Combustible: Yes

Electricity: Neither insulator nor conductor

### Simple


### Basic


### Intermediate


### Advanced


### Master

## Stone

Material generic info

### Elemental Properties

Immune: None

Combustible: Yes

Electricity: Neither insulator nor conductor

### Simple


### Basic


### Intermediate


### Advanced


### Master

## 6. Recovered Quality and Durability rules from General Rules

---

# Quality and Durability

## Quality

When an item is created, its Quality is equal to the highest success its creator rolls during the creation process. This number represents the maximum amount of damage the item can take before breaking. In essence, it is roughly equivalent to a living creature's Endurance score. Damaged items may only be repaired up to a maximum durability equal to the item's quality.


## Durability

An item's Durability score serves two purposes. First, it represents the inherent damage mitigation an item has. When the item is attacked, the damage is mitigated by its durability if unattended. Other modifiers to mitigation may apply if the item is held or worn. Second, it represents the remaining amount of damage the item can take before being broken. An item with 0 remaining durability is broken and must be repaired before it can be used properly again. When an unattended item takes damage, it should be noted by the Keeper. When an item owned by a Specialist takes damage, it should be noted on the Specialist Record. For example, if an item with a quality of 45 takes 5 points of damage, the item's Durability score would be shown as 40/45, representing remaining Durability/Quality. In this example, if the item were to be attacked again, it would have 40 points of mitigation instead of the original 45.

## 7. Equipment/armor dependency

**⚠️ IMPORTANT:** do not finalize armor material ratings, item mitigation, shield mitigation, Penetration, or durability-based protection until the Combat/Armor review determines whether and how mitigation survives.


---

# Chapter 9 — World, Social, Travel & Miscellaneous Rules

## Reconstruction status legend

- **✅ CONFIRMED** — established by later explicit decisions and treated as current canon unless deliberately reopened.
- **🔄 SUPERSEDED** — recovered source material that has been replaced by a later decision.
- **⚠️ REVIEW / CONVERSION** — concept or content is useful, but one or more mechanics must be reconciled with the current engine.
- **⬜ NEEDS DEVELOPMENT** — incomplete or absent; substantial design work remains.
- **❗ CONTRADICTION** — two surviving sources or decisions conflict and must not be silently reconciled.
- **💡 SUGGESTION** — design suggestion from this reconstruction pass; not canon unless Mike approves it.

**Authority used in this reconstruction:** newest explicit decisions in the current reconstruction work override older text; CLEAN source files are the baseline for material not subsequently changed. Archival Markdown is treated as a searchable transcription of its CLEAN source, not as independent canon. No discrepancy has been silently fixed.

## 1. Reputation and Disposition

**⚠️ REVIEW, low dependency**

CLEAN provides a -100 to +100 Reputation/Disposition framework with named bands. It has not been explicitly superseded, but it also has not been recently re-confirmed.

# Reputation and Disposition

## Reputation

In general, Specialists will lean toward being heroic or villainous. Performing heroic or villainous acts will affect how the population at large tends to view them by default. A Specialist’s reputation is a number between -100 and 100. This number typically starts at 0, and is increased by performing positive, helpful, heroic actions or decreased by performing negative, harmful, villainous actions. The Keeper will let you know when you need to adjust this number.

A Specialist’s reputation influences NPCs’ dispositions toward them. Specialists with positive reputations are generally looked on more favorably by NPCs who tend toward the positive end of the spectrum such as town guards, and less favorably by those who tend toward the negative end of the spectrum such as criminals. Conversely, Specialists with negative reputations are generally looked on more favorably by the criminals, and less favorably by the guards.

Another effect of having an exceptionally high or exceptionally low reputation is notoriety. Generally, the further you are from 0 toward the positive, the more people know of your heroic deeds, while the further you are from 0 toward the negative, the more people will know of your villainy. Larger positive or negative numbers increase the chance that people in smaller, and more wide-spread and smaller communities will be aware of your reputation, and will be disposed toward you accordingly.

## Disposition

### 100 (Zealot)

A creature with a disposition of 100 toward a Specialist worships the ground the Specialist walks on. This creature will do anything and everything in their power, including self-sacrifice, to make the Specialist happy.

### 75 to 99 (Fanatic)

A creature with a disposition of 75 or greater trusts a Specialist implicitly. They’ll do nearly anything within their power to make the Specialist happy, but draws the line at self-harm or self-sacrifice. They may attempt to defend the Specialist from attacks, but not against overwhelming odds of when doing so will obviously be suicidal.

### 50 to 74 (Good Friend)

A creature with 50 to 74 disposition toward a Specialist regards them as a good friend. In general, they trust the Specialist, but may question their motives if asked to do something that could result in the creature being harmed. The creature may fight alongside the Specialist, but won’t go out of their way to defend the Specialist over themselves.

### 25 to 49 (Friend)

A creature with 25 to 49 disposition toward a Specialist regards them as a friend, but is not inherently inclined to trust them, and questions their motives more often than not. This creature won’t attack the Specialist unless the Specialist attacks them first. A combatant whose disposition is raised above 25 will cease attacking a foe unless the foe does something to make themselves threatening, such as attacking.

### -24 to 24 (Indifferent)

A creature with -24 to 24 disposition is essentially indifferent toward the Specialist. If the Specialist exhibits hostility toward the creature or any other creatures affiliated with the creature, they won’t hesitate to attack. Short of open hostility, though, the creature won’t go out of their way to interact with the Specialist.

### -49 to -25 (Unfriendly)

A creature with -49 to -25 disposition is distrusting toward a Specialist, but will scrutinize any actions that could potentially be considered threatening. If the creature feels threatened, they won’t hesitate to attack.

### -74 to -50 (Hostile)

A creature with -74 to -50 disposition is hostile toward the Specialist and will actively look for reasons to attack them. They will observe laws, but will otherwise attack on sight.

### -99 to -75 (Enemy)

A creature with -99 to -75 disposition is violently hostile, and will attack the Specialist on sight regardless of laws.

### -100 (Nemesis)

A creature with -100 disposition toward a Specialist views them as the bane of their existence. This creature seeks to actively track and destroy everything the Specialist holds dear, and ultimately obliterate them and theirs.

## 2. Movement, travel, and alternative movement

**⚠️ MIXED STATUS**

Modern combat distance separates Speed from Movement Speed and uses Size-based MU. CLEAN travel rules remain useful evidence for terrain, long-distance movement, creature-powered travel, and alternate movement methods, but any formula that uses old Speed directly must be converted.

# Movement

Movement is the basis of adventuring. Without movement, Specialists wouldn’t be Specialists… They’d be statues. As such, we’ve provided some guidelines on how to handle movement.

## General Movement

In Boundless, there are two types of movement: combat movement, and travel movement. Combat movement is covered in the combat section. Travel movement covers any form of overland, or over water movement, whether it’s walking, swimming, flying, riding, driving a vehicle, rowing a boat, or sailing a ship. While combat movement is more precise, and measured in movement units, travel movement is less precise, and measured in relative travel time. For example, if an average person takes 5 days to get from one village to another village, the distance would be “five days”. Specialists generally travel from an hour after dawn until an hour before dusk. Nocturnal Specialists, on the other hand, generally travel from an hour after dusk until an hour before dawn.

Adventurers often travel longer hours than the average person, and sometimes even do “forced march”. While this cuts down on the travel time, it also takes a toll on the adventurers, as they forego rest to arrive sooner.

## Relative Movement

Movement is based on the standard form of movement for a particular area. For example, the standard movement on a road is the movement of a wagon. The standard movement through a forest or plain is walking. The standard movement on water is sailing. The standard movement through the air is flying. Use the following chart to determine approximate travel time changes. Riding in the air is a special circumstance, where a rider is on a flying mount.

Each form of movement that depends on the physical prowess of a creature, such as walking, flying or rowing, etc. are all capable of moving at double and quadruple speeds. Increased movement speeds use Fatigue points over time. Creature powered movement can also be slower than normal with no penalty or fatigue point cost.

| Terrain | Standard | Walking | Flying | Riding | Driving | Rowing | Swimming | Sailing | Burrowing |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Land | Walking | N/A | N/P | x2 | x2 | N/P | N/P | N/P | N/P |
| Air | Flying | N/P | N/A | x2 | N/P | N/P | N/P | N/P | N/P |
| Land | Riding | x1/2 | N/P | N/A | Same | N/P | N/P | N/P | N/P |
| Road | Driving | x1/2 | N/P | Same | N/A | N/P | N/P | N/P | N/P |
| Water | Rowing | N/P | N/P | N/P | N/P | N/A | x1/2 | x2 | N/P |
| Water | Swimming | N/P | N/P | N/P | N/P | x2 | N/A | x4 | N/P |
| Water | Sailing | N/P | N/P | N/P | N/P | x1/2 | x1/4 | N/A | N/P |
| Underground | Burrowing | N/P | N/P | N/P | N/P | N/P | N/P | N/P | N/A |
| N/A indicates that a change is not applicable, as it is referring to its own movement type. N/P indicates that a particular form of movement is not possible for that terrain. | N/A indicates that a change is not applicable, as it is referring to its own movement type. N/P indicates that a particular form of movement is not possible for that terrain. | N/A indicates that a change is not applicable, as it is referring to its own movement type. N/P indicates that a particular form of movement is not possible for that terrain. | N/A indicates that a change is not applicable, as it is referring to its own movement type. N/P indicates that a particular form of movement is not possible for that terrain. | N/A indicates that a change is not applicable, as it is referring to its own movement type. N/P indicates that a particular form of movement is not possible for that terrain. | N/A indicates that a change is not applicable, as it is referring to its own movement type. N/P indicates that a particular form of movement is not possible for that terrain. | N/A indicates that a change is not applicable, as it is referring to its own movement type. N/P indicates that a particular form of movement is not possible for that terrain. | N/A indicates that a change is not applicable, as it is referring to its own movement type. N/P indicates that a particular form of movement is not possible for that terrain. | N/A indicates that a change is not applicable, as it is referring to its own movement type. N/P indicates that a particular form of movement is not possible for that terrain. | N/A indicates that a change is not applicable, as it is referring to its own movement type. N/P indicates that a particular form of movement is not possible for that terrain. |

As illustrated by the chart, some movement forms are not generally applicable, though there are some exceptions. For example, if a lake is frozen, swimming, rowing and sailing would no longer be possible, but walking, riding, driving, and even burrowing would become possible. Special conditions such as this should be handled by the keeper.

## Alternative Methods of Movement

When using a movement type that you are not native to (swimming or flying for a human, for example) your fatigue drains twice as quickly when moving at full speed. When using alternative movement methods at half your normal movement speed, your fatigue drains at the normal rate.

## 3. Carrying, lifting, pushing, pulling

**⚠️ REVIEW**

The CLEAN physical-exertion formulas are sufficiently concrete to preserve as the starting point:

- Normal carry ≤ Toughness kg.
- Heavy carry ≤ 2× Toughness kg; duration Stamina minutes; 1/2 speed.
- Overloaded carry ≤ 3× Toughness kg; duration Stamina minutes; 1/4 speed.
- Dead lift ≤ 10× Toughness kg; cannot move; duration Stamina seconds.
- Normal push/pull ≤ 10× Toughness; 1/2 speed; Stamina minutes.
- Heavy push/pull ≤ 20× Toughness; 1/4 speed; Stamina minutes.
- Overloaded push/pull ≤ 30× Toughness; 1/8 speed; Stamina seconds.

The exact Fatigue penalties, movement conversion to the modern MU system, and questionable/typo wording must be adjudicated rather than silently repaired.

# Weight Limitations

Throughout their adventures, Specialists will find various treasures of all shapes, sizes and weights. Since Specialists generally are not superhuman, or godly, they have restrictions to the amount of weight they’re able to carry. Moving objects, whether heavy or light, takes some amount of exertion.

If a Specialist exceeds their normal weight limit, with whatever method (dead lift, push/pull, carrying), they may do so for only a short amount of time. Following this section is a chart with some examples of each weight limit, movement speed and the length of time a Specialist may maintain such a level of overexertion.

All values given are subject to change based on circumstances. Values given assume smooth transport and minimal friction, such as pushing or pulling a cart, or a smooth marble object across a smooth marble surface. Pushing or pulling an object through difficult terrain, such as gravel or sand, or up a hill requires more effort. Keepers may increase fatigue damage or effective weight of objects to compensate for increased difficulty.

## Carrying

### Normal

A Specialist may carry any amount below or equal to their normal weight limit without any penalty. Normal weight limit for a Specialist is a number of kilograms (kg) equal to their Toughness score. For example, a Specialist with a Toughness score of 10 may carry up to 10kg without penalty. Specialists exceeding their normal speed take 5 points of fatigue damage, and an additional 5 cumulative points of fatigue damage per minute.

### Heavy

The Specialist may carry up to twice their normal weight limit, as shown below, for a period of time equal to their Stamina score in minutes. Specialists carrying heavy loads may only move at ½ their normal movement speed. For example, a Specialist with a Toughness score of 10 and a Stamina score of 10 could carry more than 10kg, up to 20kg for up to 10 minutes. Specialists exceeding this time limit while carrying a heavy load take 1 Fatigue point of damage, and an additional 1 cumulative (2, 3, 4, etc.) points of fatigue damage per minute. Specialists exceeding ½ their normal speed while carrying a heavy load take 1d10 points of fatigue damage, and an additional 1d10 cumulative (2d10, 3d10, 4d10, etc.) points of fatigue damage per minute. These penalties stack.

### Overloaded

Specialists may carry up to a maximum of 3 times their normal weight limit and remain mobile. While doing so, the Specialist may only move at ¼ of their normal speed for a period of time equal to their Stamina score in minutes. For example, a Specialist with a Toughness score of 10 and a Stamina score of 10 could carry more than 20kg, up to 30kg for up to 10 minutes. Specialists exceeding this time limit while overloaded take 5 points of fatigue damage, and an additional 5 cumulative (10, 15, 20, etc.) points of fatigue damage per minute. Specialists exceeding ¼ their normal speed while overloaded take 2d10 points of fatigue damage, and an additional 2d10 cumulative (4d10, 6d10, 8d10, etc.) points of fatigue damage per minute. These penalties stack.

## Dead Lift

For a dead lift, the Specialist may only lift a number of kilograms not to exceed 10 times their Toughness score off the ground, and they may not move while doing so. The Specialist may lift this weight for a number of seconds equal to their Stamina score. Example: if a Specialist with a Toughness score of 10 is carrying 10kg in gear and items, they may only dead lift an additional 90kg for a total of 10 seconds. Specialists may not move while deadlifting, nor can they lift weights in excess of their dead lift limit. Specialists attempting to move while dead lifting, or exceed their dead lift limit immediately lose all remaining Fatigue points, rendering them unconscious. A Specialist who exceeds their time limit takes 10 points of fatigue damage, and an additional 10 cumulative (20, 30, 40, etc.) points of fatigue damage per second.

## Push or Pull

### Normal

A Specialist may push or pull up to 10 times their Toughness score at ½ their normal speed for an amount of time equal to their Stamina score. For example, a Specialist with a Toughness score of 10 and a Stamina score of 10 could push or pull up to 100kg at ½ their normal speed for up to 10 minutes. Specialists exceeding their time limit take 1 Fatigue point of damage, and an additional cumulative (2, 3, 4, etc.) point of fatigue damage per minute. Specialists exceeding ½ their normal movement speed take 1d10 points of fatigue damage, and an additional 1d10 cumulative (2d10, 3d10, 4d10, etc.) points of fatigue damage per minute. These penalties stack.

### Heavy

A Specialist may push or pull a heavy load, 20 times their Toughness score, and move at ¼ of their normal speed for a period of time equal to their Stamina score in minutes. For example, a Specialist with a Toughness score of 10 and a Stamina score of 10 could push or pull more than 100kg, up to 200kg for up to 10 minutes. Specialists exceeding their time limit while pushing or pulling a heavy load take 5 points of fatigue damage, and an additional 5 cumulative (10, 15, 20, etc.) points of fatigue damage per minute. Specialists exceeding ¼ of their normal speed take 2d10 points of fatigue damage, and an additional 2d10 cumulative (4d10, 6d10, 8d10, etc.) points of fatigue damage per minute. These penalties stack.

### Overloaded

A Specialist may push or pull a weight no more than 30 times their Toughness score, moving at 1/8 speed for a period of time equal to their Stamina score in seconds. For example, a Specialist with a Toughness score of 10 and a Stamina score of 10 may push or pull more than 200kg, up to 300kg at 1/8 their normal speed for up to 10 seconds. An overloaded Specialist exceeding their time limit while pushing or pulling takes 10 points of fatigue damage, and an additional 10 cumulative (20, 30, 40, etc.) points of fatigue damage per second. An overloaded Specialist exceeding 1/8 of their normal movement speed while pushing or pulling takes 40 points of fatigue damage, and an additional 40 cumulative (80, 120, 160, etc.) points of fatigue damage per second. These penalties stack.

## Overloaded

Specialists may not exceed overloaded weight limits without immediately losing all remaining fatigue points. At any point in time the Specialist exceeds any time or speed limits described above, they automatically start taking Fatigue point damage as shown in the chart below. Note: all values are based on a Specialist with a Toughness score of 10, and a Stamina score of 10.

| Weight Limit | Weight | Movement | Time allowed |
| --- | --- | --- | --- |
| Carry - Normal | Up to 10kg | Normal | Any |
| Dead lift - Normal | Up to 100kg | None | Stamina score in seconds |
| Push/pull - Normal | Up to 100kg | 1/2 speed | Stamina in minutes |
| Carry - Heavy | 11-20kg | 1/2 speed | Stamina in minutes |
| Push/pull - Heavy | 101 – 200kg | 1/4 speed | Stamina score in minutes |
| Carry - Overloaded | 21-30kg | 1/4 speed | Stamina score in minutes |
| Push/pull - Overloaded | 201 – 300kg | 1/8 speed | Stamina score in seconds |

## 4. Fatigue and sleep

**⚠️ REVIEW / PARTLY SUPERSEDED**

Modern Fatigue is a 1:1 derivative of Stamina and participates in the Downed/Unconscious/Death matrix. CLEAN uses older Fortitude/fatigue language and sleep-regeneration formulas. Preserve the recovery concepts, but convert terminology and numbers only after review.

# Fatigue and Sleep

The vast majority of living creatures tend to get tired, and eventually need to sleep. Specialists are no different. Adventuring eventually takes a toll, and most Specialists will find themselves in need of sleep to recuperate their various pools.

## Fatigue

Any damage to a Specialist’s Fortitude points or Fortitude pool is considered fatigue. Some examples of causes of fatigue are carrying heavy loads, lack of sleep, and spells that directly attack Fortitude points. Fatigue points can only be restored by resting.

## Sleep

A Specialist’s pools are restored while they sleep. On the other hand, a Specialist that goes without it not only doesn’t benefit from pool regeneration, but eventually begins to suffer penalties, even to the point of exhaustion.

### The effects of sleep

Sleep is the best way for a Specialist to restore their various pools. In general, the amount of sleep a Specialist gets in relation to the amount of sleep they need should determine how much their pools are regenerated. For example, if a Specialist needs 8 hours of sleep, but only gets 4 hours of sleep, their pools should regenerate by an amount roughly half of any spent or lost points. For example, if a Specialist has a maximum Vitality pool of 100 and has lost 50 Vitality points, they would gain 25 points back after 4 hours.

The amount of sleep needed should refer to a 24-hour period. Thus, if a Specialist is awoken after 4 hours by battle, and manages to get back to sleep within a reasonable time, they would still only need 4 more hours of sleep to be fully restored, even if additional points were lost during the short interruption to their sleep.

### The effects of not sleeping

Each day without a full night of sleep temporarily reduces your max fortitude pool by an additional amount of 10 x the number of days without sleep. For example: 3 days without sleep results in 60 points ((1x10)+(2x10)+(3x10) = 60) of reduction to the max amount of the Fortitude pool.

Each day without sleep increases the amount of sleep needed to get the next full night of sleep, restoring your Fortitude pool, by an additional cumulative number of hours equal to the number of days without sleep. For example: 3 days without sleep results in a Specialist needing 14 hours (8+1+2+3 = 14) of sleep.

If the decrease in the maximum Fortitude pool drops the Specialist’s maximum Fortitude pool below 1, the Specialist is exhausted and automatically passes out. The Specialist must then sleep for the entire duration needed to restore the Fortitude pool to its natural maximum. For example, if a Specialist with a natural maximum Fortitude pool of 60 goes 3 days without sleep (thus reducing their maximum Fortitude pool by 60), the Specialist would immediately pass out, and would need 14 hours of sleep before regaining consciousness. Even the threat of severe and immediate danger, including being attacked, fails to wake the Specialist.

## 5. Illness, disease, poison

**⚠️ REVIEW.** Useful world/condition framework; needs conversion to the universal success engine and unified Conditions philosophy.

# Illness, Disease and Poison

Throughout their adventures, Specialists may be exposed to various maladies through one means or another. Maladies fall under the categories of illness, disease or poison. Illnesses are generally contracted from the environment, and are short lived. Diseases are generally contracted via magic, environment, or genetics, and are typically chronic or persistent. Poison is typically contracted from the environment, bites, contact with poisonous plants, magic, or ingesting poisoned foods (usually in the case of nobles). The effects of each can range from mild to severe, or even fatal.

The following table shows symptoms which could be attributed to illness, disease or poison interchangeably.

| Low severity | Sneezing, Coughing, Fever, Sweating, Vomiting, Rash/Inflammation, Insomnia, Dizziness, Confusion, Unconsciousness, Silenced, Sleep, Pain, Allergic reaction (mild), Diarrhea |
| --- | --- |
| Medium-low severity | Fatigued, Diarrhea, Nausea, Pulmonary edema, Dementia, Skin lesions, Cysts/boils, Blurred vision, Disabled (cannot attack, still move), Immobilized (cannot move, still attack), Slowed, Deafened, Weakness, Stiffness, Allergic reaction (moderate) |
| Medium-high severity | Hypersensitivity, Ataxia, Kidney failure, Hemorrhaging, Dysentery, Pneumonia, Seizures, Hemophilia, Blindness, Paralysis, Seizure, Ataxia, Suffocation, Hemorrhaging, Allergic reaction (severe) |
| High severity | Liver failure, Heart failure, Blindness, Hypotonia, Encephalitis, Necrosis, Insanity, Systemic Infection, Coma, Berserk (fatal exposure/withdrawal), Petrify, Death, Anaphylaxis |

## 6. Addictions

**⚠️ REVIEW.** Particularly relevant because later Berserk/Meginserk are addictive drugs. CLEAN addiction rules should be the starting evidence for that subsystem.

# Addictions

Some substances are addictive. In general, we recommend avoiding substance abuse. That said, berserkers and meginserkers suffer addictions. Other addictive substances may also be used to make Specialists seem more “alive”, such as alcoholism or tobacco smoking. Some poisons may also be employed to reduce the effects of withdrawals of the same type of poison.

That said, we wish to make it clear that we don’t condone or promote substance abuse outside of the game. Alcoholism, drug abuse, and tobacco addiction are serious issues which can cause severe health problems and can be very difficult to overcome.

## 7. Religion

**⚠️ REVIEW, low mechanical dependency.** Divine and arcane power are intended to remain distinct in the broader Boundless setting.

# Religion

Boundless doesn’t promote in-game religion. There are a couple reasons for this. Primarily, we don’t want to offend anybody by creating any sort of false idols. In our experience, there are people who talk about in-game religions, and give the game a bad name to those who overhear conversations without understanding that the player is talking about the game.

That said, we do understand that some Keepers will want to have religion in their games. If that’s the case, more power to you. We suggest finding a religion that exists, whether in your real life, or in another game, and tailoring it to Boundless. When doing so, however, we strongly urge Keepers and players to be mindful of the beliefs of others, and not to be offensive to those who may follow a particular religion. For Keepers that do choose to have religion in their games, we also suggest treating it more as an organizational tool, similar to a guild, rather than a focus of worship. The hierarchy of the clergy may be important to followers of a religion, but specific religious practices, in many cases, are probably best left out of Boundless. Ultimately, though, it’s up to the Keeper and the players.

In particular, religions with a lot of “mythology” behind them and supporting them make good game religions. Think of it as a good excuse to research and learn about a religion that interests you to keep it as accurate as possible.

We also strongly urge Keepers not to fall back on religion as “Deus Ex Machina”, or “Hand of God”. This means that you should give your players the chance to shine, rather than putting them in completely helpless situations for the sole purpose of saving them with some godly figure. If your players find themselves in a completely hopeless situation, you may want to reexamine your story, and cut back on the difficulty a bit.

## 8. Advanced creatures

**⚠️ REVIEW:** pets, spirit guides, familiars, kindred beasts, and special mounts are preserved as world/system concepts. They may ultimately depend on Creature/Traits and advancement rules.

# Advanced Creatures

In many fantasy settings, there are people who have strong ties, or sometimes even magical bonds to various creatures, that allow the creatures to help their owners in various ways. Boundless is no different. Below are some of the types of creatures a Specialist may train, befriend, and form magical bonds with.

### Pets

Pets are mundane, domesticated animals that follow training, and remain loyal so long as they’re cared for, and treated fairly well. Pets must be fed on a regular basis, or allowed to hunt their own food if the animal is capable of hunting. A pet may be trained through the use of the Falconry skill in the case of flying pets, the Handle animal skill in the case of non-flying, non-beast of burden pets, or the Ride skill in the case of beasts of burden. Pets generally remain loyal, but gain no special bonuses or benefits, and don’t advance through the use of experience. Neglected or abused pets are likely to run away from their owners at the first opportunity they get.

Even mundane pets may become familiars, kindred beasts or special mounts, as appropriate, if their owner is, or becomes, the bearer of a spirit guide.

### Spirit Guides

A spirit guide is an incorporeal creature that takes the form of a specific animal. The animal is essentially a portion of its bearer’s psyche. The bearer of a spirit guide may train his or her spirit guide through the use of the appropriate skill, such as falconry for a flying spirit guide, handle animal for a non-flying, non-beast of burden spirit guide, and ride for a beast of burden spirit guide.

When the bearer of a spirit guide reaches intermediate tier training with his or her spirit guide, the bearer may choose for the guide to remain in spirit form, or send the guide to find a suitable physical host of the same animal type. In the latter case, the spirit guide then symbiotically merges with the mind of the animal, and the animal becomes a familiar, kindred beast, or special mount as appropriate.

While a spirit guide remains an incorporeal animal, it helps its bearer to access their own subconscious, and grants a static, cumulative bonus to its bearer for each tier of training ; 1 for simple, 3 for basic, 6 for intermediate, 10 for advanced, and 15 for master. These bonuses only apply to the Listen, Spot, Empathy, Falconry, Handle animal, Lip reading, Ride, Search, and Tracking skills, and only if the bearer knows the skill. In addition, the bearer may choose a single other skill they’re trained in, to which they may apply the bonus.

### Familiars

If the bearer of a spirit guide chooses for their guide to become a familiar, they lose the skill bonuses provided by the guide, and instead gain a physical version of the guide with its own abilities and traits. The bearer of the familiar may continue to train their familiar using the appropriate animal training skill.

The bearer of the familiar may train their familiar in certain skills the bearer knows, subject to Keeper approval. In such cases, the animal training skill used to train the familiar acts exactly like the Education skill, allowing the bearer to train the familiar in skills up to one tier lower than their rank in the animal training skill, or the skill the familiar is to learn (whichever is lower).

While familiars are frail, and not prone to physical combat, they have the potential to cast spells on a limited basis. The owner of a familiar may train its familiar in any spells up to the tier below their highest tier of spells, and only from structures and energies the owner already knows. At first rank of magic, the familiar may cast an instantaneous touch spell of one energy type known to the owner. Each additional rank, the owner may teach its familiar one additional energy or structure the owner knows already. Familiars needn’t meet the minimum primary casting stat score to cast a spell, but they must have enough points in their Magic pool to cast the spell.

### Kindred Beasts

If the bearer of a spirit guide chooses for their guide to become a kindred beast, they lose the skill bonuses provided by the guide, and instead gain a physical version of the guide with its own abilities and traits. The bearer of the kindred beast may continue to train their kindred beast using the appropriate animal training skill.

The bearer of the kindred beast may train their kindred beast in certain skills the bearer knows, subject to Keeper approval. In such cases, the animal training skill used to train the kindred beast acts exactly like the Teaching skill, allowing the bearer to train the kindred beast in skills up to one tier lower than their rank in the animal training skill, or the skill the kindred beast is to learn (whichever is lower).

Kindred beasts are wild, ferocious, and able to charge head first into combat. The owner of a kindred beast may train their beast in any martial attacks up to the tier below their highest tier of martial components, and only from components the owner already knows. The beast must be physically capable of using an attack to learn it. For example, a beast with opposable thumbs could be trained to use ranged attacks, such as a sling or bow, while more animalistic beasts may only learn melee attacks that apply to their bite and/or claw attacks. At each rank martial rank, a kindred beast may learn one martial component its owner knows. Kindred beasts needn’t meet the minimum primary martial stat score to learn a martial component, but they must have enough points in their Martial pool to use the attack.

### Special mounts

If the bearer of a spirit guide chooses for their guide to become a special mount, they lose the skill bonuses provided by the guide, and instead gain a physical version of the guide with its own abilities and traits. The rider of the special mount may continue to train their special mount using the Ride skill.

The rider of the special mount may train their special mount in certain skills the rider knows, subject to Keeper approval. In such cases, the Ride skill acts exactly like the Teaching skill, allowing the rider to train the special mount in skills up to one tier lower than their rank in the Ride skill, or the skill the special mount is to learn (whichever is lower).

Special mounts are beasts of burden with a strong connection to their rider. In most ways, a special mount works like a kindred beast, with a few exceptions, as listed below:

Special mounts may never learn ranged attacks.

Special mounts may act on their rider’s action when the rider is mounted.

Special mounts have access to special maneuvers to assist their rider in and out of combat.

## 9. Ammunition recovery

**⚠️ REVIEW:** appears in both General Rules and Combat. Retain until weapon/equipment pass determines the final ammunition model.

# Ammunition Recovery

For Specialists that use projectile weapons, ammunition has the potential to be fairly expensive. There is also a possibility that ammunition that hasn’t been used may be recovered. Certain circumstances may make a particular arrow, bolt, rock, etc. unable to be recovered, such as a troll fleeing with an arrow sticking out of his shoulder. In general, though, about 10% of used ammunition should be able to be recovered by the owner (or left to be recovered by scavengers, if the owner doesn’t take the time to recover it).

## 10. Improvisation cross-reference

Improvisation is catalogued in the Core chapter because it crosses Items, Magic, Martial, and Skills. It should remain available here as a world-facing principle once exact modifiers are modernized.


---

# Chapter 10 — Open Questions, Contradictions & Work Queue

## Reconstruction status legend

- **✅ CONFIRMED** — established by later explicit decisions and treated as current canon unless deliberately reopened.
- **🔄 SUPERSEDED** — recovered source material that has been replaced by a later decision.
- **⚠️ REVIEW / CONVERSION** — concept or content is useful, but one or more mechanics must be reconciled with the current engine.
- **⬜ NEEDS DEVELOPMENT** — incomplete or absent; substantial design work remains.
- **❗ CONTRADICTION** — two surviving sources or decisions conflict and must not be silently reconciled.
- **💡 SUGGESTION** — design suggestion from this reconstruction pass; not canon unless Mike approves it.

**Authority used in this reconstruction:** newest explicit decisions in the current reconstruction work override older text; CLEAN source files are the baseline for material not subsequently changed. Archival Markdown is treated as a searchable transcription of its CLEAN source, not as independent canon. No discrepancy has been silently fixed.

This file is deliberately blunt. These are the places where the reconstruction cannot honestly claim a final rule yet.

## A. RED — blocks multiple other systems

### A1. Skill core resolution

**✅ RESOLVED:** Skill thresholds are **2 / 3 / 4 / 5 / 6 successes** for Simple through Master. Skill difficulty is independent of Training degree. Anyone may attempt a Skill; mathematical capability emerges from the dice available rather than from permission gates.

**✅ RESOLVED:** generic favorable/unfavorable circumstance modifiers are removed. Hasty and Meticulous are the universal pace-based Skill modifiers. Concrete advantages/disadvantages come from actual rules sources such as tools, Traits, Magic, Conditions, assistance, environment, or Skill-specific text.

**Remaining Skill work:** individual Skill timing/examples and entry-by-entry cleanup. Teamwork and Skills in combat are resolved.

### A2. Character creation economy

**❗ Conflict:** CLEAN = 100 Stat points + initial Advancement/10 points. Later Trait architecture = 100 creation points shared by Stats and Traits, with negative Traits returning points.

**Decision required:** one unified creation budget and starting maximums.

### A3. Armor / mitigation ecosystem

**⚠️ Do not delete mitigation yet.** Review armor dice, armor categories, Armor Training, shield dice, shield Training, natural armor, mitigation, shield mitigation, Penetration, Armor Conditioning, Favored Shield, Rhino Hide, Pack Attack, Quality/Durability, and magic Protection together.

### A4. Martial Component conversion

Many Components are conceptually strong but mathematically written for a different engine. Convert static numbers (e.g. 40 reduced by 5), old caps, mitigation reductions, negative AP counters, old Evasion/Armor sequencing, and AP-as-scaling formulas into success-counting mechanics.

## B. ORANGE — significant but bounded

### B1. Defense path equipment details

The paths themselves are confirmed: Agility/Unarmored, Insight/Evasion, Stamina/Armor, mutually exclusive per roll. Still define armor categories and all edge cases (light armor + Evasion, shields with each path, natural armor, magical armor, improvised armor).

### B2. Critical effects stress test

**✅ Trigger resolved:** all qualifying systems use the universal **Critical Die**. Success + Critical Die 10 = Crit+; failure + Critical Die 1 = Crit-. Other natural 10s/1s do not trigger a critical by themselves.

Remaining effect questions:
- Defensive Crit+: -1d10 per excess defensive success to the attacker's next attack against the same defender — test severity and duration.
- Passive Defense: critical success/failure eligibility has been reopened for stress testing.
- Attacker Crit-: -1d10 to next defense per natural 1 showing is confirmed; test **half Movement Speed** as the movement consequence instead of the previous no-further-movement rule.
- Defender Crit-: +1 damage per damage die is confirmed; define exact order with doubled crit damage and mixed damage, and test whether the defender also suffers the half-Movement consequence.

### B3. Overwhelming outcomes

**✅ Skills resolved:** OwS occurs at **150% of the normal Skill threshold, rounded up** (3 / 5 / 6 / 8 / 9). OwF occurs when a failed Skill check misses the normal threshold by **3 or more successes**. Simple Skill checks cannot produce OwF.

**✅ Combined Skill outcomes:** OwS may combine with Crit+; OwF may combine with Crit-. In extended checks, OwS/Crit+ are +2 success marks each, OwF/Crit- are +2 failure marks each, same-sign combinations automatically resolve the current stage.

**Still required:** determine whether Overwhelming outcomes need a generalized rule outside Skills/opposed systems, and finish Skill-specific examples for quality, time, materials, social outcomes, and other contextual consequences.

### B4. Reaction/timing rules

Define when AP can be reserved/spent, number of reactions, interrupt ordering, multiple defenders, counterattacks, counterspells, delayed actions, and simultaneous effects.

### B5. Size and Movement Units

Lock the complete Size ladder and feet-per-MU (or equivalent measurement). Confirm standard movement action count/cost and alternate movement types.

### B6. Magic maintenance and exceptional multi-turn casting

Identify the exact Magic Component that permits multi-turn AP expenditure and rewrite it as a true exception. Rebuild Concentration maintenance separately.

### B7. Counterspelling

Choose/convert opposing-Energy attack and opposing-Energy shield approaches under the modern opposed engine.

### B8. Advancement costs

Decide whether 1/2/3/4/5 remains the purchase ladder for Magic/Martial/Skills while Traits use 3/6/9/12/15, or whether costs should be unified differently.

## C. YELLOW — content/balance conversion

### C1. Individual Skills

Preserve degree capabilities but review outdated assumptions, fixed numbers, catastrophic/spectacular language, time increments, materials damage, and Skill-specific target numbers.

### C2. Skill modes and Teamwork

**✅ Hasty:** half normal time, -1d10 per task tier.

**✅ Meticulous:** double normal time, +1d10 per task tier.

**✅ Progressive/Productive/Ongoing:** use the same Skill thresholds; resolve the current task/stage at 4 success marks before 4 failure marks. Meaningful disruptions may force additional checks; routine sustained activity does not require pointless rerolls.

**✅ Teamwork:** assistance grants rerolls rather than bonus dice; normally one Helper, with 1 reroll untrained and 1 reroll per Training degree when trained. Each die can be rerolled only once, the new result replaces the old result, and the Critical Die may be rerolled.

**✅ Skills in combat:** active checks cost 1 AP, passive/reflexive checks cost 0 AP, helping costs 1 AP, actual task time still matters, and Hasty/Meticulous retain their normal time rules. A non-ongoing Meticulous check is the Specialist's only proactive action for the turn but does not prevent Active Defense or eligible reactions. Ongoing Skill use may restrict Active Defense when simultaneous performance is unreasonable, subject to Keeper judgment.

**✅ Skill/attack interaction:** independent Skill actions do not fail as a chain and do not grant generic attack bonuses. A Specialist may instead declare Skill checks as part of an integrated attack maneuver; each Skill AP grants +1d10 to the attack if every linked Skill check succeeds, while failure of any linked Skill check causes the integrated maneuver and attack to fail.

### C3. Magic Energy and Structure entries

Audit every entry's AP, potency, duration, area, target rules, alternate defenses, damage, and terminology. Spreadsheet calculators are not authority.

### C4. Traits

Finalize every cost, prerequisite, exclusion, body-plan interaction, natural weapon profile, sense, skin effect, Size effect, wing movement, Unnatural Hunger feeding/recovery, Putrid, Adhesive, and other negative/positive Trait effects.

### C5. Crafting / Quality / Durability

Wait for Skills and armor/mitigation decisions, then rebuild repeated progress, object Quality, repairs, breakage, and materials.

### C6. Carrying/exertion

Decide whether the recovered Toughness multipliers survive and translate speed penalties into modern Movement/MU.

### C7. Conditions glossary

Create one shared set of Conditions used by Martial, Magic, Traits, Crafting, and environment.

## D. GREEN — do not reopen casually

- d10 pool, 6–10 success.
- Stat Dice = 1 + floor(Stat/10).
- No automatic successes.
- Opposed success comparison.
- Combat tie = Glancing Blow, 1d10 base damage.
- Net attack successes become damage dice.
- Five tiers and 15/30/45/60/75 prerequisites.
- Training = +1d10 per degree; no +2-per-degree exceptions.
- Speed alone generates AP.
- AP = 1 + 2×floor(Speed/10).
- AP refresh; no next-turn carry.
- No normal AP accumulation across turns to enact one action.
- Maintenance is not enactment.
- Action ceilings 3/6/9/12/15.
- Initiative rolled once and remains static.
- Luck failure has no penalty; no Initiative-specific Luck cap.
- One defense path per roll: Agility/Unarmored, Insight/Evasion, Stamina/Armor.
- Passive Defense costs no AP; Active replaces Passive. Passive critical eligibility is intentionally reopened for stress testing.
- Single weapon profile unless explicit dual/hybrid construction.
- Universal Critical Die: success + Critical Die 10 = Crit+; failure + Critical Die 1 = Crit-.
- Attack Critical Success doubles damage dice.
- Skill thresholds = 2/3/4/5/6.
- Hasty = half time and -1d10 per task tier; Meticulous = double time and +1d10 per task tier.
- Extended Skill checks resolve at 4 success marks before 4 failure marks, with confirmed Critical/Overwhelming mark values.
- Generic favorable/unfavorable Skill modifiers are removed.
- Magic and Martial use the same base resolution engine.
- Creature Type is a Trait-based classification; Traits carry the cost.
- Negative Traits grant points only when taken at creation.
- Conditions should be unified, not source-specific bespoke systems.

## Recommended editing order

1. Finish individual Skill timing/examples and entry-by-entry Skill cleanup.
2. Armor/mitigation/defense equipment pass.
3. Martial Component conversion.
4. Character creation + Advancement economy.
5. Size/MU and reaction timing.
6. Critical-effect stress testing, including Passive Defense and movement consequences.
7. Magic Component/Energy conversion, including counterspelling and maintenance.
8. Trait-by-Trait pass.
9. Crafting/Quality/Durability.
10. World/social/travel cleanup and final prose integration.


---

# Chapter 11 — Source Map & Provenance

## Reconstruction status legend

- **✅ CONFIRMED** — established by later explicit decisions and treated as current canon unless deliberately reopened.
- **🔄 SUPERSEDED** — recovered source material that has been replaced by a later decision.
- **⚠️ REVIEW / CONVERSION** — concept or content is useful, but one or more mechanics must be reconciled with the current engine.
- **⬜ NEEDS DEVELOPMENT** — incomplete or absent; substantial design work remains.
- **❗ CONTRADICTION** — two surviving sources or decisions conflict and must not be silently reconciled.
- **💡 SUGGESTION** — design suggestion from this reconstruction pass; not canon unless Mike approves it.

**Authority used in this reconstruction:** newest explicit decisions in the current reconstruction work override older text; CLEAN source files are the baseline for material not subsequently changed. Archival Markdown is treated as a searchable transcription of its CLEAN source, not as independent canon. No discrepancy has been silently fixed.

## Source treatment

### CLEAN DOCX and archival Markdown

The Markdown companions used here are archival/searchable transcriptions of the CLEAN DOCX files. They do not independently establish newer canon. Where a transcription appears odd (for example, a suspicious number or typo), this reconstruction preserves the discrepancy and flags it instead of silently repairing it.

### Magic spreadsheet

`Magic Structure and Energies.xlsx` is treated as source material for **names, categories, tier placement, and relationships**. Calculator formulas are intentionally not used to establish current mechanics.

### Non-CLEAN files

No older non-CLEAN file was necessary for this pass. They remain available as archaeological evidence if a future question cannot be answered from the CLEAN set/current decisions.

## Chapter/source crosswalk

| Reconstruction chapter | Principal CLEAN sources |
| --- | --- |
| Core | General Rules; Combat; Specialist Basics |
| Specialist Creation | Specialist Basics; Creature/Traits for creation-economy conflict |
| Combat | Combat; General Rules; Martial; Magic |
| Skills | Skills; General Rules; Specialist Basics |
| Martial | Martial; Combat; Specialist Basics |
| Magic | Magic; Magic Structure and Energies workbook/transcription; Combat |
| Creatures & Traits | Creatures WIP; Creature layout; Creature traits; Specialist Basics |
| Crafting | Crafting and Materials; Skills; General Rules |
| World/Misc | General Rules; Combat; Specialist Basics |

## Known transcription/source discrepancies to keep visible

- CLEAN Skills transcription states normal Intermediate success target **26**; Mike recalled **24** during reconstruction. Do not silently choose one as historical truth until the original DOCX location is checked if the distinction matters. Since the modern system will not use summed totals, this is currently historical rather than blocking.
- CLEAN Skills contains wording such as "Simple five successful rolls. Intermediate four" where Basic may have been intended. Treat as a source inconsistency, not an invitation to auto-correct.
- CLEAN General Rules carrying/exertion contains at least one suspicious Speed/overload wording issue. Preserve until adjudicated.
- CLEAN Martial contains static values and old mitigation/Evasion sequencing alongside later-looking dice language. This is a conversion problem, not evidence for multiple concurrent resolution systems.

## Preservation principle

When a recovered entry contains both a strong concept and obsolete math, keep the concept and the obsolete math visible until the replacement is explicitly approved. The reconstruction should make it impossible to accidentally forget why a later rule exists.
