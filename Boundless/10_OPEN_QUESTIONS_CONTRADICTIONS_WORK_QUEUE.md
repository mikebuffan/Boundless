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

### A1. Skill difficulty ladder

**⚠️ Current candidate:** 2 / 3 / 4 / 5 / 6 successes for Simple through Master.

**Still required:** test untrained, under-degree, equal-degree, over-degree, high-Stat, favorable/unfavorable, Hasty, Meticulous, repeated/progressive, and opposed Skill use. Decide whether every Skill difficulty uses the same five thresholds or whether situational difficulty modifies the pool/threshold.

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

- Defensive Critical Success: -1d10 per excess defense success to next attack against same defender — test severity and duration.
- Attacker Critical Failure: no further movement + -1d10 next defense per natural 1 — test high-pool failure spikes.
- Defender Critical Failure: +1 damage per damage die — define exact order with doubled crit damage and mixed damage.

### B3. Overwhelming Success

Current trigger = all dice succeed. Effects undefined. Larger pools make the event rarer; decide whether this rarity is intentional. Determine interaction with Critical Success, Skill quality, time, materials, social outcomes, and opposed checks (if Overwhelming remains Skill/unopposed-only).

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

### C2. Hasty / Meticulous / Progressive / Ongoing / Teamwork

Rebuild on success counting. Avoid unnecessary arithmetic layers.

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
- Passive Defense no AP and cannot crit; Active replaces Passive.
- Single weapon profile unless explicit dual/hybrid construction.
- Attack Critical Success doubles damage dice.
- Magic and Martial use the same base resolution engine.
- Creature Type is a Trait-based classification; Traits carry the cost.
- Negative Traits grant points only when taken at creation.
- Conditions should be unified, not source-specific bespoke systems.

## Recommended editing order

1. Skill thresholds and Skill modes.
2. Armor/mitigation/defense equipment pass.
3. Martial Component conversion.
4. Character creation + Advancement economy.
5. Size/MU and reaction timing.
6. Critical stress testing.
7. Magic Component/Energy conversion, including counterspelling and maintenance.
8. Trait-by-Trait pass.
9. Crafting/Quality/Durability.
10. World/social/travel cleanup and final prose integration.
