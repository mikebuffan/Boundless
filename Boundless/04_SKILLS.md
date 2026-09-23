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
- CLEAN restrictions that require an untrained Specialist's Stat to qualify for the attempted degree, halve untrained dice, forbid meticulous attempts, or automatically make untrained failure disastrous are **🔄 superseded** by the modern "anyone can attempt" principle unless explicitly reintroduced later.

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

## 5. Hasty, Meticulous, Progressive/Productive, and Ongoing use

### Hasty and Meticulous

**✅ CONFIRMED**

**Hasty:** complete the task in half the normal time and apply **-1d10 per tier of task difficulty**.

**Meticulous:** take double the normal time and gain **+1d10 per tier of task difficulty**.

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

Extended tasks use the same normal Skill thresholds as ordinary checks. A current task or stage succeeds when the Specialist accumulates **4 success marks before 4 failure marks**; it fails when 4 failure marks are accumulated first.

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

- **Teamwork:** not fully reconstructed and still needs a modern rule.
- **Skills in combat:** CLEAN's 1 AP-per-check concept remains under review and has not yet been converted.

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
