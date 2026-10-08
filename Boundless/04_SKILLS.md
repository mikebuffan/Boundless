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

### Skill Synergy and Limited Substitution

**✅ CONFIRMED**

Some Skills naturally overlap without being interchangeable. Boundless handles that overlap through **Synergy** and, where a Skill entry explicitly allows it, **Limited Substitution**.

#### Skill Synergy

When two Skills materially contribute to the same task, one Skill is the **Primary Skill** and determines the governing Stat, task tier, and base Skill check. One other relevant Skill may act as the **Supporting Skill**.

- The Supporting Skill contributes **+1d10 per degree of Training**: Simple +1d10, Basic +2d10, Intermediate +3d10, Advanced +4d10, Master +5d10.
- Only the Supporting Skill's **Training dice** are added. Its governing Stat dice are not added.
- Normally, only **one Supporting Skill** may provide Synergy to a check.
- The Primary and Supporting Skills must both materially apply to the task. A merely plausible association is not enough.
- Individual Skill entries should identify common or intended Synergies where useful, while the Keeper may approve unusual combinations that genuinely fit the situation.
- Synergy is internal to one Specialist and is distinct from Teamwork/Assistance.

The purpose of Synergy is to reward meaningful investment in related Skills without allowing overlapping Skills to replace one another or creating unlimited dice-pool stacking.

#### Limited Substitution

Certain Skill degrees may explicitly grant narrow competency in another Skill for a specific purpose.

- Unless the entry says otherwise, Limited Substitution allows the Specialist to treat themselves as having **Simple Training** in the substituted Skill for the stated purpose only.
- The substituted check uses the **governing Stat and normal rules of the substituted Skill**, including the +1d10 from Simple effective Training.
- Limited Substitution does **not** grant the substituted Skill generally, satisfy unrelated prerequisites, or provide access to that Skill outside the stated context.
- Limited Substitution does not itself create a Synergy bonus.
- If the Specialist already has actual Training in the substituted Skill, use that Training normally instead of the substitution. When appropriate, the original Skill may then provide Synergy.

This lets broad practical expertise cover a narrow neighboring task while preserving a strong incentive to invest in the specialized Skill itself.

#### Hard boundaries between related Skills

Related Skills may overlap in subject matter without becoming interchangeable. Each Skill should retain a clear mechanical and fictional job.

- **Synergy rewards overlap; it does not erase boundaries.** A related Skill may support the Primary Skill when both materially contribute, but the Primary Skill still determines what action is actually being attempted.
- **Limited Substitution is narrow by design.** It grants only the explicitly stated competency for the explicitly stated context and does not turn one Skill into another.
- A broad Skill should not absorb the defining functions of a narrower Skill merely because both concern the same subject.
- When two Skills seem similar, define the distinction in terms of what each one actually does at the table, then use Synergy where their expertise genuinely intersects.

> **Reconstruction editorial note:** final rulebook examples should remain setting-neutral and durable. Avoid contemporary or real-world cultural references, celebrity references, television/film jokes, or similar allusions unless a specific setting text deliberately calls for them.

#### Synergy callout candidates

The following pairings are being retained as candidates for later rulebook margin notes, tooltips, sidebars, or worked examples. They demonstrate Synergy; they are not automatically applicable unless both Skills materially contribute to the particular task.

- **Hunting + Camouflage:** conceal oneself from animal prey using prey knowledge and actual camouflage technique.
- **Hunting + Tracking:** follow animal prey by combining behavioral knowledge with interpretation of physical signs.
- **Hunting + Trapping:** choose and place traps against particular prey using prey knowledge and trapping expertise.
- **Listening + Hunting:** locate or interpret animal prey by sound.
- **Listening + Tracking:** follow an unseen moving target when sound materially contributes.
- **Listening + Search:** investigate hollow spaces, concealed mechanisms, or hidden areas where acoustic cues guide the examination.
- **Listening + Engineering:** diagnose machinery, mechanisms, or structural problems by sound.
- **Listening + Mimicry:** analyze subtle vocal details before reproducing them.
- **Pick Pocket + Sleight of Hand:** covertly transfer an object while concealing the hand movement or object through palming or misdirection.
- **Spot + Search:** use a visual irregularity noticed with Spot to guide a deliberate Search.
- **Bowyer + Carpentry:** difficult wooden components or elaborate stocks.
- **Bowyer + Blacksmithing/Weapon Smithing:** unusual metal components or reinforcement.
- **Bowyer + Engineering:** unconventional mechanical crossbow designs or unusually complex mechanisms.
- **Bowyer + Fletching:** deliberately tune ammunition characteristics to a particular weapon while keeping ammunition construction under Fletching.
- **Calligraphy + Counterfeiting:** reproduce handwriting or formal script as one component of a convincing forged document.
- **Calligraphy + Scribe:** accurately reproduce lengthy written material while preserving a formal or decorative hand.
- **Calligraphy + History/Research:** interpret difficult historical handwriting or script when visual script expertise materially aids the inquiry.
- **Carpentry + Wood Carving:** construct a functional wooden object while intricate carved ornamentation materially contributes to the same project.
- **Carpentry + Engineering:** fabricate wooden components for a genuine mechanical system whose function depends on both precise woodworking and mechanical design.
- **Cartography + Navigation:** use a map and route-finding expertise together to plot or follow a difficult route.
- **Cartography + Geography/Local Geography:** convert broad or local geographic knowledge into a more accurate spatial representation.
- **Cartography + Cryptography:** create or interpret an encoded map without collapsing mapmaking and codebreaking into the same Skill.
- **Counterfeiting + Scribe:** reproduce lengthy or structurally complex documents while preserving the broader deception.
- **Counterfeiting + Jeweler:** imitate jewelry, precious objects, maker marks, settings, or decorative details.
- **Counterfeiting + Sewing:** imitate uniforms, luxury garments, textile labels, stitching, or construction details.
- **Counterfeiting + Artistry:** imitate artwork, decorative finishes, or sculptural presentation.
- **Counterfeiting + Heraldry:** reproduce coats of arms, seals, insignia, lineage marks, or institutional symbols.
- **Counterfeiting + Engineering:** imitate a complex device whose apparent construction or mechanical details matter to the deception.
- **Disable Device + Engineering:** sabotage or bypass an unfamiliar complex mechanism where engineering knowledge materially aids the manipulation.
- **Disable Device + Lock Picking:** defeat a locking mechanism when both normal lock manipulation and mechanical interference materially contribute.
- **Disable Device + Trap Making:** neutralize a trap by combining knowledge of trap construction with practical interference.
- **Disable Device + Explosives:** disable an explosive device whose trigger mechanism and explosive charge both matter.
- **Escape + Rope Use:** work free of sophisticated rope bindings by combining escape technique with knowledge of knots, tension, and rope construction.
- **Rope Use + Escape:** design bindings specifically to eliminate common escape opportunities.
- **Escape + Lock Picking:** defeat a locked restraint when body positioning and lock manipulation both materially contribute.
- **Escape + Sleight of Hand:** conceal or manipulate a small escape aid while restrained or searched.
- **Escape + Acrobatics:** use body positioning or flexibility to escape confinement where geometry and movement are central.
- **Fletching + Weapon Smithing:** create specialized metal heads or unusual ammunition hardware.
- **Fletching + Poisons:** construct ammunition intended to retain and deliver a toxin effectively.
- **Fletching + Explosives:** construct ammunition that safely carries and survives launch with an explosive payload.
- **Fletching + Alchemy/Apothecary:** construct ammunition to carry and deliver chemical or alchemical payloads.
- **Fletching + Hunting:** tailor ammunition to particular prey when prey knowledge materially affects the design.
- **Herbology + Geography:** use habitat and terrain knowledge to support plant identification or likely distribution.
- **Apothecary + Herbology:** formulate a plant-based preparation using accurate botanical identification and ingredient selection.
- **Poisons + Herbology:** identify, harvest, or prepare plant-derived toxins using both botanical and toxicological expertise.
- **Alchemy + Herbology:** use unusual plant materials in an alchemical preparation when botanical properties materially matter.
- **Jeweler + Metallurgy:** work unusual precious-metal alloys or materials whose composition materially affects fabrication.
- **Jeweler + Appraise:** assess jewelry when workmanship, materials, and market valuation all materially contribute.
- **Jeweler + Artistry:** create jewelry whose visual composition materially contributes beyond technical fabrication.
- **Jeweler + Engineering:** construct jewelry containing genuine mechanical elements rather than ordinary clasps or hinges.
- **Leatherworking + Sewing:** construct mixed leather-and-textile garments or goods.
- **Leather Armoring + Leatherworking:** construct leather armor whose fitting, straps, lining, or non-protective leather components materially benefit from general leathercraft.
- **Leatherworking + Animal Husbandry:** create specialized saddles, harness, or tack fitted to particular animals.
- **Leatherworking + Artistry:** create elaborate tooling, relief, or decorative leatherwork.
- **Lock Picking + Engineering:** defeat unfamiliar complex mechanical locks using both mechanism knowledge and manipulation expertise.
- **Lock Picking + Sleight of Hand:** manipulate a lock while keeping the picking action concealed.
- **Musical Instrument + Singing:** perform while accompanying one's own voice or another singer where both skills materially contribute.
- **Musical Instrument + Writing:** compose songs where lyrical and instrumental composition both materially matter.
- **Musical Instrument + Acting:** perform music as part of a theatrical or character-driven presentation.
- **Musical Instrument + Wood Carving:** construct or modify a wooden instrument component where playing knowledge materially informs its shape or function.
- **Poisons + Apothecary:** create a toxic preparation whose formulation overlaps ordinary medicinal techniques.
- **Poisons + Chemistry:** analyze or formulate unusual chemical toxins using both toxicology and chemical knowledge.
- **Poisons + Alchemy:** work with alchemically altered or supernatural toxic preparations where both systems genuinely apply.
- **Poisons + First Aid:** identify or respond to poisoning when symptoms, exposure, and treatment knowledge materially overlap.
- **Rope Use + Climbing:** build and use technical climbing, rappelling, or rescue rigging.
- **Rope Use + Engineering:** operate or construct a lifting system combining rope rigging with genuine machinery.
- **Trap Making + Rope Use:** build snares, net traps, trip systems, or tensioned-line mechanisms.
- **Scribe + Researching:** collate sources, extract citations, or maintain structured scholarly records.
- **Scribe + Administration:** maintain complex organizational records where both accurate transcription and administrative structure matter.
- **Sewing + Artistry:** create textile work whose visual design materially contributes beyond construction.
- **Sewing + Rope Use:** construct and rig sails, tents, awnings, nets, or similar large textile systems.
- **Sleight of Hand + Acting:** perform concealed object manipulation within a staged character performance.
- **Sleight of Hand + Bluff:** use verbal deception to support a covert manual manipulation.
- **Trap Making + Trapping:** design or construct traps around the behavior and physical characteristics of intended prey.
- **Trap Making + Engineering:** construct unusually complex mechanical traps.
- **Wood Carving + Artistry:** create sculpture where artistic composition and carving technique both materially contribute.
- **Wood Carving + Musical Instrument:** shape a wooden instrument component where acoustic or playing knowledge materially affects the work.
- **Counterfeiting + Wood Carving:** reproduce distinctive carved ornament or sculptural details as part of a convincing imitation.
- **Writing + Researching:** produce evidence-based long-form work from gathered and cross-referenced sources.
- **Writing + History:** compose historical narrative where factual historical expertise materially contributes.
- **Writing + Scribe:** turn notes, dictation, or source material into a structured formal manuscript.
- **Writing + Calligraphy:** produce authored work whose formal handwritten presentation materially matters.
- **Writing + Musical Instrument:** compose lyrics and music as parts of the same song.
- **Writing + Public Speaking:** compose a speech specifically for effective spoken delivery.
- **Writing + Bluff:** construct a deliberately deceptive written narrative intended to be believed.
- **Counterfeiting + Writing:** forge a document whose wording and physical authenticity both materially matter.
- **Acting + Mimicry:** impersonate a particular person by combining role performance with specific vocal and behavioral reproduction.
- **Acting + Disguise:** sustain an impersonation where both physical appearance and behavior materially contribute.
- **Acting + Bluff:** support a false claim with a deliberately performed emotional state or role.
- **Acting + Public Speaking:** deliver a staged or in-character address where both performance and audience communication materially matter.
- **Acting + Musical Instrument:** perform music as part of a character-driven or theatrical presentation.
- **Acting + Singing:** perform a vocal role where both character portrayal and singing materially contribute.
- **Acting + Empathy:** portray an emotional state more convincingly when understanding that state materially contributes to the performance.

A useful finished callout should show the **Primary Skill**, the **Supporting Skill**, why both apply, the Supporting Skill's Training dice, and—where useful—why another superficially related Skill does not apply.

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
> **Status:** ✅ CONFIRMED except blast-target resolution — capability progression, Yield terminology, Yield/tier structure, radius control, and Trap Making interaction locked. The rule for creatures caught inside a blast remains intentionally unresolved until Combat reactions/defenses are finalized.

Explosives governs the safe handling, identification, creation, modification, timing, disabling, and bypassing of explosive devices. Most uses are resolved as normal Skill checks. Creating an explosive with a defined destructive output additionally uses **Yield**.

#### Yield

**Yield** measures the destructive output of an explosive and uses the same numerical tier bands as the normal 3/6/9/12/15 action ceilings.

| Yield | Minimum creation tier |
| ---: | --- |
| 1–3 | Simple |
| 4–6 | Basic |
| 7–9 | Intermediate |
| 10–12 | Advanced |
| 13–15 | Master |

Each point of Yield produces **1d10 damage** and a **5-foot default blast radius**. Thus, Yield 1 produces 1d10 damage in a 5-foot default radius, Yield 6 produces 6d10 in a 30-foot default radius, and Yield 15 produces 15d10 in a 75-foot default radius.

The desired Yield determines the minimum task tier for creating the explosive, and the Specialist must possess sufficient Explosives Training to use that degree's capability. A Specialist with higher Training may deliberately create a lower-Yield device.

For example, creating a Yield 4 explosive is a **Basic** Explosives task. If successfully created, it deals **4d10 damage** in a **20-foot default radius** before any Advanced radius control is applied.

Yield measures destructive power only. It does not automatically determine craftsmanship, reliability, durability, concealment, or other future equipment/crafting qualities.

- **Simple:** Able to safely work with ordinary fuse-and-powder explosive devices and materials, including cannon charges, dynamite, grenades, and similar devices. Simple Training permits creation up to **Yield 3** where the required materials, tools, and circumstances permit.
- **Basic:** Able to precisely time fuse-and-powder explosives, create or protect waterproof fuses, and perform more reliable modifications to such devices. Basic Training permits creation up to **Yield 6**. Simple and Basic Explosives applications may be incorporated into Trap Making; when both Skills materially contribute to the task, they may use **Synergy** under the normal rules.
- **Intermediate:** Able to work with more sophisticated liquid and solid chemical reactions to produce explosive devices. Intermediate Training permits creation up to **Yield 9**.
- **Advanced:** Able to create shaped charges and exercise deliberate control over blast geometry. Advanced Training permits creation up to **Yield 12**. The Specialist may reduce an explosive's default blast radius, normally in 5-foot increments, or shape the blast so that the destructive force is directed into a smaller or more useful area. Reducing or shaping the blast does **not** reduce the explosive's Yield or damage and does not by itself raise the task tier. Radius control cannot create more total destructive power or greater maximum reach than the explosive's normal Yield would support; exact combat-area templates, if needed, will be finalized with Combat.
- **Master:** Able to recognize explosive devices, components, and explosive-capable substances from minute but ordinary signs such as chemical odors, residue, construction details, unusual wiring, disturbed fittings, or other physical evidence. This is exceptional expertise, not supernatural detection. Master Training permits creation up to **Yield 15** and allows all Explosives applications to be incorporated into Trap Making, using Synergy when both Skills materially contribute.

Handling, identifying, modifying, disabling, bypassing, or otherwise working with an explosive without creating a new destructive output uses the normal Skill task-tier rules. The Keeper determines the task tier from the device, materials, complexity, condition, time pressure, access, and circumstances rather than from the Specialist's Training degree alone.

Hasty and Meticulous use follow the normal Skill rules when the specific task can genuinely be rushed or performed more carefully. The Keeper may rule that a particular explosive procedure cannot safely or meaningfully be accelerated.

#### Blast-target resolution — intentionally pending

This entry currently defines an explosive's **Yield, damage dice, default blast radius, and Advanced radius control only**. It does **not** yet determine how creatures or objects inside the blast area respond mechanically.

Whether a target receives a defense roll, reaction, saving throw, cover interaction, mitigation opportunity, or another combat response will be decided during the Combat reaction/defense pass and then propagated back into Explosives. The recovered legacy statement that creatures inside the blast are automatically hit is **not current authority** unless it is explicitly reconfirmed during that pass.

### Fishing:
> **Status:** ✅ CONFIRMED — capability progression and modern Skill handling locked.

Specialists with Fishing skill gain knowledge of techniques used to catch fish and other aquatic wildlife. Fishing is normally treated as an **Ongoing Skill** rather than requiring a check for every cast or minor attempt.

**Default interval:** approximately **1 hour per check** when a check is needed. The Keeper may adjust the interval when the fishing method clearly operates on a different timescale, such as traps, nets, spearfishing, hatchery work, or other specialized methods.

Task tier is determined by the prey, environment, method, scarcity, conditions, and objective rather than by the Specialist's Training degree. Training unlocks capabilities; it does not automatically set task difficulty.

- **Simple:** Able to use ordinary fishing equipment and methods, including rods, hooks, standard bait and lures, and nets.
- **Basic:** Able to improvise functional substitutes for ordinary fishing equipment when proper gear is unavailable.
- **Intermediate — I know where it is:** Able to read water, terrain, season, weather, depth, current, habitat, signs, and similar clues to identify where particular types of aquatic wildlife are most likely to be found.
- **Advanced — I know how this kind of fish behaves:** Understands feeding habits, activity cycles, preferred prey, responses to light, temperature and current, spawning behavior, and similar patterns well enough to choose appropriate bait, lure, presentation, timing, depth, and fishing method.
- **Master — I know specifically how to get that fish to bite:** Able to deliberately target a specific species, narrow category of prey, or potentially an individual specimen by tailoring bait, lure, presentation, and technique to its specific behavior, while reducing unwanted catches when circumstances permit.

A higher Training degree does not automatically make the check a higher-tier task. For example, a Master-trained Specialist deliberately targeting a common species in a stocked lake may still face a Simple or Basic task.

**Hasty Fishing:** normally unavailable. Fishing generally cannot be made twice as fast merely by trying harder. The Keeper may allow Hasty use only when the method and circumstances can genuinely be accelerated, such as certain hatchery, netting, collection, or similarly obvious cases.

**Meticulous Fishing:** allowed when circumstances permit and uses the normal Meticulous rules.

Routine fishing does not require repeated checks merely to manufacture failure. Make checks at meaningful intervals or when conditions change enough to threaten progress.

The amount or exact nature of the catch is contextual rather than fixed to a universal quantity table. Exceptional outcomes should follow the circumstances. Appropriate examples include a better-than-expected catch, reduced time, an unusually desirable specimen, preserved bait or materials, useful information about the area, damaged tackle, lost bait, a fouled net, spooked prey, or attracting an unwanted catch. These are examples rather than mandatory universal results.

### Hunting:
> **Status:** ✅ CONFIRMED — capability progression, Synergy/Substitution relationships, and modern Skill handling locked.

Hunting governs the hunt itself: understanding wild prey, choosing an approach, predicting behavior, creating opportunities, and adapting when the prey changes its behavior. It does not replace specialized Skills such as Camouflage, Tracking, Trapping, or Trap Making, and it does not replace Combat/Martial rules when a hunt becomes a fight.

Hunting is commonly treated as an **Ongoing Skill**. It has no universal fixed interval; checks occur at meaningful stages of the hunt, such as locating likely prey, approaching it, setting an ambush, maintaining contact during a pursuit, or adapting when circumstances change.

Task tier is determined by the prey, terrain, danger, rarity, circumstances, and objective rather than by the Specialist's Training degree. Size alone does not determine whether prey may be hunted.

- **Simple — I can hunt:** Understands the basic habits of common wild game and can conduct an ordinary hunt using appropriate weapons, nets, positioning, and hunting methods. If the situation becomes structured combat, attacks and defenses use the normal Combat/Martial rules.
- **Basic — I know how not to be noticed by my prey:** Understands how animal prey perceives its surroundings well enough to use blinds, natural cover, decoys, positioning, and basic visual concealment against it. If the Specialist has no Camouflage Training, Basic Hunting grants **Limited Substitution: Simple Camouflage** when concealing themselves specifically from animal prey. If the Specialist has Camouflage Training, Hunting and Camouflage may use **Synergy** when both materially apply.
- **Intermediate — I know where it is going:** Reads prey behavior well enough to identify likely feeding areas, watering points, bedding areas, travel routes, escape paths, and other probable movements. If the Specialist has no Tracking Training, Intermediate Hunting grants **Limited Substitution: Simple Tracking** when following animal prey. If the Specialist has Tracking Training, Hunting and Tracking may use **Synergy** when both materially apply.
- **Advanced — I know how to make it do what I want:** Manipulates prey behavior through calls, scents, musks, lures, decoys, wind direction, flushing, driving, and similar techniques. The Specialist also understands how and where traps should be employed against particular prey. If the Specialist has no Trapping Training, Advanced Hunting grants **Limited Substitution: Simple Trapping** when selecting and placing an existing basic trap specifically for animal prey. If the Specialist has Trapping Training, Hunting and Trapping may use **Synergy** when both materially apply.
- **Master — I know how to hunt that specific prey:** Can plan and conduct hunts against exceptionally elusive, dangerous, unusual, or cunning wild prey; deliberately target a particular specimen; anticipate likely reactions to the hunters; and adapt the hunt when the prey changes its behavior. Master Hunting may use Synergy with the relevant specialized Skill but does not increase Limited Substitution above Simple Training.

**Camouflage, Tracking, and Trapping remain distinct Skills.** Hunting provides prey-specific knowledge and may support them through Synergy. **Trap Making** is also distinct: Hunting may help determine what sort of trap would be useful against particular prey, but it does not grant Limited Substitution in Trap Making or replace the ability to construct sophisticated traps.

**Hasty Hunting:** allowed when the hunting method can genuinely be rushed, such as pressing a stalk, flushing prey early, or sacrificing careful positioning for speed. Use the normal Hasty rules.

**Meticulous Hunting:** allowed when circumstances permit and uses the normal Meticulous rules.

Exceptional outcomes should follow the circumstances rather than a universal catch/kill table. Success may create a clean opportunity without itself resolving a combat encounter. Critical or Overwhelming results may provide superior positioning, unusually accurate behavioral insight, reduced time, preservation of resources, or another context-appropriate advantage; severe failures may spook prey, lose the trail, expose the hunter, waste resources, or otherwise complicate the hunt.

### Listening:
> **Status:** ✅ CONFIRMED — capability progression, passive/active handling, range convention, and human-limit boundary locked.

Listening represents trained auditory awareness, interpretation, localization, and spatial inference. It never grants supernatural hearing or true echolocation; any information gained must be reasonably present in audible sound, echoes, resonance, reverberation, or other acoustic cues.

- **Simple — I notice unusual sounds:** Able to passively notice abnormal or noteworthy sounds that might otherwise escape attention. Passive or reflexive Listening checks follow the normal passive Skill rules and may be rolled secretly by the Keeper when revealing that a check occurred would itself give away information.
- **Basic — I can hear it through that:** Able to deliberately listen through ordinary barriers such as doors, windows, walls, floors, or similar obstructions when enough sound can reasonably pass through them. The barrier, distance, sound level, and surrounding noise help determine task difficulty.
- **Intermediate — I can tell you something about what I heard:** Able to interpret vocal and environmental sounds to infer useful information such as direction, approximate distance, relative size, number of sources, movement, speed, or similar details when those details are reasonably conveyed by the sound.
- **Advanced — I can isolate it and tell roughly where it is:** Able to separate meaningful sounds from heavy background noise, distinguish overlapping sources, maintain attention on a chosen source, and track its approximate position as it moves. An unseen or invisible creature that is making enough noise to be heard may be localized and followed by sound, but Listening does not make it visible, negate concealment generally, or reveal information the sound itself does not carry.
- **Master — I can use sound to understand the nearby space:** Able to interpret echoes, resonance, reverberation, footsteps, breathing, ambient noise, and other ordinary acoustic cues to form a rough mental model of nearby surroundings. This may reveal openings, large obstacles, approximate room dimensions, hollow spaces, unseen movement, or similar spatial information when the environment actually provides sufficient acoustic cues. A Master Listener may carefully navigate an unfamiliar dark space using ordinary environmental sound, but does not gain sight-equivalent perception.

#### Auditory distance and position

When Listening provides positional or distance information, describe that information in **5-foot increments** where appropriate: approximately 10 feet, 25 feet, 60 feet, and so on. This is a measurement convention, not guaranteed five-foot precision. Distance, barriers, echoes, competing noise, source volume, room shape, environmental acoustics, and movement may reduce precision or make localization impossible. In exceptionally clear conditions a successful check may effectively identify a five-foot area; in poor conditions the Keeper may give only a broader estimate or direction.

#### Human-limit boundary

Listening does not become supernatural, even at Master degree. A completely silent creature cannot be detected by sound alone. Listening cannot perceive color, writing, silent visual details, or identify objects with sight-like precision. It cannot freely substitute for vision, and darkness or blindness may still impose whatever limitations the relevant rules establish. The Keeper should permit impressive human-level feats while rejecting information that the available sound could not reasonably provide.

#### Active and passive use

Passive or reflexive Listening checks cost no AP in structured combat under the normal Skill rules. Deliberately stopping to listen is an active Skill check and costs 1 AP. Passive Listening should be rolled only when there is something meaningful to detect or when circumstances materially change, not repeatedly merely to manufacture failure.

When another creature is deliberately trying to avoid making noise, Listening may be opposed by Sneaking or another Skill that actually governs the attempt to remain unheard.

**Hasty Listening:** applies only when a meaningful listening interval can actually be shortened, such as taking a very quick listen at a door before moving on. Reflexive passive checks are not Hasty.

**Meticulous Listening:** allowed when circumstances permit and uses the normal Meticulous rules, representing deliberate concentration, reduced movement, and additional time spent isolating or interpreting sound.

Common Synergies may include Hunting when identifying or locating animal prey by sound, Tracking when sound materially assists in following a moving target, Search when detecting hollow spaces or concealed mechanisms, Engineering when diagnosing machinery acoustically, and Mimicry when closely analyzing vocal details. These are examples rather than an exhaustive list.

### Pick Pocket:
> **Status:** ✅ CONFIRMED — capability progression, opposed resolution, Synergy relationship, and combat boundary locked.

Pick Pocket governs the covert transfer of objects to or from another creature without their knowledge. It is distinct from Sleight of Hand: Pick Pocket focuses on taking from or planting on another creature, while Sleight of Hand focuses on palming, concealing, revealing, and manipulating objects through dexterity and misdirection.

- **Simple:** Able to remove or plant a hand-sized or smaller loose object on a sleeping or otherwise substantially unaware creature without disturbing them.
- **Basic:** Able to remove or plant larger loose objects from a sleeping or otherwise substantially unaware creature, provided doing so is physically plausible without obviously disturbing them.
- **Intermediate:** Able to remove or plant a hand-sized or smaller **unsecured** object from or on a conscious creature without their knowledge.
- **Advanced:** Able to use misdirection, timing, crowd movement, distraction, or similar techniques to remove or plant larger unsecured objects from or on a conscious creature without their knowledge.
- **Master:** Able to attempt to remove or plant worn, secured, or casually held objects on a conscious creature without their knowledge when physically plausible.

Master Pick Pocket does not replace combat disarm mechanics. An object that is actively wielded, firmly gripped, or being defended in structured combat is not normally a Pick Pocket target merely because the Specialist has Master Training. Casual possession, loose handling, accessible worn items, belt pouches, jewelry, keys, loosely held objects, and similar targets remain appropriate when circumstances permit.

#### Resolution

Against a sleeping, unaware, or otherwise non-opposing target, use a normal task tier based on factors such as object size, location, how securely it is attached, the amount of contact required, clothing or other obstructions, and how likely the target is to notice disturbance.

Against a conscious target capable of noticing the attempt, Pick Pocket is normally an **opposed check**. **Spot** is the default opposing Skill when the target is visually detecting the covert action, but the Keeper may use Listening or another Skill when it more directly governs detection in the circumstances.

A failed Pick Pocket check does not automatically mean the target identifies the Specialist unless the opposed result or situation supports that conclusion. Exact consequences follow the circumstances.

#### Synergy

**Pick Pocket and Sleight of Hand** are a common Synergy pairing when both materially contribute to the same action. For example, Pick Pocket may be the Primary Skill when lifting a purse while Sleight of Hand provides Supporting Skill dice for concealing the motion or immediately palming the object.

Pick Pocket does not grant Limited Substitution in Sleight of Hand. Each Skill remains independently valuable.

Other Skills may support Pick Pocket when genuinely relevant, such as Bluff, Acting, or another distraction-oriented Skill, but only one Supporting Skill may provide Synergy to a given check under the normal Synergy rules.

#### Pace and combat use

**Hasty Pick Pocket:** allowed when the attempt can genuinely be rushed, representing a quick grab or poorly timed opportunity. Use the normal Hasty rules.

**Meticulous Pick Pocket:** allowed when circumstances permit, representing careful observation, waiting for the ideal movement or distraction, and selecting the best moment to act. Use the normal Meticulous rules.

In structured combat, Pick Pocket follows the normal Skill-in-combat rules. An ordinary active attempt costs 1 AP. Pick Pocket may participate in an integrated maneuver only when the action is physically plausible and the object is a valid Pick Pocket target rather than an actively defended combat object.

Exceptional outcomes should be contextual. Critical or Overwhelming success might allow the transfer to go entirely unnoticed, conceal evidence of the action, take advantage of an unexpected opening, or accomplish a particularly difficult placement. Severe failure might expose the attempt, disturb the target, drop the object, snag clothing, or otherwise create an appropriate complication.

### Spot:
> **Status:** ✅ CONFIRMED — capability progression, passive/active handling, Search boundary, and common opposed uses locked.

Spot governs **rapid visual perception**: noticing movement, contrast, irregularities, and visible clues without conducting a deliberate investigation. **Search** governs methodical examination. Spot answers, “What do I notice by looking?” Search answers, “What do I find when I deliberately inspect this?”

- **Simple — I notice the obvious:** Quickly notices conspicuous visual details, movement, strong contrast, or something clearly out of place.
- **Basic — I notice subtle irregularities:** Picks out less obvious visible discrepancies without conducting a methodical search, such as a slightly different board, an unnatural shadow, a small crack, a mismatched outline, or faint movement in clutter.
- **Intermediate — I notice without looking for it:** Develops strong peripheral and environmental awareness. The Specialist may receive **passive Spot checks** for visual details that an ordinary observer would normally need to deliberately scan for, particularly movement, contrast, or environmental changes.
- **Advanced — I can pick something out of visual chaos:** Distinguishes relevant visual information in crowds, clutter, foliage, smoke, poor lighting, rapid movement, or other visually busy environments. The Specialist can maintain visual attention on a chosen subject and is especially capable of detecting deliberate visual concealment when there are actual visible cues to notice.
- **Master — I notice what almost nobody else would:** Recognizes minute visible disturbances and inconsistencies, such as a polished spot where something has repeatedly been touched, subtly disturbed dust, minute displacement of an object, faint bleaching where a book has been left open, an almost imperceptible seam, or tiny changes in posture or movement. Master Spot may reveal that something is wrong or has changed, but does not automatically reveal the hidden cause.

#### Spot and Search

Spot is immediate or rapid observation, primarily visual, and may be passive. It normally does not involve touching, opening, moving, measuring, or systematically inspecting things.

Search is deliberate investigation, normally active, and takes time. It may involve manipulating objects and carefully examining an area or item. Concealed compartments, trap triggers, secret doors, and hidden objects are normally Search territory once deliberate examination begins.

Spot and Search may use **Synergy** when both materially contribute. For example, noticing a suspicious seam with Spot may allow Spot to support a later Search check focused on that wall. Search does not automatically support a later Spot check merely because the Specialist had previously searched the area.

#### Opposed uses

Spot is a common opposing Skill against **Hiding**, **Camouflage**, **Pick Pocket**, **Sleight of Hand**, and other visually concealed actions when sight is genuinely how the action might be detected. If another sense or Skill more directly governs detection, use that instead.

#### Active and passive use

Passive or reflexive Spot checks cost no AP in structured combat under the normal Skill rules. Deliberately taking a quick visual scan is an active Spot check and costs 1 AP. An active Spot check is still a rapid visual scan, not a Search.

**Hasty Spot:** allowed when a meaningful observation interval can genuinely be shortened, such as taking only a quick glance instead of a normal scan. Use the normal Hasty rules.

**Meticulous Spot:** allowed when the Specialist spends additional time observing carefully without shifting into methodical physical investigation. Once the action becomes systematic examination or manipulation of the environment, use Search instead.

#### Distance and position

Spot has no universal fixed range. Whether a visual check is possible and its task tier depend on factors such as object size, lighting, weather, contrast, intervening terrain, concealment, and distance.

When Spot provides approximate positional information, use **5-foot increments** where that level of precision is reasonable, consistent with the Listening convention. This is a measurement convention rather than guaranteed five-foot accuracy.

Exceptional outcomes should be contextual. Critical or Overwhelming success may reveal an especially subtle clue, preserve awareness of multiple relevant visual details, notice a change earlier than expected, or provide unusually precise visual information. Severe failure may cause the Specialist to focus on the wrong detail, miss meaningful movement, lose track of a subject, or draw an incorrect conclusion from what was seen, where appropriate.

## Proficiency

### Professional tools, materials, and workspace

**✅ CONFIRMED**

Professional and crafting Skill capabilities assume access to the **tools, materials, and workspace reasonably required for the task** unless the Skill explicitly states otherwise.

Missing, damaged, improvised, or inadequate equipment may increase the task tier, restrict what can physically be attempted, prevent Hasty or Meticulous use, or make the task impossible. Appropriate improvised tools may be used where physically plausible under the normal improvisation rules.

This rule applies throughout the professional/crafting Skill catalog; individual entries need not repeat "with the appropriate tools" at every degree.

### Bowyer:
> **Status:** ✅ CONFIRMED — professional/crafting progression modernized. Bowyer establishes a reusable pattern for similar professional Skills: **Maintain → Repair → Construct → Modify → Design**. Training degree unlocks capability; it does not determine the task tier or finished-item Quality.

Bowyer governs the maintenance, repair, construction, modification, and design of bows and crossbows. It does not replace related Skills such as Fletching, Carpentry, Blacksmithing/Weapon Smithing, or Engineering, although those Skills may provide **Synergy** when they materially contribute to a particular task.

- **Simple — Maintain and assemble:** String, unstring, tune, inspect, clean, and maintain bows and crossbows. Replace ordinary consumable or wear components such as strings, cords, serving, and similar parts when appropriate materials are available.
- **Basic — Repair:** Diagnose and repair ordinary damage to bows and crossbows, including damaged strings, loose fittings, warped or damaged components, cracked stocks, minor limb or prod damage, trigger issues, and similar repairable problems.
- **Intermediate — Construct:** Build complete, conventional bows and crossbows from appropriate materials and components, including the ordinary fittings and mechanisms necessary for the weapon to function. A normal weapon does not require several unrelated crafting Skills merely because it contains several materials.
- **Advanced — Modify and specialize:** Alter existing bows and crossbows for a particular user or purpose, including adjustments to draw characteristics, balance, dimensions, stock configuration, trigger behavior, reinforcement, compactness, range-oriented design, heavy-draw construction, specialized mounting, or similarly meaningful modifications. Advanced Bowyers may also reproduce established unusual or complex designs when appropriate tools and materials exist.
- **Master — Design:** Create new bow or crossbow designs rather than merely reproduce established ones. A Master Bowyer may combine unusual materials, mechanisms, dimensions, and construction principles into functional prototypes and highly specialized weapons, subject to the normal limits of the setting and materials available.

#### Capability, difficulty, and Quality

Training degree determines **what the Specialist knows how to do**. It does not automatically determine the task tier. Replacing a string may be a Simple task even though Basic Bowyer permits broader repair work, while rebuilding a badly damaged heavy crossbow might be substantially more difficult. Likewise, Intermediate Bowyer unlocks weapon construction, but the difficulty of constructing a particular weapon depends on the design, materials, tools, conditions, and circumstances.

Training degree also does not automatically determine the **Quality** of the finished item. Quality, reliability, durability, and related crafting outcomes belong to the future Crafting/Quality rules.

#### Related Skills and Synergy

Common Synergy candidates include Bowyer + Carpentry for difficult wooden components or elaborate stocks, Bowyer + Blacksmithing/Weapon Smithing for unusual metal components or reinforcement, Bowyer + Engineering for unconventional mechanical crossbow designs, and Bowyer + Fletching when tuning ammunition characteristics to a particular weapon. The actual construction of arrows or bolts remains a Fletching task.

#### Pace

Hasty and Meticulous use follow the normal Skill rules when physically meaningful. A field repair may be rushed, and careful fitting, tuning, measuring, tillering, and alignment are natural Meticulous applications. Hasty use halves actual working time; it does not turn multi-hour or multi-day construction into an instantaneous action.

### Calligraphy:
> **Status:** ✅ CONFIRMED — capability progression, professional boundaries, and common Synergy relationships locked.

Calligraphy governs **controlled, formal, and decorative written presentation**. It determines how writing is physically rendered, not what the writing says, whether the document is legally valid, or whether the finished object convincingly passes as something it is not.

- **Simple — Controlled handwriting:** Produce clear, deliberate, consistently legible handwriting in any written language the Specialist already knows. The Specialist can reproduce ordinary lettering styles and basic formal headings without the irregularity of everyday handwriting.
- **Basic — Formal scripts:** Use established formal hands, scripts, spacing conventions, margins, headings, and other structured lettering styles consistently across a document. The Specialist can produce respectable legal, academic, religious, ceremonial, or administrative-looking writing when they know the appropriate style.
- **Intermediate — Decorative and complex work:** Produce ornamental lettering, flourishes, elaborate capitals, complex layouts, tightly controlled spacing, and other advanced presentation work. The Specialist can adapt lettering cleanly to unusual sizes, shapes, surfaces, or presentation requirements.
- **Advanced — Style reproduction:** Closely reproduce an existing handwriting or calligraphic style when given a suitable example, including characteristic stroke patterns, spacing, flourishes, pressure, and layout. The Specialist can also recognize significant stylistic differences between hands that appear similar to a less-trained observer.
- **Master — Calligraphic mastery:** Design original formal scripts and lettering systems, reproduce extremely difficult hands with exceptional fidelity, and identify minute stylistic characteristics that may reveal authorship, school, period, alteration, or inconsistency in a written work when sufficient evidence exists.

Master Calligraphy remains grounded expertise. It may reveal that two passages were written by different hands, for example, but does not identify an unknown writer without evidence that would support that conclusion.

#### Boundaries with related Skills

**Calligraphy and Scribe:** Calligraphy governs physical writing style and presentation. Scribe governs recording, transcription, dictation, copying, and document reproduction at scale. Copying a lengthy manuscript accurately is primarily Scribe; preserving or producing an exact formal hand may allow Calligraphy to provide Synergy.

**Calligraphy and Writing:** Writing governs composition: choosing words, structuring prose, recounting events, and creating narratives. Calligraphy governs how those words are rendered. Expertise in one does not imply expertise in the other.

**Calligraphy and Counterfeiting:** Calligraphy can reproduce handwriting, lettering, and formal script, but does not by itself create a convincing counterfeit document. Counterfeiting governs the broader deception, including materials, seals, aging, construction, provenance, and other details. When reproducing the written hand materially contributes to a forgery, Calligraphy is a natural Supporting Skill for Counterfeiting.

Calligraphy does not grant literacy in an unknown language or specialized legal, historical, administrative, or religious understanding merely because the Specialist can reproduce its visible script. It may, however, assist in deciphering difficult handwriting or unusual scripts when that visual expertise materially contributes.

#### Pace and long-form work

Hasty and Meticulous use follow the normal Skill rules when physically meaningful. Careful ruling, spacing, layout, stroke control, and deliberate execution are natural Meticulous applications.

Lengthy manuscripts or similarly substantial projects should use the normal extended/ongoing framework rather than treating weeks of work as a single instantaneous check.

As with other professional Skills, **Training degree unlocks capability; it does not automatically determine task difficulty or finished-item Quality**.

### Carpentry:
> **Status:** ✅ CONFIRMED — capability progression, professional boundaries, and common Synergy relationships locked.

Carpentry governs functional woodworking through measuring, cutting, shaping, fitting, joining, assembling, repairing, and modifying wooden objects. It is distinct from Wood Carving, which focuses on detailed subtractive shaping and sculpture, and from Construction, which will govern erecting complete structures from plans, materials, labor, and site conditions.

- **Simple — Basic woodworking and maintenance:** Measure, mark, cut, plane, sand, bore, fasten, maintain, and perform minor repairs on wooden objects. Construct straightforward functional pieces using simple joints and fasteners, such as crates, shelves, stools, frames, handles, simple tables, doors, and similar work.
- **Basic — Conventional construction and repair:** Construct and repair ordinary furniture, cabinetry, fixtures, doors, windows, frames, chests, workbenches, partitions, and similar wooden objects. Use established joinery reliably rather than depending entirely on crude fastening.
- **Intermediate — Complex joinery and fitted work:** Produce more complicated assemblies requiring precise fit, compound joints, fitted cabinetry, stairs, curved or angled components, complex furniture, built-ins, and similar work. The Specialist can also perform substantial repairs or alterations without rebuilding the entire object.
- **Advanced — Master joinery:** Construct complex wooden objects using hidden, locking, interlocking, or self-supporting joints. Where the design and material permit, the Specialist can produce durable work with little or no nails, screws, glue, or other external fasteners. Hidden joints, sliding dovetails, pegged joinery, concealed fasteners, nested assemblies, knock-down construction, and similar techniques belong here.
- **Master — Intricate wooden mechanisms:** Create extraordinarily precise interlocking wooden constructions such as puzzle boxes, secret compartments, hidden latches, complex folding or transforming furniture, sequential locks, nested mechanisms, and similar devices whose operation comes primarily from woodworking geometry and joinery rather than machinery.

Advanced or Master Carpentry does not require avoiding fasteners when fasteners are the correct solution. The capability is the ability to solve difficult woodworking problems without them when practical, not an obligation to reject sensible materials or hardware.

#### Boundaries with related Skills

**Carpentry and Wood Carving:** Carpentry primarily governs functional construction through cutting, shaping, joining, and assembly. Wood Carving governs detailed sculptural, ornamental, and intricate subtractive shaping. A carved ceremonial chair may use Carpentry as the Primary Skill with Wood Carving providing Synergy for the ornamentation.

**Carpentry and Architecture:** Architecture governs building design, layout, and planning. Carpentry governs fabrication and assembly of wooden components. Carpentry does not grant architectural design expertise.

**Carpentry and Engineering:** Engineering governs machines, mechanisms, and mechanical systems. Carpentry may fabricate wooden gears, frames, housings, tracks, or other components from an existing design without granting understanding of the machine as a whole. A wooden puzzle box whose operation depends on joinery may be Carpentry alone; a device whose operation depends on gears, springs, cams, or other mechanical systems is Engineering territory and may use Carpentry Synergy when wooden fabrication materially contributes.

**Carpentry and Construction:** Carpentry creates and fits wooden components. Construction governs turning plans, materials, labor, and site conditions into a completed structure. Large-scale structural erection belongs to Construction, while the fabrication and joining of its wooden elements remains Carpentry.

#### Capability, difficulty, and Quality

As with other professional Skills, Training degree determines **what the Specialist knows how to do**; it does not automatically determine task difficulty or finished-item Quality. The actual job, materials, tools, conditions, and circumstances determine task tier. Quality, reliability, durability, and related crafting outcomes remain part of the future Crafting/Quality rules.

#### Pace

Hasty and Meticulous use follow the normal Skill rules when physically meaningful. Routine repairs or simple fabrication may be rushed, while precision fitting, complex joinery, hidden joints, and intricate mechanisms are natural Meticulous applications. Hasty use halves actual working time; it does not turn multi-hour or multi-day woodworking into an instantaneous action.

### Cartography:
> **Status:** ✅ CONFIRMED — capability progression, professional boundaries, and common Synergy relationships locked.

Cartography governs the interpretation, creation, analysis, and reconstruction of maps and other spatial representations. It does not automatically grant Navigation, geographic knowledge the Specialist does not possess, or Cryptography.

- **Simple — Read ordinary maps:** Interpret common maps, legends, scales, cardinal directions, marked routes, landmarks, boundaries, and ordinary symbols. The Specialist can orient a map to the surrounding terrain when enough recognizable features are available.
- **Basic — Sketch useful maps:** Create clear, functional maps from direct observation or a known route. Mark landmarks, roads, trails, buildings, hazards, approximate distances, and similar practical information accurately enough for another person to follow.
- **Intermediate — Accurate field mapping:** Produce scaled maps using measurements, bearings, elevation changes, and repeated observations. Interpret and create topographical information, map complex routes, and reconcile several observations into a coherent representation of an area.
- **Advanced — Complex surveying and map analysis:** Map difficult environments such as dense settlements, cave systems, ruins, coastlines, multi-level structures, winding waterways, or large areas where simple visual observation is insufficient. The Specialist can also identify significant inconsistencies, distortions, omissions, or errors in existing maps.
- **Master — Cartographic reconstruction and precision:** Create highly precise maps from incomplete, fragmented, historical, or conflicting information by reconciling multiple sources and physical evidence. A Master Cartographer can reconstruct likely terrain or layouts that are partly lost, changed, inaccessible, or poorly documented, and can devise new map conventions or projection methods when existing ones are inadequate.

#### Boundaries with related Skills

**Cartography and Navigation:** Cartography represents places; Navigation determines where the Specialist is and how to get somewhere. A Cartographer can create an excellent coastal chart without necessarily being able to navigate a vessel from it, while a Navigator may use a chart without being able to produce one of equal quality. Either Skill may provide Synergy to the other when both materially contribute to the task.

**Cartography and Geography:** Geography provides knowledge of regions, terrain, landforms, climate, political boundaries, resources, and similar facts. Cartography turns spatial information into a usable map. Geography may provide Synergy when that knowledge materially contributes to mapping or interpreting an area.

**Cartography and Local Geography:** Local Geography provides detailed knowledge of a particular region. It may support Cartography when mapping that region, but does not replace the technical ability to create or analyze maps.

**Cartography and Cryptography:** Cartography may use unusual symbols, legends, shorthand, or conventions, but deliberately concealing a map's meaning from unauthorized readers is **Cryptography**. Cartography and Cryptography may use Synergy when producing or interpreting an encoded map.

Cartography does not grant a supernatural sense of direction or exact positional awareness. Knowing how to read or create maps does not automatically tell the Specialist which direction is north or where they are when no usable reference information is available; those functions belong primarily to Navigation.

#### Pace and long-form work

**Hasty Cartography** is appropriate for quick sketches, rapidly recorded routes, battlefield maps, or other work where reduced time is meaningful. Use the normal Hasty rules.

**Meticulous Cartography** is appropriate for repeated measurements, careful scale work, checking bearings, reconciling observations, and producing a map intended to be dependable. Use the normal Meticulous rules.

Large surveys, extensive expeditions, or maps assembled from many observations should use the normal extended/ongoing framework rather than being resolved as a single instantaneous check.

As with other professional Skills, **Training degree unlocks capability; it does not automatically determine task difficulty or finished-item Quality**.

### Counterfeiting:
> **Status:** ✅ CONFIRMED — capability progression, authenticity boundaries, detection handling, related-Skill Synergy relationships, and pace rules locked.

Counterfeiting governs **making an object appear to be something it is not**. It may imitate appearance, markings, wear, materials, style, construction cues, provenance, and other evidence of authenticity, but it does not create properties the counterfeit does not actually possess.

- **Simple — Superficial imitation:** Create or modify a simple object so that it resembles another common object well enough for casual visual inspection. This includes straightforward replicas, imitation markings, simple tokens, labels, seals, or other uncomplicated identifiers. Close handling or informed scrutiny is likely to expose the deception.
- **Basic — Convincing ordinary facsimiles:** Alter or reproduce an ordinary object while matching multiple visible characteristics such as proportions, coloration, markings, decorative details, and general wear. The counterfeit can withstand casual handling and ordinary observation by someone who is not specifically examining it for authenticity.
- **Intermediate — Specific imitation:** Reproduce the distinguishing appearance of a **particular item, maker, organization, style, or known example** rather than merely creating a generic imitation. The Specialist can reconcile several identifying details into a consistent counterfeit when adequate references are available.
- **Advanced — Complex and scrutinized counterfeits:** Create convincing facsimiles of rare, unusual, complicated, or highly distinctive objects and deliberately account for the sorts of inconsistencies a trained observer would normally examine. Advanced Counterfeiting may combine several areas of expertise into one deception when the Specialist has access to the necessary materials and relevant Skills.
- **Master — Exceptional replication and analysis:** Reproduce unique or highly distinctive objects with extraordinary fidelity, incorporating minute visual and physical details that most observers would overlook. A Master Counterfeiter can also analyze suspected counterfeits for subtle inconsistencies in manufacture, markings, materials, wear, style, or construction.

#### Reality boundary

**Counterfeiting can imitate evidence of a property; it does not create the property itself.**

A counterfeit magical artifact may look authentic without possessing magic. A counterfeit masterwork weapon may reproduce a maker's markings and appearance without matching the real weapon's performance. A nonfunctional replica of a machine may appear convincing until its operation or internal construction is meaningfully tested.

#### Counterfeiting and the underlying craft

A Counterfeiter does not necessarily need the corresponding craft Skill when beginning with a sufficiently similar existing object and merely altering it into a convincing facsimile.

If the counterfeit must be **constructed from raw materials, function like the real item, or possess technical characteristics beyond superficial imitation**, the relevant craft or professional Skill becomes necessary.

This creates a useful Primary/Supporting distinction:

- Altering an existing necklace to resemble a famous necklace may use **Counterfeiting as Primary** with **Jeweler as Supporting** when both materially contribute.
- Manufacturing the false necklace from raw materials may use **Jeweler as Primary** with **Counterfeiting as Supporting** to reproduce the target's identifying details.

Counterfeiting grants **no broad Limited Substitution** into the crafts it may imitate. Its ability to alter a sufficiently similar base object is already its special domain.

#### Detection and authentication

When someone actively examines a suspected counterfeit, use the Skill that actually represents the relevant expertise rather than defaulting all authentication to Spot.

Common examples include:

- **Appraise** for commercial goods, valuables, art, and market authenticity.
- **Jeweler** for jewelry and worked precious materials.
- **Calligraphy** for handwriting, script, and written-style inconsistencies.
- **Heraldry** for coats of arms, seals, insignia, lineage marks, and official symbols.
- **Sewing** for garments, uniforms, and textiles.
- **Weapon Smithing** for weapons and forged makers' marks tied to construction.
- **Artistry** for artwork and decorative pieces.
- **Engineering** for mechanical devices and machinery.

**Spot** may still notice a visible inconsistency when visual perception is genuinely the relevant detection route, but informed authentication normally relies on the appropriate domain expertise.

#### Common Synergy examples

Retain the following as candidates for final rulebook margin notes, tooltips, sidebars, or worked examples:

- **Counterfeiting + Calligraphy:** forged official documents, handwriting, formal script, signatures, or written markings.
- **Counterfeiting + Scribe:** large, complex, or highly structured copied documents.
- **Counterfeiting + Jeweler:** imitation jewelry, altered precious objects, makers' marks, settings, and decorative details.
- **Counterfeiting + Sewing:** counterfeit uniforms, luxury clothing, textile labels, insignia, stitching, and construction details.
- **Counterfeiting + Artistry:** imitation paintings, sculpture finishes, decorative art, or stylistic reproduction.
- **Counterfeiting + Heraldry:** false coats of arms, seals, insignia, lineage marks, and official symbols.
- **Counterfeiting + Engineering:** convincing replicas of complex devices where mechanical appearance or internal construction materially contributes.

Counterfeiting is intentionally an **over-arching Skill with many possible Synergy relationships**. During the final full-book rough-draft edit, evaluate whether it deserves a dedicated multi-page treatment or expanded sidebar/example section so these interactions remain clear without bloating every individual Skill entry.

#### Capability, difficulty, and Quality

Training degree determines what kinds of counterfeit work the Specialist is capable of attempting; it does **not** automatically determine task difficulty. Task tier is set by the actual target, available reference material, materials, tools, access, scrutiny expected, and circumstances.

An Advanced Counterfeiter producing a batch of simple false tavern tokens may still face a Simple task. Reproducing a unique ceremonial object from incomplete reference material may be a Master task even for a Master Counterfeiter.

Finished-item Quality remains separate and will be handled by the future Crafting/Quality rules where appropriate.

#### Pace and long-form work

**Hasty Counterfeiting** is appropriate when the deception can genuinely be rushed, such as quickly altering an object to survive a cursory inspection. Use the normal Hasty rules.

**Meticulous Counterfeiting** is appropriate for careful comparison, repeated adjustment, matching minute details, controlled aging or wear, and deliberate authentication-resistant work. Use the normal Meticulous rules.

Large or complicated counterfeit projects should use the normal extended/ongoing framework rather than being resolved as a single instantaneous check.

### Disable Device:
> **Status:** ✅ CONFIRMED — capability progression, related-Skill boundaries, failure handling, and common Synergy relationships locked.

Disable Device governs **interfering with an existing mechanical device so that it stops, bypasses, delays, or changes its normal operation**. It is practical manipulation of an existing mechanism rather than general machine design.

- **Simple — Interrupt:** Identify and interfere with an accessible point of operation in a straightforward device: jam a linkage, block a gear, disconnect a line, remove an accessible component, wedge a moving part, or otherwise stop the mechanism from functioning. The intervention may be obvious or damaging. Simply smashing an object with brute force uses the normal object/combat rules rather than requiring Disable Device.
- **Basic — Disable cleanly:** Stop a straightforward device from functioning **without unnecessarily destroying it**. Disconnect, disengage, remove, lock, or otherwise neutralize working components so that the device can later be repaired or restored.
- **Intermediate — Bypass and reversible interference:** Prevent or circumvent an intended function while leaving the broader device substantially intact. Defeat a safety, interlock, trigger, governor, alarm linkage, or similar mechanism; temporarily neutralize a device; or arrange the interference so it can be reversed without rebuilding the mechanism.
- **Advanced — Selective and controlled interference:** Disable one function while allowing others to operate, manipulate a device so that it fails or resumes operation under a reasonably predictable condition, or create delayed/conditional interference using the mechanism and available components when physically plausible. This preserves the spirit of the legacy crude-timer capability without assuming every device contains a ready-made clock.
- **Master — Reconfigure function:** Alter an existing mechanism so that it behaves differently from its intended operation: reroute triggers or controls, reverse an existing action, cause one control to operate another available function, change mechanical sequencing, defeat nested safeguards, or otherwise repurpose the device's existing capabilities. Master Disable Device can **change what the existing mechanism does**, but cannot manufacture capabilities the device physically does not possess.

#### Boundaries with related Skills

**Disable Device and Engineering:** Engineering understands, designs, builds, and fundamentally modifies machines. Disable Device interferes with machines that already exist. A Specialist need not understand the full theory of a mechanism to jam, disconnect, bypass, or reroute part of it. Conversely, knowing how a machine works does not automatically grant the field manipulation needed to sabotage it quickly. **Disable Device + Engineering** is a natural Synergy pairing for unfamiliar or highly complex mechanisms.

**Disable Device and Lock Picking:** Lock Picking opens or bypasses a lock while generally preserving its intended operation. Disable Device may jam, disconnect, defeat, or sabotage a locking mechanism. If the objective is to open a lock normally and leave it usable, use Lock Picking. If the objective is to make the lock stop securing something, Disable Device may be appropriate. The two Skills may use Synergy when both materially contribute.

**Disable Device and Trap Making:** Trap Making governs designing and constructing traps. Disable Device governs neutralizing or interfering with their mechanisms. The two may use Synergy when knowledge of trap construction materially helps dismantle or bypass one.

**Disable Device and Explosives:** Disable Device may neutralize or bypass the **mechanical trigger** of an explosive device, while Explosives governs the explosive charge itself. Which Skill is Primary depends on which part is actually being manipulated. The two may use Synergy when both materially contribute.

#### Failure handling

**Failing a Disable Device check does not automatically activate the device.** Failure means the Specialist did not accomplish the intended interference. Whether the device activates, jams worse, becomes damaged, reveals the tampering, locks into place, or simply continues operating depends on the device, the circumstances, and any Critical or Overwhelming result.

Where activation is a natural consequence of a specific mistake—such as an unforgiving trigger mechanism—the Keeper may make that consequence part of the stakes, but it is not the universal result of ordinary failure.

#### Capability and difficulty

Training degree determines **what kinds of interference the Specialist knows how to perform**; it does not automatically determine task difficulty. A Master Specialist disengaging an exposed wooden latch may face a Simple task, while a Basic-trained Specialist attempting a clean disable on an unfamiliar precision device with poor access may face a substantially harder task.

#### Pace

**Hasty Disable Device** is appropriate when the procedure can genuinely be rushed, such as trying to stop a moving mechanism before it completes an action. Use the normal Hasty rules.

**Meticulous Disable Device** is appropriate for careful disassembly, controlled testing, tracing linkages, and reversible sabotage. Use the normal Meticulous rules.

Large or complicated sabotage jobs should use the normal extended/ongoing framework rather than being resolved as a single instantaneous check.

Disable Device grants **no broad Limited Substitution** into Engineering, Lock Picking, Trap Making, or Explosives.

### Escape:
> **Status:** ✅ CONFIRMED — capability progression, restraint/confinement boundaries, physical-limit boundary, and common Synergy relationships locked.

Escape governs getting free from **restraints, confinement, and entanglement once they exist**. It does not replace the Combat/Martial rules used to escape an opponent's active grapple or hold.

- **Simple — Find the weakness:** Recognize and exploit obvious slack, poor fastening, loose knots, bad positioning, or other weaknesses in simple restraints. Escape loosely or poorly applied bindings, sacks, crude ties, simple entanglements, and similar restraints when physically possible.
- **Basic — Work free of secure flexible restraints:** Escape properly applied ropes, straps, bindings, nets, tied clothing, and similar flexible restraints by manipulating tension, shifting knots, compressing the body, creating slack, and using leverage.
- **Intermediate — Slip rigid restraints:** Escape rigid restraints such as manacles, shackles, stocks, cuffs, collars, or similar devices **when their physical construction permits escape without actually opening the lock**. This can involve exploiting fit, joint position, tolerances, leverage, body compression, or mechanical play.
- **Advanced — Complex and layered restraint:** Escape multiple or deliberately redundant restraints: bound hands and feet, body harnesses, tightly secured nets, restrictive garments, combined rope-and-shackle arrangements, awkward suspension, confined positions, or other systems specifically intended to eliminate ordinary escape methods. Advanced Training also permits effective work from extremely unfavorable positions when enough movement remains physically possible.
- **Master — Escape artistry:** Exploit extremely small tolerances and deliberately prepare for escape while restraints are being applied: subtly alter body position, control breathing or muscle tension, preserve hidden slack, position a limb advantageously, conceal a small escape aid, or identify an escape sequence through several different restraints. A Master may also squeeze through exceptionally tight openings when their anatomy can **actually fit**.

#### Physical-limit boundary

Escape never allows a Specialist to pass through an opening their body cannot physically fit through, ignore solid restraints with no exploitable movement, or dislocate joints without whatever injury consequences such an act would normally carry.

#### Escape and active grappling

**Escape governs restraints and confinement. Active control by another creature is resolved using the applicable Combat/Martial rules.** A future Martial Component may explicitly interact with Escape, but Escape does not universally replace grapple-breaking mechanics.

#### Escape and Lock Picking

Escape asks whether the Specialist can get free **without opening the locking mechanism**. Lock Picking asks whether the Specialist can defeat the lock itself. If a restraint must actually be unlocked, Lock Picking is the relevant Skill. The two may use Synergy when both materially contribute, such as working a concealed pick while restrained in an awkward position.

#### Prepared restraints and opposed use

When a Specialist deliberately prepares for escape while being restrained, such as preserving slack or positioning their body advantageously, the Keeper may resolve an opposed check against the Skill actually being used to apply the restraint, such as Rope Use or another appropriate Skill. This can create an escape opportunity without granting automatic immunity to restraints.

#### Pace and extended use

**Hasty Escape** is appropriate when the attempt can genuinely be rushed, representing a desperate effort to get free quickly. Use the normal Hasty rules.

**Meticulous Escape** is appropriate when the Specialist can stop struggling, study the restraint, test tension, and work free one small step at a time. Use the normal Meticulous rules.

Difficult escapes involving multiple restraints or several stages are natural candidates for the extended/ongoing framework.

Escape grants **no general Limited Substitution** into Lock Picking, Rope Use, Sleight of Hand, Acrobatics, or Combat/Martial grappling.

### Fletching:
> **Status:** ✅ CONFIRMED — professional progression, ammunition/weapon boundary, payload boundary, and common Synergy relationships locked.

Fletching governs the maintenance, construction, tuning, and design of arrows, bolts, darts, and similar shafted projectile ammunition. It governs the projectile rather than the weapon that launches it.

- **Simple — Maintain and repair ammunition:** Inspect, straighten, clean, rebalance, refletch, renock, and perform ordinary maintenance or minor repairs on arrows, bolts, darts, and similar shafted projectile ammunition. Replace damaged components when suitable replacements are available.
- **Basic — Assemble standard ammunition:** Construct ordinary arrows, bolts, darts, and similar ammunition from prepared components such as shafts, heads, nocks, and fletching. Produce consistent batches intended for normal use.
- **Intermediate — Fabricate and fit components:** Create and properly fit the non-specialized components of projectile ammunition from appropriate raw materials: shape shafts, cut nocks, prepare feathers or equivalent fletching, fit available heads, balance the projectile, and produce complete ammunition without relying on pre-made parts. This does not grant unrelated metalworking or other craft expertise required to manufacture specialized components from raw materials.
- **Advanced — Tune and specialize:** Tailor ammunition for a particular weapon, user, range, trajectory, target, or purpose. Control characteristics such as shaft stiffness, total weight, balance point, fletching size and configuration, head weight, aerodynamic stability, and consistency across a matched set. Conventional specialized ammunition such as heavy hunting arrows, long-range flight arrows, broadheads, bodkin-style ammunition, low-drag bolts, and highly stable short-range ammunition belongs here when the necessary components and materials exist.
- **Master — Design specialized ammunition:** Design new ammunition configurations and safely integrate unusual payloads, mechanisms, or delivery systems into arrows, bolts, darts, and similar projectiles.

#### Weapon and payload boundaries

**Bowyer governs the weapon; Fletching governs the ammunition.** A Bowyer may tune a bow or crossbow, while a Fletcher may tune ammunition to that weapon. When both materially contribute to a matched weapon-and-ammunition system, the Skills may use Synergy.

**Fletching can build the projectile and its delivery interface; it does not create the payload.** A Master Fletcher may design an arrow or bolt that safely carries a poison vial, incendiary mixture, explosive charge, alchemical payload, spell-bearing component, line, signal device, or similar attachment, but the payload itself requires the relevant Skill or other rules source.

Common Synergy pairings include:

- **Fletching + Bowyer:** deliberately tune ammunition characteristics to a particular bow or crossbow.
- **Fletching + Weapon Smithing:** specialized metal heads or unusual ammunition hardware.
- **Fletching + Poisons:** ammunition intended to retain and deliver a toxin effectively.
- **Fletching + Explosives:** projectile construction that safely carries and survives launch with an explosive payload.
- **Fletching + Alchemy/Apothecary:** ammunition used to carry and deliver chemical, medicinal, or alchemical payloads.
- **Fletching + Hunting:** situationally appropriate when prey knowledge materially affects the ammunition being designed for a particular hunt.

Fletching grants no broad Limited Substitution into these related Skills.

#### Capability, difficulty, and Quality

Training degree determines what the Specialist knows how to make or modify; it does not automatically determine task tier or finished-item Quality. A Master Fletcher replacing one damaged feather may still be performing a Simple task. The actual ammunition, materials, tools, precision required, and circumstances determine difficulty.

#### Pace

Hasty and Meticulous use follow the normal Skill rules when physically meaningful. Field repairs may be rushed, while matched sets, precision balancing, aerodynamic tuning, and specialized payload integration are natural Meticulous applications. Large batches or complicated ammunition projects should use the normal extended/ongoing framework.

### Herbology:
> **Status:** ✅ CONFIRMED — botanical identification, analysis progression, professional boundaries, and common Synergy relationships locked.

Herbology governs the identification, collection, comparison, and practical understanding of plants and plant-derived materials. It tells the Specialist what a plant is, what portions are relevant, what ordinary properties it possesses, and how environmental or seasonal factors affect it. Herbology does not itself turn those properties into medicines, poisons, alchemical preparations, or magical effects.

- **Simple — Familiar plants:** Recognize common plants from regions and environments the Specialist knows well. Identify familiar edible, irritating, poisonous, useful, or otherwise noteworthy plants and distinguish healthy specimens from obviously diseased, spoiled, or unsuitable ones.
- **Basic — Unfamiliar identification:** Examine unfamiliar plants using visible structure, habitat, growth pattern, scent, texture, and other ordinary evidence to determine likely family, uses, hazards, and close look-alikes. Ordinary identification does not require recklessly ingesting an unknown specimen.
- **Intermediate — Functional properties:** Determine which portions of a plant contain relevant mundane properties, when those properties are strongest or weakest, how maturity and season affect them, and how to collect and preserve useful specimens without unnecessarily ruining them. Controlled experimentation may be used where observation alone is insufficient.
- **Advanced — Comparative botanical analysis:** Infer likely properties of rare or unfamiliar plants by comparison with related species, habitat, growth behavior, and physical evidence. Detect subtle contamination, adulteration, disease, abnormal growth, or misleading resemblance between species and determine how environmental conditions have altered a specimen.
- **Master — Botanical expertise:** Identify and analyze exceptionally rare, altered, poorly preserved, or previously unfamiliar plants from limited but meaningful evidence. A Master Herbologist can establish a reliable classification, distinguish extremely similar species, and determine likely mundane properties with very little material when those conclusions are physically supportable.

#### Boundaries and Synergy

**Herbology** determines what a plant is and what properties it naturally has. **Apothecary** formulates mundane remedies, salves, tonics, and similar preparations. **Poisons** handles toxic substances as toxicological agents. **Alchemy** handles alchemical or magical-seeming transformations. **Farming** governs cultivation at agricultural scale.

Common Synergies include **Herbology + Geography** when habitat materially aids identification, **Herbology + Farming** when diagnosing cultivated plants, **Apothecary + Herbology** for plant-based preparations, **Poisons + Herbology** for plant toxins, and **Alchemy + Herbology** for unusual plant ingredients.

Herbology grants no Limited Substitution into those related Skills. Recognizing a useful property does not automatically grant the ability to formulate it.

#### Capability, difficulty, and pace

Training degree determines what kinds of botanical analysis are possible; the specimen, evidence, environment, condition, tools, and circumstances determine task tier.

Hasty Herbology is appropriate for rapid field identification. Meticulous Herbology is appropriate for careful comparison, dissection, repeated observation, or controlled experimentation. Large surveys and cataloguing projects should use the normal extended/ongoing framework.

Exact medicinal, toxic, alchemical, and supernatural effects remain governed by their respective subsystems.

### Jeweler:
> **Status:** ✅ CONFIRMED — professional progression, material/craft boundaries, and common Synergy relationships locked.

Jeweler governs the fabrication, repair, setting, shaping, and fine decorative working of jewelry, gemstones, and precious-metal adornments, using the appropriate tools, materials, and workspace required by the professional Skill rules.

- **Simple — Basic precious-metal work:** Shape, bend, cut, polish, size, clean, and repair straightforward jewelry made from suitable malleable materials. Produce simple rings, bands, bracelets, hooks, clasps, and comparable adornments.
- **Basic — Conventional jewelry construction:** Construct ordinary necklaces, chains, earrings, brooches, pendants, linked pieces, settings, fasteners, and multi-component jewelry using established designs. Identify obvious workmanship problems and common jewelry-construction techniques.
- **Intermediate — Stone setting and precision assembly:** Secure cut stones into appropriate settings, construct delicate multi-part pieces, perform precise joining where the material and design permit it, replace damaged settings, and work to close tolerances without unnecessarily damaging valuable materials.
- **Advanced — Lapidary and fine decorative work:** Cut, shape, facet, polish, and prepare suitable raw gems for use in jewelry. Create filigree, fine engraving, embossing, delicate surface work, complex settings, and other high-precision decorative elements.
- **Master — Complex jewelry design:** Design and construct exceptionally intricate jewelry combining advanced settings, fine precious-metal work, multiple materials, unusual geometries, movable decorative elements, and highly demanding fabrication techniques. A Master Jeweler may reproduce or restore extraordinarily complex jewelry when sufficient reference material exists.

#### Boundaries and Synergy

**Metallurgy** governs metal composition, refining, and alloys. Jeweler works prepared precious metals without automatically knowing how to refine ore or formulate alloys.

**Appraise** governs monetary or market value. Jeweler can identify materials and workmanship relevant to jewelry, but does not automatically know what a particular piece will sell for.

**Counterfeiting** creates deceptive authenticity; Jeweler creates the jewelry itself. **Engineering** governs true mechanical systems beyond ordinary hinges, clasps, and jewelry fittings.

Common Synergies include **Jeweler + Metallurgy**, **Jeweler + Appraise**, **Jeweler + Counterfeiting**, **Jeweler + Artistry**, and **Jeweler + Engineering** where both fields materially contribute.

Jeweler grants no Limited Substitution into those Skills.

#### Capability, difficulty, Quality, and pace

Training degree determines fabrication capability, not task tier, market value, or finished-item Quality. A Master repairing an ordinary loose clasp may still face a Simple task.

Hasty use is possible for repairs and rough fitting where rushing is physically plausible. Precision setting, gem cutting, filigree, and complex fabrication are natural Meticulous applications. Significant pieces may use extended checks.

Finished-item Quality, durability, and material-value effects remain part of the future Crafting/Quality rules.

### Leatherworking:
> **Status:** ✅ CONFIRMED — non-armor leathercraft progression, material boundaries, and common Synergy relationships locked. Leather Armoring remains separate pending the Toughness pass.

Leatherworking governs preparing hides and constructing, shaping, repairing, decorating, and fitting **non-armor leather goods** with the appropriate tools, materials, and workspace.

- **Simple — Hide handling and basic repair:** Remove a usable hide or skin from a creature when circumstances permit, clean and preserve it well enough for later processing, cut prepared leather, punch holes, stitch simple seams, and perform minor repairs on ordinary leather goods.
- **Basic — Conventional leather goods:** Construct straightforward belts, pouches, straps, sheaths, simple footwear, gloves, bags, basic garments, covers, and similar items from prepared leather using established patterns.
- **Intermediate — Shaping and fitted construction:** Wet-form, mold, stretch, fit, reinforce, edge, line, and assemble leather into comfortable or closely fitted garments and more complex goods. Produce durable fitted boots, fitted clothing, shaped cases, harness components, and comparable work.
- **Advanced — Refinement and complex leathercraft:** Refine, soften, dye, finish, tool, emboss, layer, and combine leather for demanding applications. Construct complex saddles, fitted harness, heavy-duty packs, articulated non-armor goods, elaborate clothing, and other objects where shaping and load distribution matter.
- **Master — Advanced leather fabrication:** Design and create highly complex leather constructions combining shaping, reinforcement, multiple leather weights, precise fitting, decoration, and unusual forms. Given appropriate material, a Master Leatherworker can fabricate nearly any object whose defining construction is genuinely leatherwork rather than armor, machinery, or another specialist craft.

#### Boundaries and Synergy

**Leather Armoring** currently owns armor whose protective construction depends primarily on leather. Leatherworking may prepare decorative elements, straps, liners, fittings, or raw leather but does not substitute for armor construction.

**Sewing** governs cloth and textile construction; Leatherworking governs hide and leather. Mixed-material goods may use Synergy.

Common Synergies include **Leatherworking + Sewing**, **Leather Armoring + Leatherworking**, **Leatherworking + Animal Husbandry** for specialized tack, **Counterfeiting + Leatherworking**, and **Leatherworking + Artistry** for elaborate tooling or decorative work.

Leatherworking grants no Limited Substitution into Leather Armoring or Sewing.

A sail genuinely made from leather or hide may use Leatherworking; ordinary textile sails belong to Sewing.

#### Capability, difficulty, Quality, and pace

Training degree determines what the Specialist can fabricate, not automatic task tier or Quality. Repairs may be Hasty. Fitted, molded, tooled, or large projects strongly support Meticulous and extended work.

Tanning/refining times, object durability, armor interactions, and Quality remain Crafting-system dependencies.

### Lock Picking:
> **Status:** ✅ CONFIRMED — capability progression, generic lock difficulty ladder, magic boundary, and related-Skill Synergy locked.

Lock Picking governs defeating a lock's intended securing function through manipulation of the lock itself while generally preserving its ability to function afterward. It assumes appropriate picking tools unless the Specialist is using a physically plausible improvised substitute.

- **Simple — Conventional locks with proper tools:** Manipulate straightforward familiar locks when the mechanism is accessible and functioning normally.
- **Basic — Varied conventional mechanisms:** Work with a broader range of ordinary lock constructions, recognize common internal behaviors from feedback, and cope with modest wear, awkward placement, or unfamiliar but conventional designs.
- **Intermediate — Difficult access and complex locks:** Pick locks requiring precise manipulation, operate from poor angles or limited visibility, work around multiple locking elements, and diagnose whether a failed attempt is caused by the lock, keyway, damage, or another obstruction.
- **Advanced — High-security and unusual mechanical locks:** Defeat sophisticated purely mechanical locks incorporating multiple stages, deceptive feedback, unusual internal geometry, nested mechanisms, or deliberate anti-tampering features when a manipulable route exists.
- **Master — Improvised and exotic mechanical entry:** Attempt extremely unfamiliar or exceptional mechanical locks and fabricate or adapt makeshift picking tools from plausible available materials when proper tools are unavailable. A Master can reason through an unknown lock's behavior while manipulating it, but still requires a physically exploitable mechanism.

#### Generic lock difficulty

When a lock has no individually defined construction difficulty, use this ladder as the default ballpark:

| Lock tier | Generic example |
| --- | --- |
| **Simple** | Crude or straightforward mechanical lock with loose tolerances, an uncomplicated mechanism, and little deliberate resistance to picking. |
| **Basic** | Ordinary competent lock used on doors, chests, gates, cabinets, and similar everyday secured objects. |
| **Intermediate** | Well-made lock with tighter tolerances, multiple working elements, or modest anti-manipulation features. |
| **Advanced** | High-security mechanical lock deliberately designed to resist picking through complex interaction, misleading feedback, multiple stages, or anti-tampering features. |
| **Master** | Exceptional bespoke lock employing unusually precise, novel, nested, or highly sophisticated mechanical security. |

These are defaults, not immutable categories. Access, condition, damage, tools, environment, unusual construction, and similar circumstances may alter the actual task tier.

**Player-made and specifically crafted locks will use the difficulty established by their construction rules once the Crafting system is finalized.**

#### Magical locks

Lock Picking can manipulate the **physical components** of a magical lock when those components remain physically accessible and manipulable. Mundane Lock Picking does **not** dispel, negate, or bypass a purely magical locking effect.

Magical lock picks or other specialized equipment may later grant additional capability against magical locks. Any such capability belongs to the **tool or magical item**, not to the mundane Skill itself.

#### Boundaries and Synergy

**Disable Device** jams, disconnects, sabotages, or mechanically interferes with a lock. **Lock Picking** defeats the lock through its locking mechanism while normally leaving it usable.

**Engineering** may explain an exotic mechanism; Lock Picking provides the manipulation expertise to defeat it.

Common Synergies include **Lock Picking + Engineering**, **Lock Picking + Disable Device**, **Lock Picking + Escape** when manipulating restraints from an awkward position, and **Lock Picking + Sleight of Hand** when the manipulation itself must remain concealed.

Lock Picking grants no Limited Substitution into those Skills.

#### Capability, difficulty, and pace

Training degree determines what kinds of lock manipulation the Specialist understands; the specific lock and circumstances determine task tier.

Hasty picking is possible under genuine time pressure. Meticulous picking represents patient feedback, repeated testing, and careful manipulation.

### Musical Instrument (Specified):
> **Status:** ✅ CONFIRMED — specified-instrument progression, related-instrument Limited Substitution, and performance boundaries locked.

Musical Instrument (Specified) governs technical performance, interpretation, arrangement, improvisation, and composition using one chosen instrument. Appropriate access to the instrument and any ordinary playing tools or accessories is assumed.

- **Simple — Basic control:** Produce intentional notes, tones, rhythms, or simple chords appropriate to the instrument; tune or prepare it for ordinary use where that is part of normal playing technique; and perform very simple musical passages.
- **Basic — Prepared performance:** Play complete straightforward pieces from notation, tablature, memorized instruction, or rehearsal with dependable timing and recognizable accuracy.
- **Intermediate — Fluent performance:** Perform complete pieces without requiring constant reference material, maintain rhythm and phrasing through ordinary variation, accompany other performers, recover from minor performance errors, and adapt tempo or dynamics to a group.
- **Advanced — Arrangement and improvisation:** Improvise coherently within an established musical form, rearrange existing pieces for the specified instrument, compose functional original music for it, and adapt a performance to changing accompaniment or audience circumstances.
- **Master — Instrumental mastery:** Perform technically exceptional material, improvise extended original passages, compose sophisticated works exploiting the instrument's capabilities, adapt pieces substantially during performance, and maintain musical coherence through difficult or unexpected changes.

#### Related-instrument Limited Substitution

Training in a specified instrument grants reduced competency with **closely related instruments that use substantially similar playing techniques**, at **one degree lower** than the Specialist's actual Training.

- Simple Training provides no related-instrument Training.
- Basic provides Simple.
- Intermediate provides Basic.
- Advanced provides Intermediate.
- Master provides Advanced.

This is an explicit exception to the normal default for Limited Substitution.

"Related" is based on meaningful technical transfer, not merely broad family labels. A guitar may transfer substantially to a similar fretted plucked string instrument; a violin may transfer substantially to a viola. Guitar does not automatically substitute for violin merely because both use strings. The Keeper adjudicates unusual cases from the actual playing technique.

Actual Training in the related instrument always supersedes the substitution.

#### Boundaries and Synergy

**Singing** governs the voice. **Writing** governs words and prose, including lyrics. **Artistry** remains a visual-art Skill rather than a universal creativity Skill. Social Skills govern attempts to influence an audience beyond the quality of the performance itself.

Common Synergies include **Musical Instrument + Singing**, **Musical Instrument + Writing**, **Musical Instrument + Acting**, and **Musical Instrument + Wood Carving** where construction or modification of a wooden instrument materially benefits from knowledge of how it is played.

#### Capability, difficulty, and pace

Training degree determines musical capability, not the intrinsic difficulty of every composition. A Master performing a beginner exercise may still face a Simple task.

Hasty and Meticulous primarily apply to composition, arrangement, rehearsal, tuning, preparation, or other tasks with a meaningful time interval. A fast musical tempo is not automatically Hasty. Long compositions and rehearsals may use extended checks.

### Poisons:
> **Status:** ✅ CONFIRMED — toxicology progression, professional boundaries, and Synergy relationships locked. Poison resistance is preserved as a future mutually exclusive Trait or Conditioning progression rather than an automatic benefit of ordinary Skill degree.

Poisons governs the safe handling, harvesting, preservation, preparation, analysis, application, and refinement of toxic substances as toxic agents. Appropriate protective equipment, tools, materials, and workspace are assumed where reasonably required.

- **Simple — Handle and apply known poisons:** Recognize the handling requirements of familiar prepared toxins, store and transport them appropriately, avoid ordinary accidental exposure, and apply a prepared poison to an appropriate delivery medium when physically possible.
- **Basic — Harvest and preserve known toxins:** Safely recover and preserve known toxic material from an identified source using established procedures. Maintain usable prepared poisons and recognize obvious degradation, contamination, or unsafe handling.
- **Intermediate — Analyze and adapt toxins:** Compare known toxic substances, identify likely delivery routes and general effects from evidence, prepare harvested material into a stable usable form according to known methods, and adapt an existing poison for a different legitimate delivery medium when the substance itself supports it.
- **Advanced — Complex toxicology:** Work safely with rare, dangerous, mixed, or difficult toxins; diagnose subtle contamination or degradation; separate useful toxic material from interfering substances using established techniques; and formulate sophisticated preparations from known toxic components without automatically increasing their mechanical potency beyond what the poison rules permit.
- **Master — Toxicological mastery:** Analyze exceptionally rare or unfamiliar poisons from limited evidence, develop new preparations from known toxic substances, determine how multiple toxic agents are likely to interact under the game rules, and refine complex poisons to the limits permitted by the eventual Poison/Crafting subsystem.

#### Boundaries and Synergy

**Herbology** identifies toxic plants and their natural properties. **Poisons** turns toxic material into a toxicological tool.

**Apothecary** handles general mundane remedies, tonics, salves, medicines, and related preparations. Its legacy toxin overlap will be reconciled during the Intelligence pass so that specialized toxicology remains the defining job of Poisons.

**Chemistry** governs general chemical understanding. **Alchemy** governs alchemical or magical-seeming transformations.

Common Synergies include **Poisons + Herbology**, **Poisons + Apothecary**, **Poisons + Chemistry**, **Poisons + Alchemy**, **Poisons + Fletching**, and **Poisons + First Aid** when symptoms or treatment materially contribute.

Poisons grants no Limited Substitution into those related Skills.

#### Poison resistance

The legacy concept of deliberately conditioning the body against toxins is preserved, but **ordinary Poisons Training does not automatically grant physiological resistance**.

Poison resistance may later be represented by either:

- an appropriate **Trait**, or
- a separate **Poison Conditioning Training progression** enabled by deliberate training and exposure.

Those two sources are **mutually exclusive and do not stack**.

The exact benefits, risks, exposure requirements, toxin categories, breadth of resistance, and advancement rules will be finalized with the Poison, Trait, and Conditioning systems.

#### Capability, difficulty, and pace

Task tier depends on toxicity, rarity, stability, contamination, tools, source material, and required preparation. Higher Training does not automatically create a stronger poison.

Hasty use may be possible for rapid application or emergency handling. Meticulous use suits analysis, extraction, refinement, and careful preparation. Production of meaningful quantities naturally supports extended checks.

### Rope Use:
> **Status:** ✅ CONFIRMED — rigging progression, boundaries, and common Synergy relationships locked.

Rope Use governs knots, lashings, rope handling, rigging, load control, line placement, and systems whose primary working element is rope or cordage.

- **Simple — Routine rope handling:** Coil, uncoil, store, untangle, and perform simple joining or splicing where appropriate. Tie dependable everyday knots for securing ordinary objects, bundles, lines, and loads.
- **Basic — Functional knots and basic rigging:** Select and tie knots appropriate to tension, attachment, joining, release, or load securing; create simple lashings; rig ordinary lines for hauling or rappelling; and construct straightforward pulley arrangements using available hardware.
- **Intermediate — Load-bearing and climbing rigging:** Construct reliable anchor systems, tensioned lines, hauling arrangements, climbing or rappelling systems, rescue lines, and multi-rope lashings while accounting for direction of load and practical rope behavior.
- **Advanced — Dynamic and specialized rope work:** Build complex tensioned systems, use ropes to capture or control moving objects where physically plausible, throw and place lines accurately, construct lassos and similar loop systems, and rig difficult loads or awkward environments without relying on trial and error.
- **Master — Complex rigging and cordage systems:** Design and construct sophisticated rope networks, nets, multi-point lifting or hauling systems, rescue rigs, suspended assemblies, and other complex structures whose function depends principally on rope geometry, tension, knots, and available anchors.

#### Boundaries and Synergy

**Climbing** governs moving the body across difficult surfaces. Rope Use creates and manages rope systems that may make climbing safer or possible.

**Engineering** owns machines and mechanical systems. Straightforward rope-and-pulley arrangements remain Rope Use; mechanical cranes, winches, gearboxes, and engineered lifting machines belong primarily to Engineering.

**Trap Making** constructs traps; Rope Use may construct their rope components. **Escape** defeats restraints; Rope Use may create or apply them.

Common Synergies include **Rope Use + Climbing**, **Rope Use + Escape**, **Escape + Rope Use**, **Rope Use + Engineering**, **Trap Making + Rope Use**, and vessel rigging applications where another relevant boating or sailing Skill materially contributes.

Rope Use grants no Limited Substitution into Climbing, Engineering, Trap Making, or Escape.

#### Capability, difficulty, and pace

Training determines what rope systems the Specialist can construct. Load, available anchors, line condition, tools, environment, and consequences determine task tier.

Hasty use works for hurried knots or emergency rigging. Meticulous use is natural for load-bearing, rescue, climbing, and complex systems. Large nets and elaborate rigs use extended checks.

Exact load limits remain dependent on material, object, and carrying/exertion rules.

### Scribe:
> **Status:** ✅ CONFIRMED — recording/transcription progression, unknown-language copying rule, document boundaries, and common Synergy relationships locked.

Scribe governs accurate recording, transcription, copying, collation, and reproduction of written information. It preserves what was said or written rather than composing the content or controlling the beauty of the handwriting.

- **Simple — Notes and short copies:** Record short statements, names, lists, events, instructions, and other straightforward information legibly enough to be used later. Copy short written passages without materially changing their meaning.
- **Basic — Sustained records:** Keep orderly records over extended periods, copy ordinary documents reliably, maintain logs and ledgers, and organize written material so another reader can follow it.
- **Intermediate — Accurate dictation and transcription:** Record speech accurately as it occurs at a practical pace, reconcile obvious repetitions or corrections without losing meaning, and transcribe lengthy material from a source while maintaining consistent organization.
- **Advanced — Long-form copying and collation:** Copy substantial books, records, tables, diagrams, and structured documents with high fidelity; compare multiple copies to locate textual discrepancies; organize indexes or cross-references; and reproduce material between languages the Specialist already knows when permitted by the language rules.
- **Master — Facsimile document reproduction:** Produce exceptionally exact textual and layout reproductions of writings, diagrams, tables, marginal notation, and complex document structures; collate damaged or conflicting copies to reconstruct the most likely complete text; and detect minute transcription discrepancies across versions.

#### Unknown-language transcription

A Scribe may copy or transcribe writing in a language they do **not** understand by treating the characters as visual information rather than meaningful language.

Doing so normally carries **significantly increased task difficulty** because the Specialist cannot use comprehension, grammar, context, familiar vocabulary, or expected wording to notice and correct transcription errors.

This does not grant translation, literacy, or understanding of the copied language.

#### Boundaries and Synergy

**Calligraphy** controls writing style and decorative presentation. **Scribe** preserves content and structure. **Writing** composes new prose. **Counterfeiting** creates deceptive authenticity.

The legacy Master ability to make exact duplicates survives within those boundaries: Scribe can reproduce content and layout; distinctive handwriting may call for Calligraphy, and making the copy falsely pass as the original belongs to Counterfeiting.

Common Synergies include **Scribe + Calligraphy**, **Scribe + Counterfeiting**, **Scribe + Writing**, **Scribe + Researching**, and **Scribe + Administration**.

Scribe grants no Limited Substitution into those Skills.

#### Capability, difficulty, and pace

Length is usually a matter of time rather than automatic task-tier escalation. Difficulty comes from source quality, complexity, damage, speed, formatting, unfamiliar notation, language comprehension, and similar factors.

Hasty Scribe covers rapid notes or emergency transcription. Meticulous use covers exact copying and collation. Large manuscripts are natural extended tasks.

### Sewing:
> **Status:** ✅ CONFIRMED — textile construction progression, material boundaries, and common Synergy relationships locked.

Sewing governs the construction, alteration, repair, fitting, and fabrication of cloth and flexible textile goods, including creation of fabric where weaving is part of the intended craft scope.

- **Simple — Stitch, mend, and basic textile work:** Sew dependable simple seams, patch tears, replace basic closures, hem cloth, perform routine garment repairs, and weave or assemble simple coarse textile when appropriate tools and materials are available.
- **Basic — Conventional garments and goods:** Read or use established patterns, cut fabric efficiently, construct ordinary clothing, bags, covers, simple curtains, blankets, and similar textile goods, and produce ordinary woven fabric using suitable equipment.
- **Intermediate — Fitting and pattern design:** Alter clothing to fit particular bodies, draft and modify patterns, construct fitted garments, create reinforced seams and structured textile pieces, line garments, and produce practical specialized textile goods such as tents, ordinary sails, padded pieces, and similar work.
- **Advanced — Fine materials and complex tailoring:** Work reliably with delicate, expensive, difficult, or unusually structured fabrics; construct elaborate fitted clothing, formal garments, layered textile work, complex draping, detailed decorative stitching, and high-precision tailoring.
- **Master — Advanced textile design:** Design and construct exceptionally complex garments and textile structures combining advanced patterning, fine weaving, difficult fabrics, intricate fitted construction, reinforcement, layering, and elaborate presentation. A Master Sewer can develop new garment patterns and textile constructions rather than merely reproduce established ones.

#### Boundaries and Synergy

**Leatherworking** governs hide and leather; Sewing governs cloth and flexible textile. Armor whose protection comes from a dedicated armor-construction technique belongs to the appropriate Armoring Skill rather than automatically to Sewing.

**Counterfeiting** may reproduce the appearance and identifiers of a garment; Sewing constructs the garment itself.

Common Synergies include **Sewing + Leatherworking**, **Sewing + Counterfeiting**, **Sewing + Artistry**, **Sewing + Calligraphy** for stitched formal lettering when appropriate, and **Sewing + Rope Use** for sails, tents, awnings, nets, or other large textile structures whose rigging materially contributes.

Sewing grants no Limited Substitution into Leatherworking or Armoring.

A textile sail belongs to Sewing; a leather or hide sail belongs to Leatherworking.

#### Capability, difficulty, Quality, and pace

Training unlocks types of textile construction; it does not dictate finished-item Quality. A Master repairing an ordinary hem may still be doing a Simple task.

Hasty use is appropriate for emergency repairs or crude temporary seams. Meticulous use suits fitting, fine fabric, pattern work, formal garments, and large textile assemblies. Large projects use extended checks.

Textile durability, armor protection, material costs, and Quality remain Crafting dependencies.

### Sleight of Hand:
> **Status:** ✅ CONFIRMED — manual-deception progression, physical plausibility boundary, opposed use, Pick Pocket boundary, and Synergy relationships locked.

Sleight of Hand governs covert manual manipulation, palming, concealment, switches, false transfers, reveals, and misdirection involving objects already under the Specialist's control. Pick Pocket governs covertly taking from or planting on another creature.

- **Simple — Palm and conceal small objects:** Conceal, retain, or manipulate a hand-sized or smaller object in the hand or immediately accessible clothing when there is a plausible place to hide it.
- **Basic — Covert transfers and retrieval:** Secretly move small objects between hands, pockets, sleeves, containers, or other nearby concealment points while keeping the manipulation from casual observers. Perform basic false transfers and controlled reveals.
- **Intermediate — Misdirection sequences:** Coordinate hand movement, timing, gaze, posture, and ordinary misdirection to switch, conceal, produce, or apparently transform handheld objects during a sequence rather than a single motion.
- **Advanced — Complex object manipulation:** Conceal, switch, reveal, or reposition larger or more awkward objects when clothing, props, surfaces, containers, assistants, or environmental concealment make the action physically plausible. Manage multiple objects or concealment locations without obviously exposing the method.
- **Master — Extended deceptive manipulation:** Perform sophisticated multi-stage routines involving several objects, repeated switches, layered concealment, false transfers, and coordinated misdirection while adapting to observers and changing circumstances. Mastery allows exceptional subtlety, not physically impossible disappearance.

#### Physical boundary

**Sleight of Hand never makes an object cease to exist.** There must be a physically plausible place for the object to go and a plausible means of getting it there.

The legacy progression toward hiding larger objects survives only where props, clothing, scenery, containers, assistants, or another genuine concealment method makes the action possible.

#### Boundaries, opposed use, and Synergy

**Pick Pocket** transfers an object to or from another creature without their knowledge. **Sleight of Hand** manipulates and conceals objects through manual dexterity and misdirection. **Smuggling** hides and transports contraband through security or across an area. **Escape** gets the Specialist out of restraint.

Sleight of Hand is normally opposed by **Spot** when an observer could detect the manipulation visually. Another sense may apply where appropriate. Failure does not automatically mean the observer understands the entire method.

Common Synergies include **Pick Pocket Primary + Sleight of Hand Supporting**, **Sleight of Hand + Acting**, **Sleight of Hand + Bluff**, **Sleight of Hand + Escape**, and **Lock Picking + Sleight of Hand** where concealed manipulation materially matters.

Sleight of Hand grants no Limited Substitution into those Skills.

#### Capability, difficulty, and pace

Object size is only one difficulty factor. Observer attention, concealment available, number of objects, movement required, lighting, clothing, preparation, and circumstances also matter.

Hasty use works for a hurried switch or concealment. Meticulous use can apply to preparation or waiting for an ideal moment, but an instantaneous live manipulation does not become Meticulous merely because the performer is skilled.

In combat, ordinary active use costs 1 AP and does not replace Disarm or Pick Pocket rules for defended objects.

### Trap Making:
> **Status:** ✅ CONFIRMED — trap-construction progression, related-Skill boundaries, and integration limits locked.

Trap Making governs designing, constructing, assembling, arming, repairing, and modifying traps and their trigger systems. It does not automatically grant the ability to place a trap effectively against particular prey, create every possible payload, or neutralize an existing trap.

- **Simple — Basic traps:** Construct straightforward traps using simple triggers, gravity, tension, snares, pits, deadfalls, simple alarms, or other uncomplicated principles when appropriate materials are available.
- **Basic — Reliable contained traps:** Construct reusable or enclosed traps such as cages, weighted closures, trip mechanisms, simple pressure triggers, and other established designs with dependable activation and reset behavior.
- **Intermediate — Stored-energy and linked traps:** Build traps using springs, counterweights, tension, linked components, multiple moving parts, or chained mechanical actions. Integrate an ordinary weapon, projectile, restraint, alarm, or other physically compatible payload when the underlying components are available.
- **Advanced — Concealed and conditional traps:** Construct complex traps whose trigger, mechanism, or payload is difficult to detect; create multi-stage activation sequences; separate trigger from payload; and design traps that respond to simple physical criteria such as direction, weight, size, tension, opening, movement, or a particular sequence of mechanical events.
- **Master — Integrated trap systems:** Design original, highly complex traps combining several triggers, mechanisms, safeguards, payloads, or reset states. A Master may integrate another Skill, attack system, explosive, or magical effect **only when that other system actually provides a method for being stored, triggered, delivered, or mechanically incorporated**. Trap Making does not manufacture the other effect.

#### Boundaries and Synergy

**Trapping** selects, calibrates, and places traps against particular animals or creatures. **Trap Making** builds the trap.

**Disable Device** neutralizes or bypasses an existing mechanism. **Engineering** governs genuinely machine-like mechanisms beyond ordinary trap construction. **Explosives** creates and handles explosive charges while Trap Making may integrate them into a trigger and delivery system.

The legacy Master ability to incorporate another attack, Skill, or spell is preserved in spirit but remains subject to the actual rules of that other system.

Common Synergies include **Trap Making + Trapping**, **Trap Making + Engineering**, **Trap Making + Rope Use**, **Trap Making + Explosives**, and relevant weapon- or projectile-crafting Skills when specialized physical components materially contribute.

Trap Making grants no Limited Substitution into those Skills.

#### Capability, difficulty, and pace

Training determines trap architectures the Specialist knows how to build. Complexity, concealment, materials, precision, available space, intended trigger conditions, tools, and payload determine task tier.

Hasty Trap Making is appropriate for improvised emergency traps. Meticulous use is natural for concealed, conditional, reusable, or precision traps. Significant traps frequently use extended checks.

**Magical integration cannot bypass Magic's storage, trigger, maintenance, duration, or other limitations.** Exact magical integration remains dependent on the finalized Magic rules.

### Wood Carving:
> **Status:** ✅ CONFIRMED — subtractive woodworking progression, Carpentry boundary, and common Synergy relationships locked.

Wood Carving governs detailed subtractive shaping of wood into sculptural, ornamental, decorative, and finely shaped functional forms. Carpentry governs functional construction through cutting, fitting, joinery, and assembly.

- **Simple — Basic whittling and shaping:** Shape simple forms from a piece of wood using ordinary carving tools, such as stakes, handles, pegs, crude figurines, simple spoons, wedges, and comparable objects.
- **Basic — Functional and representational carving:** Produce recognizable small statues, whistles, handles, decorative panels, reliefs, toys, simple carved utensils, and other forms requiring controlled shape rather than merely rough utility.
- **Intermediate — Detailed carving:** Create intricate ornament, detailed relief work, complex curves, fitted carved components, decorative boxes, wind-instrument bodies, patterned surfaces, and sculpture requiring deliberate proportion and fine tool control.
- **Advanced — Intricate one-piece work:** Produce undercut, pierced, nested, interlocking, or highly delicate carvings such as wooden chains, captive forms, lattice work, deeply layered relief, and other pieces requiring exceptional planning because much or all of the complexity is carved from one original piece.
- **Master — Sculptural mastery:** Create highly detailed, lifelike, expressive, or exceptionally complex wooden sculpture; reproduce subtle textures and anatomy; execute minute ornamental detail; and design original carvings whose form requires mastery of grain, tool access, negative space, and structural fragility.

#### Boundaries and Synergy

**Carpentry** builds functional wooden objects through joinery and assembly. **Wood Carving** creates form primarily by removing and shaping material.

A carved furniture piece may use Carpentry as Primary with Wood Carving supporting the ornamentation. A puzzle box whose function depends on joints, sliding panels, or interlocking construction belongs primarily to Carpentry.

**Artistry** governs visual artistic composition across media. Wood Carving governs execution in wood. **Musical Instrument** governs playing and musical/acoustic expertise; Wood Carving can physically shape wooden instrument components.

Common Synergies include **Carpentry + Wood Carving**, **Wood Carving + Artistry**, **Wood Carving + Musical Instrument**, **Bowyer + Wood Carving**, and **Counterfeiting + Wood Carving** for distinctive carved details.

Wood Carving grants no Limited Substitution into Carpentry or Artistry.

#### Capability, difficulty, Quality, and pace

Training unlocks carving techniques and complexity, not automatic artistic Quality. Where artistic composition matters separately from carving execution, Artistry may provide Synergy.

Hasty use suits crude shaping or emergency functional carving. Meticulous use is natural for fine detail, undercut work, realism, and fragile pieces. Large sculptures use extended checks.

Quality and durability remain Crafting concerns.

### Writing:
> **Status:** ✅ CONFIRMED — composition progression, memory boundary, document boundaries, and common Synergy relationships locked.

Writing governs composing original written content: choosing words, structuring information, creating narratives, controlling tone and voice, and presenting factual or fictional material coherently to a reader.

- **Simple — Clear written account:** Produce a coherent short account, description, letter, instruction, or narrative from information the Specialist actually possesses. Preserve important points without requiring exceptional style or structure.
- **Basic — Structured composition:** Organize longer material into a logical sequence, maintain a consistent subject and tone, summarize or expand known information appropriately, and write for a particular ordinary audience or purpose.
- **Intermediate — Vivid and engaging prose:** Control pacing, imagery, characterization, explanation, narrative voice, and descriptive detail well enough to create compelling factual accounts or convincing fictional stories. Write fantastical or imaginative material with internal coherence.
- **Advanced — Complex and persuasive narrative construction:** Sustain long-form works, manage multiple characters or lines of information, foreshadow and resolve ideas, imitate established genres or broad stylistic conventions, and construct fictional accounts that read like plausible factual narratives when the supporting information is sufficient.
- **Master — Literary mastery:** Compose sophisticated long-form works with deliberate structure, layered themes, distinct voices, subtle characterization, controlled rhetoric, and sustained internal consistency; adapt style substantially for different audiences or purposes; and create original narrative forms without losing clarity or coherence.

#### Memory boundary

**Writing can only recount an event as accurately as the writer's memory, notes, testimony, or other sources permit. Training in Writing does not grant enhanced memory.**

When accurate facts must be recovered or verified, use History, Researching, Scribe, Local Geography, or another relevant Skill or source as appropriate.

#### Boundaries and Synergy

**Scribe** records and reproduces existing information accurately. **Calligraphy** determines the visual presentation of handwriting. **Writing** creates the content.

**Bluff** governs persuading another creature to believe something false. Advanced or Master Writing can create a plausible fictional account, but whether a particular reader accepts a false claim may require Bluff or another social mechanic.

**Counterfeiting** makes a document appear authentically issued or physically genuine. Writing may produce its text.

Common Synergies include **Writing + Researching**, **Writing + History**, **Writing + Scribe**, **Writing + Calligraphy**, **Writing + Musical Instrument** for lyrics and songs, **Writing + Public Speaking** for speeches, **Writing + Bluff** for deliberately deceptive written narratives, and **Counterfeiting + Writing** for forged documents whose wording must also be convincing.

Writing grants no Limited Substitution into those Skills.

#### Capability, difficulty, and pace

Length is usually a time issue rather than an automatic task-tier increase. Difficulty comes from structural complexity, audience, source quality, required precision, constraints, unfamiliar form, and purpose.

Hasty Writing covers rapid notes, hurried letters, rough reports, or emergency instructions. Meticulous Writing covers revision, restructuring, research integration, and deliberate word choice. Long-form work naturally uses extended checks.

If written persuasion later receives formal social mechanics, Writing should create the text while the appropriate social Skill determines its effect on a particular reader.

## Charisma

### Acting:
> **Status:** ✅ CONFIRMED — performance progression, social/performance boundaries, opposed use, and common Synergy relationships locked.

Acting governs deliberately portraying a role, emotional state, personality, or fictional identity through voice, expression, posture, movement, and performance.

- **Simple — Prepared performance:** Deliver rehearsed lines, actions, or emotional cues in a recognizable and reasonably consistent way. Perform a simple scripted role with minimal prompting.
- **Basic — Sustained scripted portrayal:** Maintain a prepared character or role through a complete scene without prompting, including appropriate tone, facial expression, posture, timing, and basic emotional presentation.
- **Intermediate — Character performance:** Portray believable emotional states and distinct fictional personalities rather than merely reciting prepared material. Adapt delivery to another performer, react naturally within a scene, and remain in character through minor unexpected changes.
- **Advanced — Adaptive portrayal:** Sustain a role through unscripted interaction, adjust emotion and behavior to changing circumstances, conceal genuine reactions when deliberately performing another state, and convincingly portray roles significantly different from the Specialist's normal demeanor.
- **Master — Improvisational embodiment:** Create and sustain a believable character or emotional performance with little or no preparation, improvise dialogue and behavior consistently, recover from major disruptions without visibly breaking character, and maintain a complex role across extended interactions.

#### Boundaries and Synergy

**Acting and Bluff:** Acting determines how convincingly the Specialist performs a role or displayed emotional state. Bluff determines whether the Specialist convinces someone that a false claim is true. Either may support the other when both materially contribute.

**Acting and Mimicry:** Acting portrays a role or personality. Mimicry reproduces the specific voice, gestures, habits, and mannerisms of another individual. **Acting + Mimicry** is a natural Synergy pairing when impersonating a particular person.

**Acting and Disguise:** Disguise changes physical appearance; Acting sells the behavior behind it. Either may be Primary depending on whether the central challenge is appearance or sustained portrayal.

**Acting and Public Speaking:** Public Speaking presents information effectively to an audience. Acting portrays a role. A theatrical monologue is primarily Acting; an address to a crowd is primarily Public Speaking. A staged speech performed in character may use Synergy.

Other common Synergies include **Acting + Musical Instrument**, **Acting + Singing**, and **Acting + Empathy** when understanding an emotional state materially helps portray it.

Acting grants no Limited Substitution into Bluff, Mimicry, Disguise, Public Speaking, or other related Skills.

#### Opposed use

Acting may be opposed by **Empathy** when another creature is trying to determine whether a displayed emotional state is genuine.

For specific impersonation, the opposing Skill depends on what the observer is actually scrutinizing. Disguise, Mimicry, Local Geography, Heraldry, Empathy, or another relevant Skill may matter when that knowledge or perception would expose the performance.

Failure does not automatically mean an observer knows the Specialist is lying. The performance may instead appear stiff, emotionally wrong, inconsistent, or suspicious according to the circumstances.

#### Capability, difficulty, and pace

Training degree determines performance capability; the role, audience, preparation, duration, scrutiny, circumstances, and required adaptation determine task tier.

Hasty Acting is appropriate when a role, cover, or emotional display must be invented almost immediately. Meticulous use most naturally represents rehearsal, preparation, character study, and deliberate refinement before a performance.

Long performances do not require constant rerolls merely because time passes. Use the extended/ongoing framework only when meaningful disruptions, changing audiences, sustained deception, or other pressures make continued performance uncertain.

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

### Construction:
> **Status:** ⬜ NEEDS DEVELOPMENT — governing Stat confirmed as **Stamina**. Full degree progression will be designed during the Stamina Skill pass.

Construction will govern turning plans, materials, labor, sequencing, and site conditions into completed structures. It is intended to remain distinct from Architecture (design), Engineering (structural/mechanical systems), Carpentry (wood fabrication and joinery), and Masonry (stone/brick/mortar work), while using Synergy with those Skills when their expertise materially overlaps.

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
