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
