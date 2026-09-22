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

There are no automatic successes. Critical Success and Overwhelming Success are special roll states rather than automatic successes.

## 2. Opposed and threshold checks

**✅ Opposed checks:** higher successes wins. Combat ties become Glancing Blows in the attacker's favor. Noncombat ties default to the minimum successful outcome unless the relevant subsystem specifies otherwise.

**⚠️ Threshold checks:** meeting or exceeding the threshold succeeds. The universal/Skill difficulty ladder is under active reconstruction. A provisional 2/3/4/5/6 success ladder is stress-tested in the Skills chapter but is **not yet canon**.

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

## 7. Critical Success, Critical Failure, and Overwhelming Success

**✅ Critical Success trigger:** the underlying action must succeed and must show the required natural 10s for its tier: Simple 1, Basic 2, Intermediate 3, Advanced 4, Master 5.

**✅ Attack Critical Success:** double the damage dice.

**⚠️ Provisional defensive Critical Success:** when an active defender wins and qualifies for a Critical Success, the attacker takes -1d10 per excess defensive success on their next attack against that same defender. Passive Defense cannot critically succeed.

**⚠️ Provisional attacker Critical Failure:** once the attack qualifies for Critical Failure using natural 1s, the attacker cannot move for the remainder of that turn and suffers -1d10 to their next defensive action per natural 1 showing on the failed attack.

**✅ Defender Critical Failure concept:** attacker gains +1 damage per damage die rolled, preserving the appropriate damage type.

**⚠️ Overwhelming Success:** every die in the available pool shows a success (6–10). It may occur with or without Critical Success. Mechanical effects outside ordinary success remain undefined, especially for Skills.

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
