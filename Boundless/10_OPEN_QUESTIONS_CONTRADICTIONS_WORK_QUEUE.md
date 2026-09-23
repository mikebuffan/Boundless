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

**Remaining Skill work:** Teamwork, Skills in combat, individual Skill timing/examples, and entry-by-entry cleanup. These no longer block the core threshold engine.

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

**⬜ Remaining:** Teamwork still needs a modern rule. Skills in combat remain under review.

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

1. Finish Skill Teamwork, Skills-in-combat, and individual Skill timing/examples.
2. Armor/mitigation/defense equipment pass.
3. Martial Component conversion.
4. Character creation + Advancement economy.
5. Size/MU and reaction timing.
6. Critical-effect stress testing, including Passive Defense and movement consequences.
7. Magic Component/Energy conversion, including counterspelling and maintenance.
8. Trait-by-Trait pass.
9. Crafting/Quality/Durability.
10. World/social/travel cleanup and final prose integration.
