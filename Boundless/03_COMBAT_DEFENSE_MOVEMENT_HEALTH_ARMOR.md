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
