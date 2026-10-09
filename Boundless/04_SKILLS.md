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
- **Hunting + Trap Making:** choose effective placement and prey criteria while combining Hunting's behavioral knowledge with Trap Making's construction and calibration.
- **Listening + Hunting:** locate or interpret animal prey by sound.
- **Listening + Tracking:** follow an unseen moving target when sound materially contributes.
- **Listening + Search:** investigate hollow spaces, concealed mechanisms, or hidden areas where acoustic cues guide the examination.
- **Listening + Engineering:** diagnose machinery, mechanisms, or structural problems by sound.
- **Listening + Mimicry:** analyze subtle vocal details before reproducing them.
- **Pick Pocket + Sleight of Hand:** covertly transfer an object while concealing the hand movement or object through palming or misdirection.
- **Spot + Search:** use a visual irregularity noticed with Spot to guide a deliberate Search.
- **Bowyer + Carpentry:** difficult wooden components or elaborate stocks.
- **Bowyer + Blacksmithing/Weapon Crafting:** unusual metal components or reinforcement.
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
- **Fletching + Weapon Crafting:** create specialized metal heads or unusual ammunition hardware.
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
- **Armoring + Leatherworking:** construct leather armor whose protective design and general leathercraft both materially contribute.
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
- **Poisons + Medicine:** identify or respond to poisoning when toxicology, symptoms, exposure, and patient treatment materially overlap.
- **Rope Use + Climbing:** build and use technical climbing, rappelling, or rescue rigging.
- **Rope Use + Engineering:** operate or construct a lifting system combining rope rigging with genuine machinery.
- **Trap Making + Rope Use:** build snares, net traps, trip systems, or tensioned-line mechanisms.
- **Scribe + Researching:** collate sources, extract citations, or maintain structured scholarly records.
- **Scribe + Administration:** maintain complex organizational records where both accurate transcription and administrative structure matter.
- **Sewing + Artistry:** create textile work whose visual design materially contributes beyond construction.
- **Sewing + Rope Use:** construct and rig sails, tents, awnings, nets, or similar large textile systems.
- **Sleight of Hand + Acting:** perform concealed object manipulation within a staged character performance.
- **Sleight of Hand + Bluff:** use verbal deception to support a covert manual manipulation.
- **Trap Making + Hunting:** construct and calibrate traps around the behavior and physical characteristics of intended prey.
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
- **Diplomacy + Local Culture:** negotiate or observe protocol where specific cultural customs materially shape the interaction.
- **Diplomacy + Heraldry:** conduct formal dealings with noble or institutional parties where house knowledge materially matters.
- **Leadership + Administration:** direct people while a complex operation also depends on schedules, assignments, and resources.
- **Leadership + Strategy:** translate a military or competitive plan into coordinated action by followers.
- **Merchant + Appraise:** negotiate a transaction using a defensible estimate of the goods' actual value.
- **Merchant + Finance:** structure a deal whose cash flow, reserves, credit, or longer-term budget materially matter.
- **Mimicry + Lip Reading:** reproduce observed speech sounds by combining visible articulation analysis with vocal imitation.
- **Public Speaking + Leadership:** address a group in a way that supports actual command, cohesion, or motivation.
- **Alchemy + Chemistry:** formulate an alchemical preparation whose mundane chemical behavior materially contributes to its supernatural effect.
- **Alchemy + Apothecary:** formulate a supernatural preparation whose medicinal delivery or bodily interaction materially matters.
- **Apothecary + Medicine:** prepare or select a medicine specifically for a diagnosed patient's condition.
- **Chemistry + Explosives:** formulate or analyze energetic material while explosive charge design and controlled use remain under Explosives.
- **Education + Researching:** create curricula, reconstruct teaching material, or build a self-study path from difficult sources.
- **Geology + Prospecting:** identify promising formations and then follow or extract the actual deposit in the field.
- **Law + Researching:** build a legal argument from statutes, precedent, records, or other sources.
- **Navigation + Transportation (Specified):** maintain a route while actively operating the relevant conveyance.
- **Acrobatics + Swimming:** perform genuinely acrobatic movement underwater beyond ordinary aquatic maneuvering.
- **Hiding + Camouflage:** choose effective concealment while visual treatment materially helps the position blend into its surroundings.
- **Sneaking + Hiding:** move between concealed positions while managing both motion and line of sight.
- **Transportation (Specified) + Animal Handling:** operate an animal-drawn conveyance while the draft animals themselves require meaningful handling.
- **Seduction + Empathy:** read reciprocal attraction, comfort, hesitation, and interest while pursuing consensual intimacy.
- **Animal Handling + Riding:** direct or manage a mount where both mounted control and broader animal behavior materially matter.
- **Animal Handling + Animal Husbandry:** train or manage an individual animal whose long-term care, breeding, or population context materially matters.
- **Questioning + Empathy:** adapt inquiry to emotional reactions, discomfort, guardedness, or rapport.
- **Farming + Animal Husbandry:** coordinate crop and livestock systems on a mixed agricultural operation without merging the two Skills.
- **Construction + Architecture:** execute a structure whose design or unusual site integration materially affects the build.
- **Construction + Engineering:** build a structure containing specialized mechanical or structural systems.
- **Armoring + Blacksmithing:** construct armor whose forged metal components materially require both protective design and blacksmithing.
- **Armoring + Leatherworking:** construct armor whose protective design and leather shaping materially contribute.
- **Armoring + Sewing:** construct padded, quilted, textile, or mixed armor whose protective design and textile construction both matter.
- **Weapon Crafting + Blacksmithing:** construct a weapon whose forged metal components materially require both weapon design and blacksmithing.
- **Weapon Crafting + Metallurgy:** design or construct a weapon whose alloy composition materially affects performance.
- **Farrier + Animal Handling:** perform hoof or shoe work on an animal whose behavior materially affects the task.

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

Hunting governs the hunt itself: understanding wild prey, choosing an approach, predicting behavior, creating opportunities, adapting when the prey changes its behavior, and choosing where and how to employ traps against animal prey. It does not replace specialized Skills such as Camouflage, Tracking, or Trap Making, and it does not replace Combat/Martial rules when a hunt becomes a fight.

Hunting is commonly treated as an **Ongoing Skill**. It has no universal fixed interval; checks occur at meaningful stages of the hunt, such as locating likely prey, approaching it, setting an ambush, maintaining contact during a pursuit, or adapting when circumstances change.

Task tier is determined by the prey, terrain, danger, rarity, circumstances, and objective rather than by the Specialist's Training degree. Size alone does not determine whether prey may be hunted.

- **Simple — I can hunt:** Understands the basic habits of common wild game and can conduct an ordinary hunt using appropriate weapons, nets, positioning, and hunting methods. If the situation becomes structured combat, attacks and defenses use the normal Combat/Martial rules.
- **Basic — I know how not to be noticed by my prey:** Understands how animal prey perceives its surroundings well enough to use blinds, natural cover, decoys, positioning, and basic visual concealment against it. If the Specialist has no Camouflage Training, Basic Hunting grants **Limited Substitution: Simple Camouflage** when concealing themselves specifically from animal prey. If the Specialist has Camouflage Training, Hunting and Camouflage may use **Synergy** when both materially apply.
- **Intermediate — I know where it is going:** Reads prey behavior well enough to identify likely feeding areas, watering points, bedding areas, travel routes, escape paths, and other probable movements. If the Specialist has no Tracking Training, Intermediate Hunting grants **Limited Substitution: Simple Tracking** when following animal prey. If the Specialist has Tracking Training, Hunting and Tracking may use **Synergy** when both materially apply.
- **Advanced — I know how to make it do what I want:** Manipulates prey behavior through calls, scents, musks, lures, decoys, wind direction, flushing, driving, and similar techniques. The Specialist also understands **where, when, and why** an existing trap should be employed against particular prey. Constructing, repairing, calibrating, or mechanically modifying the trap remains **Trap Making**. When both materially apply, Hunting and Trap Making may use **Synergy**.
- **Master — I know how to hunt that specific prey:** Can plan and conduct hunts against exceptionally elusive, dangerous, unusual, or cunning wild prey; deliberately target a particular specimen; anticipate likely reactions to the hunters; and adapt the hunt when the prey changes its behavior. Master Hunting may use Synergy with the relevant specialized Skill but does not increase Limited Substitution above Simple Training.

**Camouflage and Tracking remain distinct Skills.** Hunting provides prey-specific knowledge and may support them through Synergy. The former **Trapping** Skill is removed: its prey-selection and placement knowledge is absorbed into Hunting, while its mechanical construction and trigger-calibration functions belong to **Trap Making**. Hunting does not grant Limited Substitution in Trap Making or replace the ability to construct sophisticated traps.

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

Bowyer governs the maintenance, repair, construction, modification, and design of bows and crossbows. It does not replace related Skills such as Fletching, Carpentry, Blacksmithing/Weapon Crafting, or Engineering, although those Skills may provide **Synergy** when they materially contribute to a particular task.

- **Simple — Maintain and assemble:** String, unstring, tune, inspect, clean, and maintain bows and crossbows. Replace ordinary consumable or wear components such as strings, cords, serving, and similar parts when appropriate materials are available.
- **Basic — Repair:** Diagnose and repair ordinary damage to bows and crossbows, including damaged strings, loose fittings, warped or damaged components, cracked stocks, minor limb or prod damage, trigger issues, and similar repairable problems.
- **Intermediate — Construct:** Build complete, conventional bows and crossbows from appropriate materials and components, including the ordinary fittings and mechanisms necessary for the weapon to function. A normal weapon does not require several unrelated crafting Skills merely because it contains several materials.
- **Advanced — Modify and specialize:** Alter existing bows and crossbows for a particular user or purpose, including adjustments to draw characteristics, balance, dimensions, stock configuration, trigger behavior, reinforcement, compactness, range-oriented design, heavy-draw construction, specialized mounting, or similarly meaningful modifications. Advanced Bowyers may also reproduce established unusual or complex designs when appropriate tools and materials exist.
- **Master — Design:** Create new bow or crossbow designs rather than merely reproduce established ones. A Master Bowyer may combine unusual materials, mechanisms, dimensions, and construction principles into functional prototypes and highly specialized weapons, subject to the normal limits of the setting and materials available.

#### Capability, difficulty, and Quality

Training degree determines **what the Specialist knows how to do**. It does not automatically determine the task tier. Replacing a string may be a Simple task even though Basic Bowyer permits broader repair work, while rebuilding a badly damaged heavy crossbow might be substantially more difficult. Likewise, Intermediate Bowyer unlocks weapon construction, but the difficulty of constructing a particular weapon depends on the design, materials, tools, conditions, and circumstances.

Training degree also does not automatically determine the **Quality** of the finished item. Quality, reliability, durability, and related crafting outcomes belong to the future Crafting/Quality rules.

#### Related Skills and Synergy

Common Synergy candidates include Bowyer + Carpentry for difficult wooden components or elaborate stocks, Bowyer + Blacksmithing/Weapon Crafting for unusual metal components or reinforcement, Bowyer + Engineering for unconventional mechanical crossbow designs, and Bowyer + Fletching when tuning ammunition characteristics to a particular weapon. The actual construction of arrows or bolts remains a Fletching task.

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
- **Weapon Crafting** for weapons and makers' marks tied to construction.
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
- **Fletching + Weapon Crafting:** specialized metal heads or unusual ammunition hardware.
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
> **Status:** ✅ CONFIRMED — non-armor leathercraft progression, material boundaries, and common Synergy relationships locked. Armor construction is now consolidated under Armoring.

Leatherworking governs preparing hides and constructing, shaping, repairing, decorating, and fitting **non-armor leather goods** with the appropriate tools, materials, and workspace.

- **Simple — Hide handling and basic repair:** Remove a usable hide or skin from a creature when circumstances permit, clean and preserve it well enough for later processing, cut prepared leather, punch holes, stitch simple seams, and perform minor repairs on ordinary leather goods.
- **Basic — Conventional leather goods:** Construct straightforward belts, pouches, straps, sheaths, simple footwear, gloves, bags, basic garments, covers, and similar items from prepared leather using established patterns.
- **Intermediate — Shaping and fitted construction:** Wet-form, mold, stretch, fit, reinforce, edge, line, and assemble leather into comfortable or closely fitted garments and more complex goods. Produce durable fitted boots, fitted clothing, shaped cases, harness components, and comparable work.
- **Advanced — Refinement and complex leathercraft:** Refine, soften, dye, finish, tool, emboss, layer, and combine leather for demanding applications. Construct complex saddles, fitted harness, heavy-duty packs, articulated non-armor goods, elaborate clothing, and other objects where shaping and load distribution matter.
- **Master — Advanced leather fabrication:** Design and create highly complex leather constructions combining shaping, reinforcement, multiple leather weights, precise fitting, decoration, and unusual forms. Given appropriate material, a Master Leatherworker can fabricate nearly any object whose defining construction is genuinely leatherwork rather than armor, machinery, or another specialist craft.

#### Boundaries and Synergy

**Armoring** owns armor whose defining purpose is protective construction, including leather armor. Leatherworking may prepare decorative elements, straps, liners, fittings, shaped leather, or raw material but does not substitute for Armoring.

**Sewing** governs cloth and textile construction; Leatherworking governs hide and leather. Mixed-material goods may use Synergy.

Common Synergies include **Leatherworking + Sewing**, **Armoring + Leatherworking**, **Leatherworking + Animal Husbandry** for specialized tack, **Counterfeiting + Leatherworking**, and **Leatherworking + Artistry** for elaborate tooling or decorative work.

Leatherworking grants no Limited Substitution into Armoring or Sewing.

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

Common Synergies include **Poisons + Herbology**, **Poisons + Apothecary**, **Poisons + Chemistry**, **Poisons + Alchemy**, **Poisons + Fletching**, and **Poisons + Medicine** when symptoms or treatment materially contribute.

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

Common Synergies include **Rope Use + Climbing**, **Rope Use + Escape**, **Escape + Rope Use**, **Rope Use + Engineering**, **Trap Making + Rope Use**, and vessel rigging applications where **Transportation (Specified)** materially contributes.

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

**Hunting** determines prey behavior and effective placement against animal targets. **Trap Making** designs, builds, repairs, and mechanically calibrates the trap.

**Disable Device** neutralizes or bypasses an existing mechanism. **Engineering** governs genuinely machine-like mechanisms beyond ordinary trap construction. **Explosives** creates and handles explosive charges while Trap Making may integrate them into a trigger and delivery system.

The legacy Master ability to incorporate another attack, Skill, or spell is preserved in spirit but remains subject to the actual rules of that other system.

Common Synergies include **Trap Making + Hunting**, **Trap Making + Engineering**, **Trap Making + Rope Use**, **Trap Making + Explosives**, and relevant weapon- or projectile-crafting Skills when specialized physical components materially contribute.

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

**Acting and Bluff:** Acting determines how convincingly the Specialist performs a role or displayed emotional state. Bluff determines whether the Specialist convinces someone that a false claim is true.

**Acting and Mimicry:** Acting portrays a role or personality. Mimicry reproduces the specific voice, gestures, habits, and mannerisms of another individual.

**Acting and Disguise:** Disguise changes physical appearance; Acting sells the behavior behind it.

**Acting and Public Speaking:** Public Speaking presents information effectively to an audience. Acting portrays a role.

Common Synergies include **Acting + Mimicry**, **Acting + Disguise**, **Acting + Bluff**, **Acting + Public Speaking**, **Acting + Musical Instrument**, **Acting + Singing**, and **Acting + Empathy**.

Acting grants no Limited Substitution into those Skills.

#### Opposed use and pace

Acting may be opposed by **Empathy** when another creature is trying to determine whether a displayed emotional state is genuine. Specific impersonation may bring Disguise, Mimicry, Local Culture, Heraldry, or another relevant Skill into the contest depending on what is being scrutinized.

Failure does not automatically mean an observer knows the truth; the performance may merely seem stiff, emotionally wrong, inconsistent, or suspicious.

Hasty Acting covers an improvised cover or emotional display. Meticulous Acting covers rehearsal, character study, and deliberate preparation. Long performances use ongoing checks only when meaningful new pressure arises.

### Bluff:
> **Status:** ✅ CONFIRMED — deception capability, opposed use, and social boundaries locked.

Bluff governs deliberate deception through false statements, omissions, feigned certainty, concealed reactions, and improvised verbal misdirection. It does not alter physical evidence or force belief where no plausible path to belief exists.

- **Simple — Minor deception:** Present a small, plausible falsehood or alter an incidental detail without obvious contradiction.
- **Basic — Sustained lie:** Maintain a coherent false account through ordinary follow-up questions.
- **Intermediate — Controlled tells:** Maintain a poker face, conceal obvious nervousness, and use verbal misdirection while under moderate scrutiny.
- **Advanced — Complex fabrication:** Sustain layered lies involving several facts, people, or motives and adapt the story when challenged.
- **Master — Adaptive deception:** Maintain an elaborate deception through extended interaction and make highly unlikely claims seem plausible when circumstances, evidence, or the target's beliefs provide a credible route to belief.

#### Boundaries and Synergy

Acting performs a role; Bluff asserts or implies something false. Disguise changes appearance. Mimicry copies specific external behavior. Writing composes text. Counterfeiting creates deceptive objects or documents.

Common Synergies include **Bluff + Acting**, **Bluff + Disguise**, **Bluff + Mimicry**, **Bluff + Writing**, and **Bluff + Sleight of Hand**.

Bluff may be opposed by **Empathy**, **Questioning**, or another Skill that genuinely represents the listener's route to exposing the deception. Bluff grants no Limited Substitution.

The legacy combat-distraction use is handled through the confirmed **integrated Skill maneuver** rules rather than a separate universal defense penalty.

### Diplomacy:
> **Status:** ✅ CONFIRMED — protocol, negotiation, mediation, and cross-cultural social boundaries locked.

Diplomacy governs formal etiquette, negotiation, mediation, protocol, and management of relationships between people or groups with potentially different interests.

- **Simple — Familiar courtesy:** Observe ordinary formal respect, introductions, titles, and expected public etiquette in familiar settings.
- **Basic — Formal protocol:** Navigate structured meetings, audiences, ceremonies, negotiations, and status differences without obvious breaches.
- **Intermediate — Cross-cultural adaptation:** Infer the social function of unfamiliar etiquette from context and adjust behavior quickly enough to participate respectfully.
- **Advanced — Negotiation and mediation:** Identify competing interests, frame compromises, preserve face, and de-escalate formal disputes when an agreement is realistically possible.
- **Master — High-stakes diplomacy:** Manage complex negotiations involving several parties, protocol, concessions, reputation, and long-term consequences.

#### Boundaries and Synergy

**Local Culture** supplies specific customs; **Heraldry** supplies noble-house knowledge; **Law** supplies legal constraints; **Leadership** motivates followers; **Merchant** handles commerce.

Common Synergies include **Diplomacy + Local Culture**, **Diplomacy + Heraldry**, **Diplomacy + Law**, **Diplomacy + Empathy**, and **Diplomacy + Merchant**. Diplomacy grants no Limited Substitution.

Task tier depends on unfamiliarity, stakes, hostility, number of parties, and conflict of interests. Major negotiations naturally support extended resolution.

### Intimidate:
> **Status:** ✅ CONFIRMED — coercion-through-threat identity and autonomy boundaries locked.

Intimidate governs using credible threat, presence, leverage, and controlled menace to make another creature fear a consequence strongly enough to alter its immediate choices. It is coercion, not mind control.

- **Simple — Obvious threat:** Pressure a vulnerable target when the Specialist has an evident advantage or credible consequence.
- **Basic — Controlled menace:** Communicate threat convincingly through posture, tone, timing, or displayed capability without immediately acting on it.
- **Intermediate — Read leverage:** Identify what a target fears losing and frame a credible threat around that vulnerability.
- **Advanced — Hardened opposition:** Pressure disciplined, experienced, angry, or socially protected targets when sufficient leverage or danger exists.
- **Master — Strategic intimidation:** Use layered threats, reputation, timing, and situational leverage against individuals or groups that would ignore ordinary menace.

#### Boundaries and Synergy

Bluff can falsify a threat's truth; Intimidate makes the consequence emotionally compelling. Leadership motivates coordinated followers. Torture inflicts suffering. Empathy may reveal fear or leverage.

Common Synergies include **Intimidate + Bluff**, **Intimidate + Empathy**, **Intimidate + Acting**, and situational **Intimidate + Leadership**. Intimidate grants no Limited Substitution.

A target with no reason to believe the threat, or no meaningful concern about its consequence, may simply be impossible to intimidate by that route. Exact fear/morale Conditions remain a later dependency.

### Leadership:
> **Status:** ✅ CONFIRMED — group direction, motivation, and command boundaries locked.

Leadership governs organizing, motivating, directing, and sustaining coordinated effort among people who have some reason to accept the Specialist's authority or guidance. It does not create permanent loyalty or erase incompatible goals.

- **Simple — Small-team direction:** Give clear immediate direction to a small willing group and keep members focused on a straightforward objective.
- **Basic — Maintain cohesion:** Coordinate a team through routine confusion, fatigue, disagreement, or pressure while assigning useful roles.
- **Intermediate — Unit leadership:** Rally demoralized groups, reorganize disrupted teams, and communicate priorities through subordinate leaders.
- **Advanced — Large-group command:** Direct large organizations or forces through changing circumstances while delegating effectively and maintaining cohesion.
- **Master — Institutional leadership:** Coordinate several major groups or command structures over extended operations while balancing morale, delegation, competing priorities, and strategic intent.

#### Boundaries and Synergy

**Administration** organizes tasks, resources, records, and schedules; Leadership directs people. **Strategy** creates military or competitive plans; Leadership gets people to execute them. **Public Speaking** addresses audiences.

Common Synergies include **Leadership + Administration**, **Leadership + Strategy**, **Leadership + Public Speaking**, **Leadership + Empathy**, and **Leadership + Diplomacy**.

Exact morale, command, or follower bonuses remain a later dependency rather than an automatic effect of this Skill.

### Merchant:
> **Status:** ✅ CONFIRMED — trade negotiation, market behavior, and Appraise/Finance boundaries locked.

Merchant governs commercial negotiation, barter, sales practice, market behavior, deal structure, and practical conduct of trade.

- **Simple — Routine trade:** Conduct ordinary purchases and sales, recognize obviously favorable or unfavorable offers, and follow common market practices.
- **Basic — Bargain:** Negotiate price, quantity, delivery, or simple terms and operate a small stall or comparable retail activity.
- **Intermediate — Complex exchange:** Barter unlike goods or services, account for scarcity and demand, and structure deals involving credit, delivery, commissions, or multiple items.
- **Advanced — Market positioning:** Negotiate high-value or specialized transactions and identify leverage among several buyers or sellers.
- **Master — Brokerage and trade networks:** Structure major multi-party transactions, broker scarce or unusual goods, and negotiate deals whose value depends on timing, access, reputation, or distribution.

#### Boundaries and Synergy

**Appraise** estimates value; Merchant negotiates the transaction. **Finance** manages budgets and cash flow. **Bluff** handles deliberate deception. **Smuggling** moves concealed contraband.

Common Synergies include **Merchant + Appraise**, **Merchant + Finance**, **Merchant + Diplomacy**, **Merchant + Bluff** when deception is actually used, and **Merchant + Local Geography/Local Culture** when local markets materially matter.

Market fluctuation and economic tables remain later world/economy dependencies.

### Mimicry:
> **Status:** ✅ CONFIRMED — voice/mannerism reproduction and impersonation boundaries locked.

Mimicry governs reproducing observed sounds, voices, speech patterns, gestures, posture, and habitual mannerisms. It copies recognizable external behavior; Acting supplies the broader role and personality.

- **Simple — Surface imitation:** Copy obvious inflection, rhythm, simple nonverbal sounds, or conspicuous gestures after observation.
- **Basic — Vocal shaping:** Deliberately alter pitch, resonance, cadence, and pronunciation to reproduce broad vocal qualities unlike the Specialist's normal voice.
- **Intermediate — Specific voice:** Reproduce a particular person's recognizable speech pattern or a complex observed sound with sufficient exposure.
- **Advanced — Behavioral mimicry:** Reproduce characteristic gestures, posture, pacing, habitual expressions, and other physical mannerisms alongside vocal traits.
- **Master — Integrated imitation:** Combine voice, cadence, gestures, posture, and small habits into a highly convincing external imitation of a specific observed individual or sound source for extended periods.

Mimicry does not provide the target's memories, knowledge, motives, or relationships.

Common Synergies include **Mimicry + Acting**, **Mimicry + Disguise**, **Mimicry + Listening**, **Mimicry + Lip Reading**, and **Mimicry + Bluff**. Mimicry grants no Limited Substitution.

### Public Speaking:
> **Status:** ✅ CONFIRMED — audience presentation progression and Leadership/Acting boundaries locked.

Public Speaking governs presenting information clearly and compellingly to an audience while controlling delivery, structure, attention, pacing, and interaction.

- **Simple — Prepared reading:** Deliver prepared text audibly and intelligibly to a cooperative audience.
- **Basic — Structured presentation:** Speak from notes or an outline while maintaining organization and clarity.
- **Intermediate — Audience engagement:** Adjust pacing, emphasis, examples, and explanation to maintain interest and make information understandable.
- **Advanced — Adaptive address:** Handle interruptions, questions, hostile reactions, or changing audience mood while preserving the purpose of the speech.
- **Master — Large-scale oratory:** Hold and direct the attention of large, difficult, or divided audiences through exceptional structure, delivery, timing, and responsiveness.

Common Synergies include **Public Speaking + Writing**, **Public Speaking + Leadership**, **Public Speaking + Acting**, **Public Speaking + Diplomacy**, and **Public Speaking + Empathy**.

Public Speaking does not automatically create loyalty, make false claims true, or override an audience's interests. Formal crowd-morale effects remain a later dependency.

### Singing:
> **Status:** ✅ CONFIRMED — vocal music progression and performance boundaries locked.

Singing governs controlled musical use of the voice: pitch, rhythm, breath, tone, phrasing, harmony, interpretation, improvisation, and vocal composition.

- **Simple — Basic vocal control:** Sustain intentional pitch and rhythm, hum or sing simple melodies, and manage ordinary breathing through short phrases.
- **Basic — Prepared song:** Perform complete straightforward songs from notation, memorization, or rehearsal with recognizable pitch and timing.
- **Intermediate — Fluent performance:** Maintain pitch, phrasing, dynamics, and breath through complete songs; harmonize or perform reliably with others; and recover from minor errors.
- **Advanced — Arrangement and improvisation:** Improvise within an established form, alter melody or phrasing intentionally, compose functional vocal music, and adapt to accompaniment or other singers.
- **Master — Vocal mastery:** Perform technically exceptional material, sustain difficult control and expression, improvise extended original passages, and compose sophisticated vocal works.

**Musical Instrument (Specified)** governs instruments. **Writing** governs lyrics. **Acting** governs role portrayal.

Common Synergies include **Singing + Musical Instrument**, **Singing + Writing**, **Singing + Acting**, and **Singing + Public Speaking** in performances that genuinely use both.

### Torture:
> **Status:** ✅ CONFIRMED — controlled suffering, coercion boundary, and truth-information safeguard locked.

Torture governs the deliberate infliction and control of physical or psychological suffering for punishment, coercion, domination, or intimidation. It does **not** determine whether information obtained under suffering is true.

- **Simple — Controlled suffering:** Apply a deliberately painful or distressing method while retaining some control over intensity and immediate risk.
- **Basic — Sustained coercive harm:** Maintain suffering over time while better controlling accidental escalation and the subject's immediate physical response.
- **Intermediate — Calibrated pressure:** Adjust intensity based on the subject's condition, recognize obvious danger signs, and combine periods of pressure and relief without assuming medical expertise.
- **Advanced — Psychological torment:** Deliberately exploit isolation, anticipation, fear, humiliation, uncertainty, or other nonphysical pressures.
- **Master — Integrated coercive regime:** Combine physical and psychological pressure over extended periods while deliberately managing escalation, timing, condition, and coercive objective.

**Questioning** obtains and evaluates information. **Intimidate** threatens consequences. **Medicine** manages injury. Common Synergies include **Torture + Questioning**, **Torture + Intimidate**, **Torture + Empathy**, and **Torture + Medicine** where both genuinely apply.

Exact injury, trauma, Fatigue, morale, and Condition effects remain later dependencies. The Skill requires no detailed real-world harm procedures to function at the table.

## Intelligence

### Administration:
> **Status:** ✅ CONFIRMED — organizational coordination, records, delegation, and Leadership boundary locked.

Administration governs organizing people, tasks, records, schedules, resources, and responsibilities so a group or institution can accomplish planned work.

- **Simple — Small-task coordination:** Organize a few people, assignments, supplies, or records for a short straightforward project.
- **Basic — Routine operation:** Maintain schedules, responsibilities, inventories, and recurring processes for a small organization or project.
- **Intermediate — Multi-team coordination:** Coordinate several work streams, deadlines, dependencies, and records across a medium project or organization.
- **Advanced — Large operation:** Build and maintain administrative systems for large organizations, complex projects, or several simultaneous efforts.
- **Master — Institutional administration:** Coordinate multiple organizations, departments, or major projects over long periods while managing delegation, reporting, resources, contingencies, and changing priorities.

**Leadership** directs and motivates people; Administration structures the work. **Finance** manages money; Administration tracks broader resources and tasks.

Common Synergies include **Administration + Leadership**, **Administration + Finance**, **Administration + Scribe**, **Administration + Construction**, and **Administration + Strategy** where logistics materially matter.

Large projects are natural extended tasks. Exact workforce/productivity modifiers remain later organization/crafting dependencies.

### Alchemy:
> **Status:** ✅ CONFIRMED — explicitly mystical craft identity, ingredient harvesting/preservation, and supernatural-effect boundary locked.

Alchemy is the prepared-substance craft of producing **supernatural or spell-like effects** through formulae, catalysts, rare ingredients, transformation, and controlled mystical reactions. Alchemy is not merely advanced Chemistry.

- **Simple — Recognize and prepare alchemical ingredients:** Identify known alchemical uses, document observed supernatural properties, clean, stabilize, measure, and prepare ordinary mystical ingredients for later work.
- **Basic — Reproduce minor supernatural effects:** Follow established formulae for modest spell-like effects using suitable ingredients, such as brief sensory enhancement, minor light or darkness effects, temporary warmth or cooling beyond ordinary chemistry, or comparable low-order phenomena.
- **Intermediate — Harvest and preserve unusual reagents:** Safely harvest and preserve alchemically significant material from flora, fauna, minerals, magical creatures, environments, or other unusual sources while retaining the property needed by a known formula. Create more substantial established potions, oils, powders, fumes, or similar preparations.
- **Advanced — Transform and modify effects:** Alter established formulae, combine compatible mystical properties, change delivery form where plausible, and create potent temporary supernatural effects such as major sensory alteration, significant temporary Stat modification, extraordinary resistance, or similarly powerful transformations.
- **Master — Spell-like formulation:** Develop or reproduce sophisticated supernatural preparations capable of effects such as invisibility, fire breathing, dramatic temporary Stat changes, supernatural senses, major transformation, or other spell-like results permitted by the Alchemy/Crafting rules.

#### Boundaries and Synergy

**Chemistry** governs mundane chemical science and reactions. **Apothecary** creates medicinal preparations that support, enhance, or accelerate bodily processes. **Alchemy** crosses the line into explicitly supernatural effects.

An Apothecary preparation may stop bleeding, dull severe pain, fight infection, improve recovery, or restore some lost function through extraordinary medicine. A draught that regenerates destroyed tissue, regrows a limb, reverses petrification, or otherwise performs restoration the body could not naturally accomplish is Alchemy.

**Poisons** governs toxicological use. **Herbology** identifies plants and their natural properties.

Common Synergies include **Alchemy + Chemistry**, **Alchemy + Herbology**, **Alchemy + Apothecary**, **Alchemy + Poisons**, and relevant creature/monster knowledge when harvesting an unusual reagent.

#### Capability, difficulty, and dependencies

Training degree determines the kinds of supernatural formulation the Specialist can understand. Formula complexity, ingredient rarity, stability, potency, duration, delivery, and desired effect determine task tier.

Alchemy does **not** bypass Magic balance merely because its effect is bottled. Exact effect strength, duration, stacking, storage, activation, failure, ingredient costs, Quality, and interaction with Magic remain dependencies for the Alchemy/Crafting pass.

### Apothecary:
> **Status:** ✅ CONFIRMED — medicine-preparation identity, extraordinary natural healing scope, and Alchemy/Poisons boundaries locked.

Apothecary governs preparing medicinal salves, balms, tonics, poultices, powders, pills, washes, painkillers, antidotes, and other remedies that support, enhance, or accelerate processes a living body could naturally perform.

- **Simple — Basic remedies:** Prepare simple bandaging compounds, soothing pastes, mild salves, washes, and other treatments for minor wounds, irritation, or discomfort from known recipes.
- **Basic — Functional medicines:** Prepare painkillers, fever reducers, antiseptic or cleansing preparations, basic antidotal remedies, and medicines in common liquid, paste, or salve forms.
- **Intermediate — Stable formulations:** Produce powders, concentrated preparations, preserved doses, more reliable antidotes, and multi-ingredient medicines whose preparation requires careful measurement and sequencing.
- **Advanced — Potent medicine:** Prepare numbing agents, strong pain control, pills or measured doses, powerful recovery aids, and treatments that meaningfully accelerate clotting, recovery, or resistance to ordinary disease or injury.
- **Master — Extraordinary medicine:** Formulate exceptionally potent but still biologically grounded medicines capable of rapid stabilization, major pain control, significant antidotal effects, accelerated natural healing, disease recovery, or restoration allowed by the Health/Crafting rules.

#### Boundaries and Synergy

**Medicine** diagnoses and treats the patient directly. **Apothecary** makes the medicine.

**Poisons** is the specialist toxicology Skill. Apothecary may recognize harmful dosage or formulate antidotal medicine, but specialized poison extraction, weaponization, toxic refinement, and advanced toxicology belong to Poisons.

**Alchemy** creates supernatural effects. Apothecary can push natural healing unusually far, but actual regeneration or other restoration impossible through the body's natural processes belongs to Alchemy.

Common Synergies include **Apothecary + Medicine**, **Apothecary + Herbology**, **Apothecary + Chemistry**, **Apothecary + Poisons**, and **Apothecary + Alchemy** where a formula truly straddles the boundary.

Exact healing values, recovery acceleration, dosage, addiction/tolerance, antidote rules, costs, and Crafting Quality remain later dependencies.

### Appraise:
> **Status:** ✅ CONFIRMED — valuation progression and Merchant/domain-knowledge boundaries locked.

Appraise governs estimating the monetary, trade, collector, or practical market value of goods and services from available evidence.

- **Simple — Common goods:** Estimate the ordinary local value of familiar trade goods, tools, supplies, and services.
- **Basic — Specialized materials:** Evaluate common jewelry, gems, precious materials, crafted goods, and other items whose value depends on workmanship or material quality.
- **Intermediate — Art and specialist goods:** Estimate the value of art, rare craftwork, specialized equipment, and unusual goods when sufficient comparison or expertise exists.
- **Advanced — Markets and exchange:** Compare currencies, regional prices, scarcity, condition, provenance, and market differences to estimate likely exchange value.
- **Master — Unique and obscure objects:** Establish a defensible value range for ancient, unique, highly rare, or poorly documented objects by combining material evidence, provenance, comparable sales, historical significance, and likely buyer demand.

Appraise determines **value**, not authenticity by itself. Counterfeiting, Artistry, Jeweler, History, Heraldry, Metallurgy, or another domain Skill may provide Synergy when those facts matter.

**Merchant** negotiates the deal after value is estimated.

### Architecture:
> **Status:** ✅ CONFIRMED — building design/site planning identity and Construction/Engineering boundaries locked.

Architecture governs designing buildings and habitable structures: layout, spatial planning, circulation, site use, structural intent, environmental integration, and production of plans from which construction can proceed.

- **Simple — Concept design:** Produce readable building concepts, room relationships, basic dimensions, and straightforward layouts.
- **Basic — Site-aware design:** Account for grade, drainage, access, orientation, ordinary foundations, and common site constraints.
- **Intermediate — Resource and systems planning:** Design around available materials, climate, local resources, occupancy, circulation, and ordinary structural requirements.
- **Advanced — Difficult-site architecture:** Integrate buildings into unusual landscapes or constraints such as cliffs, trees, bridges, dense urban sites, underground spaces, or irregular terrain.
- **Master — Complete architectural plans:** Produce coordinated, detailed multi-level plans for complex structures, including dimensions, sections, sequencing assumptions, and interfaces with specialist systems.

**Construction** executes the structure. **Engineering** handles machine-like or specialized structural/mechanical systems. **Carpentry**, **Masonry**, and other crafts fabricate material-specific work.

Common Synergies include **Architecture + Construction**, **Architecture + Engineering**, **Architecture + Geography**, **Architecture + Mathematics**, and material craft Skills where the design depends on them.

Building performance, structural loads, project costs, and construction times remain Crafting/Construction dependencies.

### Camping:
> **Status:** ✅ CONFIRMED — field-camp setup, shelter, comfort, and campsite-risk progression locked.

Camping governs selecting, establishing, maintaining, and breaking a temporary campsite using carried gear and available environmental resources.

- **Simple — Basic camp tasks:** Select serviceable firewood, establish a basic fire where permitted, organize bedrolls, and perform routine camp setup.
- **Basic — Shelter and camp organization:** Pitch ordinary tents or tarps, arrange sleeping and work areas, and protect common gear from routine weather.
- **Intermediate — Food and wildlife precautions:** Store food and refuse responsibly, reduce ordinary wildlife problems, organize sanitation, and choose a campsite with practical access to water and resources.
- **Advanced — Difficult-condition camping:** Improve shelter, drainage, wind protection, warmth, cooling, comfort, and safety under poor weather or terrain.
- **Master — Improvised field shelter:** Establish a safe, functional camp using minimal carried equipment and appropriate natural materials, selecting the best available location while balancing exposure, water, hazards, concealment, and comfort.

Common Synergies include **Camping + Geography**, **Camping + Meteorology**, **Camping + Hunting**, **Camping + Rope Use**, and **Camping + Local Geography**.

Camping does not replace Construction for permanent structures or Medicine for health effects. Exact rest/recovery benefits, exposure rules, and environmental hazards remain later dependencies.

### Chemistry:
> **Status:** ✅ CONFIRMED — mundane chemical science, practical product scope, and Alchemy/Explosives boundaries locked.

Chemistry governs **mundane** chemical substances, reactions, analysis, refinement, formulation, and practical chemical products. Its effects may be impressive, dangerous, or technologically advanced, but they arise from material chemistry rather than supernatural transformation.

- **Simple — Controlled experimentation:** Safely combine familiar substances, observe reactions, document results, measure basic quantities, and recognize obvious chemical hazards.
- **Basic — Refinement and preparation:** Separate, purify, concentrate, dissolve, neutralize, preserve, or otherwise prepare known compounds using established procedures.
- **Intermediate — Predictive chemistry:** Compare known reactions, identify likely incompatibilities, reproduce practical compounds, and formulate useful materials such as dyes, solvents, adhesives, preservatives, smoke compounds, simple luminous substances, protective balms/coatings, or energetic precursors where setting technology permits.
- **Advanced — Applied formulation:** Design or adapt acids, bases, corrosives, incendiary or heat-producing compounds, cooling or insulating mixtures, reactive coatings, advanced luminous compounds, sophisticated solvents, and other high-performance mundane chemical products.
- **Master — Chemical analysis and design:** Identify properties of unfamiliar substances through appropriate senses, tests, and scientific method; infer likely reactions; and design new mundane formulations from understood components.

#### Boundaries and Synergy

**Alchemy** produces supernatural effects. Chemistry does not make invisibility potions, supernatural Stat enhancements, or magical regeneration.

**Explosives** governs designing, assembling, shaping, placing, triggering, and controlling explosive charges. Chemistry may create or analyze an energetic material or explosive precursor, but that does not grant Explosives capability.

**Poisons** governs toxicological use. Chemistry may identify or synthesize toxic chemicals, while Poisons governs preparation and employment specifically as poisons.

Common Synergies include **Chemistry + Explosives**, **Chemistry + Poisons**, **Chemistry + Apothecary**, **Chemistry + Alchemy**, and **Chemistry + Metallurgy** where reactions materially affect metal processing.

Exact product lists, damage, durations, protection values, availability, and Crafting costs remain later dependencies.

### Cryptography:
> **Status:** ✅ CONFIRMED — code/cipher creation and analysis locked; unknown-language translation explicitly excluded.

Cryptography governs encoding, encrypting, analyzing, and deciphering deliberately obscured written or symbolic information.

- **Simple — Use known keys:** Encode or decode straightforward messages when the correct key, cipher procedure, or codebook is available.
- **Basic — Create routine codes:** Design and use basic substitution systems, code phrases, keys, and simple ciphers suitable for ordinary secrecy.
- **Intermediate — Analyze weak systems:** Break familiar or flawed codes through pattern analysis, generic keys, frequency, repetition, contextual testing, and systematic trial.
- **Advanced — Keyless cryptanalysis:** Attack unfamiliar sophisticated ciphers without the intended key when enough material or structural evidence exists; design stronger layered systems.
- **Master — Complex symbolic analysis:** Analyze highly complex, damaged, partial, archaic, or multi-layer encoded documents and identify recurring structure in unknown writing systems.

Cryptography does **not** automatically translate an unknown language. At Master, it may identify repeated symbols, separators, numerical patterns, likely names, or encoded structure, but semantic translation requires language knowledge or another rule that grants it.

Common Synergies include **Cryptography + Mathematics**, **Cryptography + Researching**, **Cryptography + Scribe**, **Cryptography + Cartography**, and relevant linguistic or historical knowledge.

### Education:
> **Status:** ✅ CONFIRMED — pedagogy identity and Learning Access role locked; exact advancement discount deferred.

Education governs teaching: breaking knowledge into learnable steps, diagnosing misunderstanding, structuring practice, adapting explanations, building curricula, and accelerating another person's acquisition of a Skill the instructor actually knows.

- **Simple — Teach fundamentals:** Effectively teach Simple techniques of a Skill the instructor possesses at Simple or better.
- **Basic — Structured instruction:** Teach through Basic techniques, organize practice, identify common beginner errors, and adjust explanations to the learner.
- **Intermediate — Developing expertise:** Teach through Intermediate techniques, diagnose persistent mistakes, sequence exercises, and guide students from rules toward judgment.
- **Advanced — Advanced instruction:** Teach through Advanced techniques, adapt instruction to unusual learners or circumstances, and build effective multi-stage curricula.
- **Master — Master instruction:** Teach any degree the instructor personally possesses, train other instructors, design comprehensive programs, and reconstruct effective teaching methods for exceptionally difficult material.

#### Learning Access

Before purchasing a new Skill degree, a Specialist must have a reasonable means of acquiring that knowledge. **Learning Access** may come from:
- instruction or demonstration by someone who possesses the desired degree;
- self-directed study from appropriate resources, usually supported by **Researching**;
- sufficient meaningful practical experience with the Skill.

A skilled practitioner does **not** need Education merely to demonstrate what they know. Education represents the ability to teach it efficiently.

A qualified instructor with sufficient Education may reduce the student's advancement cost and/or required training time. The exact reduction remains deferred until the advancement-cost economy is finalized.

Normal instruction with adequate time does not require a roll merely to permit advancement. Education checks are for genuine uncertainty: compressed training, unusual barriers, poor resources, difficult learners, reconstructing a curriculum, or similarly meaningful complications.

Common Synergies include **Education + Researching**, **Education + Administration**, and **Education + the taught Skill** when evaluating or designing instruction.

### Engineering:
> **Status:** ✅ CONFIRMED — machine/system design identity and Disable Device/Construction boundaries locked.

Engineering governs understanding, designing, assembling, modifying, and diagnosing machines or devices whose function depends on interacting mechanical systems such as gears, springs, linkages, cams, transmissions, pressure, power transfer, or comparable setting technology.

- **Simple — Simple mechanisms:** Safely disassemble, inspect, and understand straightforward mechanical devices.
- **Basic — Restore simple devices:** Reassemble, repair, and adjust ordinary mechanisms from known designs.
- **Intermediate — Complex mechanism analysis:** Disassemble, diagnose, repair, or modify multi-part machines and determine how their systems interact.
- **Advanced — Complex system construction:** Reassemble and construct advanced mechanisms, integrate multiple systems, alter function within the capability of the components, and troubleshoot unfamiliar machinery.
- **Master — Original engineering:** Design and construct new complex devices or machines from first principles within available materials, power sources, technology, and Crafting rules.

**Disable Device** interferes with an existing mechanism. **Trap Making** builds traps. **Construction** erects structures. Engineering handles genuine mechanical/system design.

Common Synergies include **Engineering + Mathematics**, **Engineering + Carpentry**, **Engineering + Blacksmithing**, **Engineering + Construction**, **Engineering + Disable Device**, **Engineering + Lock Picking**, and **Engineering + Trap Making**.

Exact machine statistics, power systems, build times, Quality, and Durability remain Crafting dependencies.

### Finance:
> **Status:** ✅ CONFIRMED — budgeting, cash flow, forecasting, and Merchant/Admin boundaries locked.

Finance governs tracking, forecasting, allocating, and evaluating money across households, projects, businesses, organizations, or investments.

- **Simple — Expense tracking:** Record and predict routine short-term expenditures for a small operation.
- **Basic — Income and budget:** Estimate ordinary income, create workable budgets, and compare expected versus actual cash flow.
- **Intermediate — Forecasting:** Anticipate seasonal changes, irregular costs, reserves, debt, and foreseeable events while maintaining a longer-term budget.
- **Advanced — Multi-operation finance:** Track and compare finances across several businesses, departments, projects, or revenue streams.
- **Master — Financial planning:** Build and manage complex budgets involving multiple organizations, long horizons, contingencies, capital allocation, and competing priorities.

**Merchant** negotiates transactions. **Administration** organizes broader operations. **Appraise** values individual goods/services.

Common Synergies include **Finance + Merchant**, **Finance + Administration**, **Finance + Mathematics**, and **Finance + Law** when legal structure materially affects finances.

Taxation, banking, interest, investments, and formal economy rules remain optional world/economy dependencies rather than assumed spreadsheet requirements.

### Geography:
> **Status:** ✅ CONFIRMED — environmental interpretation and Local Geography/Navigation boundaries locked.

Geography governs interpreting broad physical environments, landforms, vegetation patterns, water, climate relationships, and spatial environmental clues.

- **Simple — Obvious environmental cues:** Read clear signs such as vegetation concentration, drainage, slope, or terrain to make basic environmental inferences.
- **Basic — Resource inference:** Distinguish common environmental states and use terrain/vegetation evidence to infer likely water, shelter, or passable ground.
- **Intermediate — Regional pattern reading:** Interpret multiple environmental clues to identify likely vegetation zones, drainage paths, soil conditions, and resource areas.
- **Advanced — Landscape inference:** Reason from terrain, climate, vegetation, and landform relationships to locate likely fertile ground, water systems, passes, or other regional features.
- **Master — Sparse-evidence geography:** Build reliable regional conclusions from incomplete environmental evidence and infer likely relationships among water, terrain, vegetation, soils, climate, and settlement.

**Local Geography (Specified)** is memorized/familiar knowledge of a particular area. **Navigation** determines course and direction. **Cartography** creates or interprets maps.

Common Synergies include **Geography + Navigation**, **Geography + Cartography**, **Geography + Herbology**, **Geography + Geology**, **Geography + Meteorology**, and **Geography + Camping**.

Geography never locates an unseen resource with no supporting evidence merely because Training is high.

### Geology:
> **Status:** ✅ CONFIRMED — earth/stone interpretation, ore/gem prospect inference, and Prospecting boundary locked.

Geology governs identifying rocks, minerals, strata, deposits, land history, and geologic processes from observable evidence.

- **Simple — Common stone and mineral identification:** Recognize common rock, soil, and mineral types and obvious physical characteristics.
- **Basic — Uncommon materials:** Identify less familiar minerals, ores, sedimentary materials, and misleading look-alikes from appropriate examination.
- **Intermediate — Read geologic history:** Interpret exposed strata, core samples, formations, erosion, deposition, or deformation to infer changes over long periods.
- **Advanced — Ore inference:** Use formations and mineral indicators to identify likely locations and directions of metal-bearing deposits.
- **Master — Rare deposit inference:** Identify likely environments and formations for rare minerals or gemstones and distinguish promising evidence from superficial resemblance.

**Prospecting** physically locates, follows, and extracts deposits in the field. Geology provides scientific interpretation.

Common Synergies include **Geology + Prospecting**, **Geology + Geography**, **Geology + Mining/Construction activities where relevant**, **Geology + Masonry**, and **Geology + Metallurgy**.

### Heraldry:
> **Status:** ✅ CONFIRMED — symbols, noble houses, lineage, and institutional identity knowledge locked.

Heraldry governs recognizing, interpreting, researching, and correctly using coats of arms, crests, seals, insignia, lineage symbols, noble houses, and comparable formal identity systems.

- **Simple — Major symbols:** Recognize prominent current royal, governmental, military, or institutional marks.
- **Basic — Noble and regional heraldry:** Identify less prominent current houses, branches, offices, ranks, and common symbolic conventions.
- **Intermediate — Historical lineages:** Recall or research past houses, succession, alliances, cadet branches, obsolete symbols, and important changes.
- **Advanced — House character and politics:** Understand reputations, traditions, rivalries, obligations, and political relationships associated with known houses and institutions.
- **Master — Heraldic expertise:** Interpret obscure or partial heraldry, reconstruct likely identity from limited evidence, and address or appeal to noble/institutional traditions with exceptional precision.

Common Synergies include **Heraldry + History**, **Heraldry + Diplomacy**, **Heraldry + Counterfeiting**, **Heraldry + Researching**, and **Heraldry + Law**.

Heraldry supplies knowledge; it does not itself persuade a noble or authenticate an object beyond heraldic evidence.

### History:
> **Status:** ✅ CONFIRMED — historical knowledge/research progression with evidence boundary locked.

History governs knowledge and investigation of past events, periods, peoples, institutions, conflicts, artifacts, and historical context.

- **Simple — Familiar recent history:** Accurately recall widely known recent events from areas or communities reasonably familiar to the Specialist.
- **Basic — Broader documented history:** Recall established events, people, dates, and developments from studied regions or periods.
- **Intermediate — Focused historical investigation:** Research a specific event, object, place, or person using available sources and place findings in useful context.
- **Advanced — Critical historical analysis:** Compare conflicting sources, distinguish later interpretation from contemporary evidence, identify likely bias, and reconstruct complex historical sequences.
- **Master — Deep historical synthesis:** Connect obscure evidence across periods, recognize rare parallels, and reconstruct likely historical context from fragmentary but meaningful sources.

A Master historian does **not** know facts never learned, observed, preserved, or inferable. The legacy “recall without ever reading it” becomes expert inference and broad accumulated study rather than supernatural knowledge.

Common Synergies include **History + Researching**, **History + Archaeology**, **History + Heraldry**, **History + Law**, **History + Local Geography**, and **History + Writing**.

### Law:
> **Status:** ✅ CONFIRMED — legal research, interpretation, advocacy, and loophole analysis locked.

Law governs understanding, researching, interpreting, and arguing within formal legal systems the Specialist has studied or can investigate.

- **Simple — Legal research:** Locate relevant statutes, procedures, or precedents with sufficient time and usable sources.
- **Basic — Routine legal practice:** Research efficiently, understand ordinary procedure, and prepare a straightforward prosecution, defense, petition, contract, or legal argument.
- **Intermediate — Infer unfamiliar law:** Use observed institutions, enforcement, procedure, and related legal principles to make cautious inferences about an unfamiliar jurisdiction while continuing research.
- **Advanced — Complex advocacy:** Build sophisticated arguments from evidence, procedure, precedent, jurisdiction, and competing interpretations; identify weaknesses in an opposing case.
- **Master — Loopholes and exceptional interpretation:** Find obscure exceptions, conflicts, procedural routes, jurisdictional issues, and defensible loopholes within complex legal systems.

**Bluff** handles intentional falsehoods; **Public Speaking/Diplomacy** may govern delivery or negotiation; Law supplies legal substance.

Common Synergies include **Law + Researching**, **Law + Diplomacy**, **Law + Public Speaking**, **Law + History**, and **Law + Finance**.

Exact trial procedures and legal institutions are worldbuilding dependencies, not mandatory universal subsystems.

### Local Geography (Specified):
> **Status:** ✅ CONFIRMED — location-specific spatial familiarity locked.

Local Geography (Specified) represents deep familiarity with one defined place or region: roads, neighborhoods, landmarks, routes, resources, hidden places, local terrain, and practical spatial relationships.

- **Simple — Major features:** Find or give directions to major settlements, roads, waterways, districts, farms, and prominent landmarks in the specified area.
- **Basic — Ordinary local detail:** Locate particular businesses, buildings, minor landmarks, side roads, crossings, and commonly used routes.
- **Intermediate — Uncommon places:** Know forgotten paths, abandoned sites, caves, minor ruins, service routes, local shortcuts, and other places not obvious to visitors.
- **Advanced — Minute familiarity:** Locate obscure small features or navigate complicated portions of the area from memory with very little external reference.
- **Master — Intimate spatial knowledge:** Understand the specified area's practical layout with exceptional completeness, including relationships, shortcuts, overlooked connections, and likely access routes even when circumstances change.

This Skill is purchased separately for each specified area. **Geography** interprets general environments; **Navigation** determines course; **Local Geography** knows a particular place.

Common Synergies include **Local Geography + Navigation**, **Local Geography + Cartography**, **Local Geography + Merchant**, **Local Geography + History**, and **Local Geography + Smuggling**.

### Mathematics:
> **Status:** ✅ CONFIRMED — quantitative reasoning progression locked.

Mathematics governs formal calculation, quantitative reasoning, geometry, algebra, probability, measurement, and higher mathematical analysis.

- **Simple — Arithmetic:** Reliably perform addition, subtraction, ratios, and ordinary practical measurement.
- **Basic — Applied arithmetic:** Perform multiplication, division, percentages, proportions, conversions, and routine quantitative comparisons.
- **Intermediate — Algebraic reasoning:** Solve for unknowns, manipulate equations, model multi-step quantitative relationships, and work with practical probability or rates.
- **Advanced — Geometry and advanced calculation:** Work with formal geometry, trigonometric relationships where setting education supports them, complex order of operations, and multi-variable quantitative problems.
- **Master — Higher mathematics:** Use advanced mathematical frameworks such as calculus, linear algebra, sophisticated probability, optimization, or setting-equivalent higher mathematics.

Common Synergies include **Mathematics + Engineering**, **Mathematics + Finance**, **Mathematics + Cryptography**, **Mathematics + Architecture**, **Mathematics + Navigation**, and **Mathematics + Cartography**.

Routine calculations beneath meaningful uncertainty should not require rolls.

### Metallurgy:
> **Status:** ✅ CONFIRMED — metal identification, refining, and alloy design locked.

Metallurgy governs the composition, identification, smelting, refining, heat behavior, treatment, and alloying of metals and ores.

- **Simple — Common metals and ores:** Recognize common metallic ores and prepared metals and understand their ordinary properties.
- **Basic — Common refinement:** Smelt and refine common ores, remove ordinary impurities, and prepare usable metal stock with appropriate equipment.
- **Intermediate — Rare metals:** Identify uncommon or precious metals, their ores, characteristic impurities, and expected working properties.
- **Advanced — Advanced refining:** Smelt, separate, purify, and prepare difficult, rare, or high-value metals while controlling contamination and composition.
- **Master — Alloy design:** Combine compatible metals into purposeful alloys, adjust composition for desired properties, analyze unknown alloys, and reproduce sophisticated formulations when appropriate materials exist.

Metallurgy makes and understands the metal. **Blacksmithing**, **Armoring**, **Weapon Crafting**, **Jeweler**, and other crafts shape it into finished goods.

Common Synergies include **Metallurgy + Blacksmithing**, **Metallurgy + Armoring**, **Metallurgy + Weapon Crafting**, **Metallurgy + Jeweler**, **Metallurgy + Chemistry**, and **Metallurgy + Geology**.

Exact material statistics remain a Crafting/Materials dependency.

### Navigation:
> **Status:** ✅ CONFIRMED — course-finding, orientation, and Cartography/Local Geography boundaries locked.

Navigation governs determining direction, position, route, and course from landmarks, maps, celestial bodies, instruments, environmental cues, and accumulated travel information.

- **Simple — Major references:** Orient using obvious landmarks, known roads, major map features, or clear directional references.
- **Basic — Route finding:** Correlate less obvious landmarks with maps, choose practical routes, and recover from small course errors.
- **Intermediate — Solar navigation:** Use the sun, shadow, time, terrain, and ordinary environmental cues to establish direction and maintain a route.
- **Advanced — Celestial navigation:** Use stars, constellations, and other reliable night-sky references to determine direction and maintain longer courses.
- **Master — Minimal-input navigation:** Maintain or reconstruct a course from sparse, changing, or imperfect information by combining wind, movement, estimated travel, environmental cues, maps, and known references.

**Cartography** creates/analyzes maps. **Geography** interprets environments. **Local Geography** knows a place. Transportation operates the conveyance.

Common Synergies include **Navigation + Cartography**, **Navigation + Geography**, **Navigation + Local Geography**, **Navigation + Mathematics**, **Navigation + Meteorology**, and **Navigation + Transportation (Specified)**.

Exact long-distance travel and getting-lost procedures remain travel-system dependencies.

### Researching:
> **Status:** ✅ CONFIRMED — information retrieval/cross-reference progression and self-directed Learning Access role locked.

Researching governs locating, evaluating, cross-referencing, organizing, and reconstructing information from available records, testimony, archives, libraries, databases, collections, or setting-equivalent sources.

- **Simple — Direct sources:** Find useful sources whose titles, cataloging, or obvious subject directly match the question.
- **Basic — Indirect sources:** Locate relevant material through indexes, citations, related topics, authors, institutions, or contextual references.
- **Intermediate — Obscure-source discovery:** Trace information through sources that do not obviously advertise the subject, follow chains of references, and compare multiple accounts.
- **Advanced — Hidden or difficult information:** Find material buried in large collections, encoded or deliberately obscured references, restricted catalogs, fragmented archives, or unusual classification systems when access exists.
- **Master — Deep reconstruction:** Cross-reference obscure, damaged, contradictory, multilingual-known, or partially encoded sources to reconstruct a defensible body of information from fragments.

#### Self-directed Learning Access

With appropriate instructional resources and opportunity to practice, Researching may provide the **Learning Access** necessary to teach oneself a new Skill degree.

Researching does not directly grant the Skill or bypass XP/advancement costs. It answers whether the Specialist can assemble a viable course of self-study from the resources available.

Simple Training might be learned from good introductory manuals; advanced self-study normally requires correspondingly advanced, complete, and usable sources plus practical opportunity. A Researching check is needed only when the quality, completeness, access, or organization of those resources makes success genuinely uncertain.

Common Synergies include **Researching + Education**, **Researching + History**, **Researching + Law**, **Researching + Cryptography**, **Researching + Scribe**, and whatever domain Skill is being investigated.

Exact training-time and Education-discount rules remain an Advancement dependency.

### Smuggling:
> **Status:** ✅ CONFIRMED — concealment-and-transport identity and Hiding/Sleight boundaries locked.

Smuggling governs planning and executing the concealed transport of prohibited, sensitive, or unwanted cargo, creatures, or people through routes, inspections, borders, checkpoints, or security.

- **Simple — Small unobtrusive cargo:** Carry or place small contraband using ordinary concealment or social normalcy where inspection is light.
- **Basic — Purposeful concealment:** Hide small or moderate cargo in clothing, baggage, containers, vehicles, or loads so casual inspection is unlikely to reveal it.
- **Intermediate — Concealed passenger or large cargo:** Design hiding arrangements, routes, timing, paperwork, or load placement for people or large objects that must pass meaningful inspection.
- **Advanced — Layered smuggling operation:** Combine route knowledge, concealment, decoys, compartment use, timing, and security awareness to move conspicuous or difficult cargo through serious controls.
- **Master — Complex smuggling network:** Plan highly sophisticated movement of people or cargo across multiple security layers, routes, jurisdictions, or transfers while minimizing exposure.

**Sleight of Hand** conceals/manipulates objects immediately under personal control. **Hiding** conceals a creature by position. **Counterfeiting** creates false credentials/cargo identity.

Common Synergies include **Smuggling + Local Geography**, **Smuggling + Counterfeiting**, **Smuggling + Merchant**, **Smuggling + Hiding**, **Smuggling + Transportation (Specified)**, and **Smuggling + Administration** for large operations.

Security, inspection, legal, and economy details remain worldbuilding dependencies.

### Strategy:
> **Status:** ✅ CONFIRMED — military/competitive planning, unit coordination, and Leadership boundary locked.

Strategy governs analyzing objectives, terrain, forces, capabilities, information, logistics, and likely opposition to formulate plans for coordinated conflict.

- **Simple — Single-unit planning:** Track one unit or small force and make straightforward plans around its objective and capabilities.
- **Basic — Similar-unit coordination:** Coordinate several comparable units, account for positioning and mutual support, and plan basic reserves or contingencies.
- **Intermediate — Combined forces:** Plan operations involving several different unit types, capabilities, ranges, speeds, or roles.
- **Advanced — Operational strategy:** Exploit friendly and opposing strengths, weaknesses, terrain, timing, deception, supply, and objectives across a substantial engagement or campaign phase.
- **Master — Grand strategy:** Plan major operations for numerous varied forces, multiple fronts or objectives, long logistics chains, subordinate commanders, contingencies, and strategic consequences.

**Leadership** directs people in execution. **Administration** organizes resources and schedules. Strategy creates the conflict plan.

Common Synergies include **Strategy + Leadership**, **Strategy + Administration**, **Strategy + Geography**, **Strategy + Local Geography**, **Strategy + History**, and **Strategy + Engineering** for specialized capabilities.

Exact mass-combat, morale, supply, and army rules remain later dependencies and should not be assumed to require detailed bookkeeping.

## Agility

### Acrobatics:
> **Status:** ✅ CONFIRMED — Tumble consolidated into Acrobatics; movement/recovery identity and Balance/Jumping boundaries locked.

Acrobatics governs controlling the body through complex motion, rotation, inversion, rolls, flips, dives, controlled falls, momentum redirection, and recovery from disrupted movement.

- **Simple — Basic body control:** Perform cartwheels, handsprings, simple rolls, low-risk dives, and controlled transitions between standing and ground movement.
- **Basic — Controlled recovery:** Perform front flips and more demanding rolls, recover efficiently from ordinary stumbles or planned drops, and use a roll to reduce the disruption of manageable impacts.
- **Intermediate — Advanced movement:** Perform backflips, complex dives, rapid directional changes, and controlled tuck-and-roll recoveries after significant movement or a fall when physically possible.
- **Advanced — Chained acrobatics:** Link difficult flips, rolls, handsprings, vaults, and inversions while maintaining control; deliberately redirect momentum to reduce harm from severe but survivable impacts.
- **Master — Acrobatic mastery:** Perform exceptional gymnastic sequences, recover from extreme loss of orientation or footing when a physical recovery path exists, and maintain control through highly demanding movement.

#### Boundaries and Synergy

**Balance** maintains stability on precarious support. **Jumping** determines generated leap height/distance and precise landing placement. Acrobatics controls the body before, during, and after complex motion.

The former **Tumble** Skill is fully absorbed here.

Common Synergies include **Acrobatics + Balance**, **Acrobatics + Jumping**, **Acrobatics + Escape**, **Acrobatics + Swimming** for genuinely acrobatic underwater movement, and combat applications allowed by the integrated Skill maneuver rules.

Acrobatics does not negate physically unavoidable impact or allow impossible midair corrections. Exact fall-damage interaction remains a Combat/Movement dependency.

### Balance:
> **Status:** ✅ CONFIRMED — precarious-support stability identity locked.

Balance governs maintaining or recovering stability when footing, support, load distribution, or the supporting surface itself makes remaining upright uncertain.

- **Simple — Narrow footing:** Stand or move across support somewhat narrower than an ordinary stance under calm conditions.
- **Basic — Foot-width support:** Stand reliably on support roughly as narrow as the Specialist's foot and move carefully across modest instability.
- **Intermediate — Moving on narrow support:** Walk, turn, crouch, or perform ordinary tasks on foot-width or comparably precarious surfaces.
- **Advanced — Extremely narrow/unstable support:** Move across very narrow, shifting, vibrating, sloped, or otherwise difficult support while controlling carried weight.
- **Master — Exceptional balance:** Maintain useful stability on extraordinarily narrow or unstable support when the surface can physically bear the Specialist and there remains a plausible contact path.

**Acrobatics** handles complex motion/recovery; Balance handles sustained stability. Common Synergies include **Balance + Acrobatics**, **Balance + Climbing**, **Balance + Transportation (Specified)** for unusual conveyances, and **Balance + Dancing** where difficult footing materially affects performance.

### Dancing:
> **Status:** ✅ CONFIRMED — learned dance, partnered movement, and improvisational performance locked.

Dancing governs rhythmic patterned movement performed alone or with partners, including learned forms, leading/following, transitions, and improvisation.

- **Simple — Basic steps:** Follow simple measured steps or a familiar basic dance alone.
- **Basic — Partnered form:** Follow or perform established partnered steps with someone who understands the same form.
- **Intermediate — Varied sequences:** Combine multiple learned movements smoothly, transition between figures, and maintain timing without constant prompting.
- **Advanced — Partner adaptation:** Lead or follow through complex partnered movement, adapt to variations, and maintain form through unexpected changes.
- **Master — Improvisational dance:** Create and lead coherent spontaneous sequences, guide less-trained partners, and adapt movement fluidly to music, space, and other dancers.

Common Synergies include **Dancing + Musical Instrument**, **Dancing + Singing**, **Dancing + Acting**, **Dancing + Balance**, and **Dancing + Local Culture** for culturally specific forms.

Dancing does not replace Acrobatics merely because a performance contains difficult athletic movement.

### Hiding:
> **Status:** ✅ CONFIRMED — positional concealment kept distinct from Camouflage and Sneaking.

Hiding governs concealing oneself through position, cover, line of sight, silhouette, timing, and use of existing surroundings.

- **Simple — Full cover:** Hide behind or within obvious cover large enough to conceal the Specialist under ordinary observation.
- **Basic — Partial/congruent concealment:** Use shadows, clutter, terrain, furniture, vegetation, or similarly favorable surroundings to reduce exposure where substantial concealment exists.
- **Intermediate — Tight concealment:** Hide using cover somewhat smaller than the Specialist, awkward geometry, partial visual obstruction, or carefully chosen angles.
- **Advanced — Difficult visual concealment:** Use limited cover, mismatched surroundings, timing, silhouette control, and observer sight lines to remain difficult to locate.
- **Master — Minimal-cover concealment:** Exploit exceptional positioning, visual clutter, observer attention, and environmental geometry to remain unseen with very little conventional cover when a plausible visual concealment path exists.

#### Boundaries and Synergy

**Camouflage** changes the visual appearance of a creature, object, or position to blend with surroundings. **Hiding** chooses and uses concealment. **Sneaking** moves without being detected.

Common Synergies include **Hiding + Camouflage**, **Hiding + Sneaking**, **Hiding + Local Geography**, and **Hiding + Smuggling** when concealing a person during transport.

Hiding cannot make a visible creature literally invisible or conceal someone in an empty, fully observed space without some plausible obstruction, distraction, visual blending, or other mechanism.

Hiding is commonly opposed by **Spot** or **Search**, depending on whether the observer is rapidly noticing or deliberately examining.

### Sneaking:
> **Status:** ✅ CONFIRMED — stealthy movement, detection opposition, and cautious-speed model locked.

Sneaking governs moving while minimizing sound, visibility, and other immediately observable movement cues.

- **Simple — Cautious quiet movement:** Move slowly while controlling obvious footfall, equipment noise, and sudden motion.
- **Basic — Concealed movement:** Coordinate route, timing, cover, and noise to remain difficult to detect while moving through favorable conditions.
- **Intermediate — Efficient stealth:** Move through moderately difficult terrain or around ordinary observers while managing sound and visual exposure without constant stops.
- **Advanced — High-pressure stealth:** Maintain stealth through difficult surfaces, changing observer positions, sparse cover, or other unfavorable conditions while continuing to make progress.
- **Master — Stealth at practical pace:** Move with exceptional control through complex environments and, under reasonable conditions, maintain effective stealth at ordinary walking pace without automatically treating the attempt as Hasty.

#### Movement pace

The default Sneaking pace is **approximately half normal Movement** because careful foot placement, timing, route choice, and equipment control take time.

A Specialist may use **Hasty Sneaking** to cover the same distance in half that time—approximately normal walking pace for ordinary Sneaking—but takes the normal Hasty penalty for the task tier.

Master Training can support ordinary walking pace without Hasty when conditions are reasonable; running, sprinting, or unusually difficult stealth movement still requires appropriate rules and circumstances.

#### Boundaries and Synergy

Hiding is stationary/positional concealment. Camouflage changes visual appearance. Sneaking is movement.

Sneaking may be opposed by **Listening**, **Spot**, or another relevant sense depending on how detection is possible.

Common Synergies include **Sneaking + Hiding**, **Sneaking + Camouflage**, **Sneaking + Balance**, and **Sneaking + Local Geography** where route familiarity materially helps.

Exact combat movement interaction remains part of the Movement/Combat pass.

### Transportation (Specified):
> **Status:** ✅ CONFIRMED — consolidates Boating, Sailing, Skating, Skiing, and Teamster; governed by Agility; related-mode Limited Substitution locked.

Transportation (Specified) governs operating **one chosen non-riding mode of transportation** whose control depends on the Specialist's input, balance, steering, handling, or maneuvering.

Examples include **Skis, Skates, Canoe/Rowboat, Sailboat, Wagon/Carriage, Sled**, larger sailing vessels, and other setting-appropriate conveyances. Each specification is purchased separately.

- **Simple — Basic operation:** Start, mount/board, steer, stop, or propel the specified mode under favorable, ordinary conditions with appropriate equipment.
- **Basic — Routine control:** Maintain direction and speed, manage ordinary loads or passengers, perform common turns and stops, and operate through routine environmental variation.
- **Intermediate — Difficult handling:** Control the conveyance against moderate current, slope, poor surface, traffic, uneven terrain, wind, or other meaningful handling complications.
- **Advanced — Hazardous maneuvering:** Operate through strong currents, rapids, difficult routes, tight spaces, high speeds, rough seas, steep descents, or comparable hazards appropriate to the specified mode.
- **Master — Exceptional operation:** Extract reliable performance from the specified conveyance under extreme but physically survivable conditions, use very limited favorable input effectively, and perform highly precise or demanding maneuvers.

#### Related-mode Limited Substitution

Training in one Transportation specification grants competency with **closely related modes using substantially similar controls and handling principles at one degree lower**:
- Simple provides no substitution.
- Basic provides Simple.
- Intermediate provides Basic.
- Advanced provides Intermediate.
- Master provides Advanced.

Actual Training in the related specification supersedes substitution.

A canoe may transfer meaningfully to another small oared craft; wagon to cart; ice skates to a sufficiently similar skate type. Skating does not substitute for sailing merely because both are Transportation.

#### Boundaries and Synergy

**Riding** governs being mounted on and directing a creature. Transportation governs non-riding conveyances.

For animal-drawn vehicles, Transportation governs the vehicle, route, braking, turning, load, and handling. **Animal Handling** may provide Synergy when directing the draft animals materially matters.

Large sailing craft commonly support Synergy with **Rope Use**, **Navigation**, **Meteorology**, **Leadership**, or **Engineering** depending on the task.

Transportation is governed by **Agility** because its central competency is controlling a moving conveyance. Stamina still matters through Fatigue/exertion where appropriate.

Exact vehicle statistics, speeds, collisions, crew requirements, and travel rules remain later dependencies.

### Ventriloquism:
> **Status:** ✅ CONFIRMED — concealed articulation and voice-source illusion locked.

Ventriloquism governs speaking with minimized visible articulation and manipulating timing, direction, resonance, and visual coordination to make speech appear to originate from another source.

- **Simple — Minimal lip movement:** Speak intelligibly while substantially reducing obvious mouth movement.
- **Basic — Coordinated prop speech:** Operate a simple puppet or moving prop while coordinating speech convincingly enough to create a basic talking-object illusion.
- **Intermediate — Timed source illusion:** Match speech to another object's visible movement, conceal articulation reliably, and create convincing source ambiguity at short range.
- **Advanced — Throw the voice:** Manipulate acoustic and visual cues to make speech appear to come from another nearby location when the environment permits the illusion.
- **Master — Live movement synchronization:** Anticipate and coordinate with another creature's visible mouth or body movement closely enough to create the appearance that the creature is producing the Specialist's words under plausible viewing conditions.

Common Synergies include **Ventriloquism + Acting**, **Ventriloquism + Mimicry**, **Ventriloquism + Bluff**, and **Ventriloquism + Listening** where acoustics materially matter.

Ventriloquism does not literally relocate sound or override physics. Distance, echoes, observer position, acoustics, and visibility determine difficulty.

## Looks

### Camouflage:
> **Status:** ✅ CONFIRMED — visual blending kept distinct from Hiding and Sneaking.

Camouflage governs altering the visible appearance of a creature, object, equipment, or position so that it blends with its surroundings or breaks up recognizable shape.

- **Simple — Basic environmental coloring:** Apply simple paints, coverings, or material chosen to resemble a familiar environment and reduce obvious visual contrast.
- **Basic — Prepared camouflage:** Treat clothing, fabric, equipment, or carried gear so color and pattern better match a particular environment.
- **Intermediate — Object and position camouflage:** Camouflage larger objects, equipment, hides, camps, or positions by combining color, texture, outline disruption, and local materials.
- **Advanced — Rapid adaptation:** Modify or replace camouflage efficiently when moving between environments and account for changing light, season, terrain, and viewing direction.
- **Master — Integrated concealment treatment:** Camouflage creatures, equipment, positions, or sizeable objects with exceptional attention to color, texture, silhouette, shadow, and environmental context so they are extremely difficult to distinguish at appropriate distance.

#### Boundaries and Synergy

**Hiding** chooses and uses a concealed position. **Sneaking** moves stealthily. Camouflage changes what the subject visually looks like.

Common Synergies include **Camouflage + Hiding**, **Camouflage + Hunting**, **Camouflage + Sneaking**, **Camouflage + Artistry**, and **Camouflage + Local Geography** where environmental familiarity matters.

Camouflage does not make a subject invisible. Distance, movement, lighting, observer angle, and environmental mismatch remain meaningful.

### Disguise:
> **Status:** ✅ CONFIRMED — physical appearance alteration and Acting/Mimicry boundaries locked.

Disguise governs using clothing, cosmetics, prosthetics, hair, posture aids, padding, and other physical means to alter how a creature appears.

- **Simple — Minor appearance change:** Alter apparent age, grooming, complexion, hair, or other surface traits enough to look noticeably different at a glance.
- **Basic — Conceal identity:** Change several recognizable features so casual observers have difficulty identifying the Specialist as themselves.
- **Intermediate — General resemblance:** Make the Specialist resemble a particular person, profession, social type, ancestry presentation, or role well enough to survive casual comparison.
- **Advanced — Specific impersonation appearance:** Reproduce the visible features of a particular individual closely enough to fool observers with moderate familiarity when tools, materials, and anatomy permit it.
- **Master — High-fidelity disguise:** Create an exceptionally convincing visible likeness capable of surviving close visual scrutiny by very familiar observers when the physical differences can plausibly be bridged.

Disguise changes appearance only. **Acting** supplies behavior and personality; **Mimicry** supplies voice and mannerisms; **Bluff** supplies false claims.

Common Synergies include **Disguise + Acting**, **Disguise + Mimicry**, **Disguise + Bluff**, **Disguise + Counterfeiting** for supporting credentials or costume details, and **Disguise + Sewing** for specialized garments.

Disguise cannot overcome impossible anatomical differences without appropriate prosthetics, magic, Traits, or equipment.

### Panhandling:
> **Status:** ✅ CONFIRMED — solicitation-through-sympathy identity and deception boundary locked.

Panhandling governs soliciting voluntary charity by presenting need, choosing receptive audiences, reading reactions, and framing requests effectively.

- **Simple — Direct solicitation:** Ask openly for small charity and present an obvious need without sophisticated technique.
- **Basic — Presentation of need:** Choose clothing, posture, location, timing, and visible circumstances that make a genuine or represented need easier to understand.
- **Intermediate — Audience reading:** Identify people or crowds more likely to respond and tailor the request toward hunger, injury, misfortune, family need, travel hardship, or another plausible appeal.
- **Advanced — Compelling appeal:** Build a persuasive personal narrative, adjust it to observed reactions, and work a difficult or mixed crowd without losing credibility.
- **Master — Exceptional solicitation:** Turn minimal opportunity into effective voluntary charity through timing, presentation, social awareness, and compelling storytelling, even when the visible circumstances are not immediately sympathetic.

If the Specialist deliberately fabricates material facts, **Bluff** may become Primary or provide Synergy. **Acting** may support a performed condition. **Empathy** may support reading the audience.

Panhandling does not compel charity and does not create resources where none are available.

### Seduction:
> **Status:** ✅ CONFIRMED — renamed from Sex Appeal; attraction, flirtation, and autonomy boundaries locked.

Seduction governs recognizing possible attraction and deliberately presenting oneself, flirting, building romantic or sexual tension, and pursuing consensual intimate interest.

- **Simple — Read obvious interest:** Recognize clear signs of attraction or receptiveness and respond without obvious social missteps.
- **Basic — Flirtation:** Use conversation, attention, presentation, humor, and body language to express interest and test whether it is reciprocated.
- **Intermediate — Build rapport and attraction:** Sustain a mutually receptive interaction, adapt to the other person's preferences and signals, and create a stronger sense of intimacy or romantic interest.
- **Advanced — Difficult social circumstances:** Navigate mixed signals, rivalry, awkward settings, status differences, or prior emotional complications when genuine attraction remains possible.
- **Master — Exceptional romantic social skill:** Read subtle reciprocal interest and cultivate strong consensual attraction through highly effective timing, confidence, presentation, and interpersonal awareness.

#### Boundary

Seduction **cannot manufacture attraction that fundamentally does not exist**, override sexual or romantic orientation, compel consent, erase another creature's commitments or values, or force intimate behavior.

A successful check represents effective pursuit **within the target's actual range of possible interest**.

Common Synergies include **Seduction + Empathy**, **Seduction + Acting** where deliberate presentation matters, **Seduction + Bluff** only when actual deception is involved, **Seduction + Dancing**, and **Seduction + Local Culture** where courtship customs materially matter.

## Insight

### Archaeology:
> **Status:** ✅ CONFIRMED — excavation/recovery, context preservation, and restoration boundaries locked.

Archaeology governs locating, exposing, documenting, recovering, stabilizing, and interpreting material remains of past people, settlements, structures, and events without needlessly destroying their context.

- **Simple — Basic recovery:** Expose and recover robust objects or obvious ruins with elementary care and recognize when further digging risks damage.
- **Basic — Controlled excavation:** Use appropriate tools, layers, grids, notes, and handling methods to recover ordinary artifacts while preserving useful context.
- **Intermediate — Delicate excavation:** Recover fragile, buried, collapsed, waterlogged, or tightly packed material with minimal additional damage and distinguish meaningful layers or associations.
- **Advanced — Stabilization and reconstruction:** Stabilize recovered objects or structures and reconstruct damaged material when sufficient surviving evidence or comparable examples exist.
- **Master — Complex recovery:** Plan and execute difficult excavations in hazardous, unusual, deeply buried, collapsed, submerged, or otherwise challenging environments while preserving artifacts, structure, and contextual evidence as far as physically possible.

**History** supplies historical context; **Geology** interprets earth layers; **Researching** finds records; **Masonry/Construction** may support structural stabilization.

Common Synergies include **Archaeology + History**, **Archaeology + Geology**, **Archaeology + Researching**, **Archaeology + Search**, and **Archaeology + Architecture/Masonry** where ruins materially require them.

Artifact deterioration, restoration materials, site hazards, and archaeological project times remain later world/crafting dependencies.

### Artistry:
> **Status:** ✅ CONFIRMED — visual composition and fine-art execution identity locked.

Artistry governs creating visual art through composition, proportion, color, form, texture, representation, abstraction, and aesthetic judgment across suitable media.

- **Simple — Basic expression:** Create recognizable simple drawings, paintings, models, or decorative designs using familiar media.
- **Basic — Controlled technique:** Use ordinary artistic tools and media deliberately, produce balanced compositions, and create competent paintings, drawings, clay work, or comparable art.
- **Intermediate — Lifelike or expressive work:** Produce convincing representation, controlled perspective, anatomy, light, texture, or deliberate stylization and emotional visual effect.
- **Advanced — Difficult media and sophisticated composition:** Work with delicate, expensive, unforgiving, or multi-stage media and sustain complex visual design.
- **Master — Artistic mastery:** Create exceptional original works with sophisticated composition, technique, expression, and control across the Specialist's practiced media.

Material-specific craft Skills still govern their technical construction. Artistry may support **Jeweler, Wood Carving, Sewing, Leatherworking, Calligraphy, Camouflage, Counterfeiting**, and other crafts where visual design materially matters.

Artistry does not automatically determine market value; **Appraise** does.

### Cooking:
> **Status:** ✅ CONFIRMED — food preparation, preservation, menu construction, and scale progression locked.

Cooking governs preparing safe, palatable, and intentionally designed food and meals from available ingredients.

- **Simple — Basic safe preparation:** Clean, portion, heat, and prepare straightforward food so it is edible and safely cooked under ordinary conditions.
- **Basic — Seasoning and ordinary dishes:** Use common spices, fats, sauces, and techniques to improve flavor and prepare familiar complete dishes.
- **Intermediate — Ingredient combination:** Build balanced dishes from available ingredients, substitute sensibly, control texture and timing, and coordinate several components.
- **Advanced — Refined cuisine:** Execute difficult techniques, precise timing, advanced seasoning, presentation, and multi-component meals for discerning diners.
- **Master — Large or exceptional service:** Design and execute complex multi-course meals or high-volume service while coordinating timing, variety, dietary needs, presentation, and consistency.

Common Synergies include **Cooking + Herbology** for edible/culinary plants, **Cooking + Hunting/Fishing** for unusual ingredients, **Cooking + Apothecary** where medicinal food genuinely overlaps, and **Cooking + Administration** for major kitchens.

Food spoilage, nutrition, long-term preservation, and meal-based recovery bonuses remain optional survival/world dependencies.

### Empathy:
> **Status:** ✅ CONFIRMED — emotion-reading identity and deception/social support role locked.

Empathy governs reading emotional state, tension, comfort, fear, enthusiasm, reluctance, and interpersonal reaction from expression, posture, tone, behavior, and context.

- **Simple — Strong emotions:** Identify obvious emotional states such as anger, fear, joy, grief, or panic when they are strongly expressed.
- **Basic — Moderate emotion:** Read less intense states and distinguish broad mixtures such as nervous excitement, resentment, discomfort, or guarded interest.
- **Intermediate — Subtle or concealed emotion:** Detect muted, mixed, or deliberately restrained emotional cues when enough behavior is observable.
- **Advanced — Familiar-person nuance:** Read minute deviations, habitual tells, and subtle emotional changes in people the Specialist knows well.
- **Master — Stranger-level nuance:** Build a careful emotional read of unfamiliar people from very subtle but meaningful cues without assuming knowledge the evidence cannot support.

Empathy reads emotion; it is **not automatic lie detection** and does not reveal thoughts.

Common Synergies include **Empathy + Questioning**, **Empathy + Diplomacy**, **Empathy + Leadership**, **Empathy + Seduction**, **Empathy + Intimidate**, **Empathy + Acting**, and **Empathy + Animal Handling** only where creature behavior is sufficiently analogous and the Keeper agrees.

Bluff or Acting may oppose Empathy when deliberately masking relevant cues.

### Medicine:
> **Status:** ✅ CONFIRMED — renamed from First Aid; direct patient care, diagnosis, treatment, and surgery identity locked.

Medicine governs assessing injury or illness and directly treating a patient through stabilization, wound care, splinting, diagnosis, procedures, surgery, and recovery management.

- **Simple — Immediate first aid:** Clean and bandage ordinary wounds, control straightforward bleeding, recognize obvious urgent danger, and provide basic stabilization.
- **Basic — Routine treatment:** Apply prepared medicines appropriately, treat common minor injuries or illnesses, monitor recovery, and recognize when a condition exceeds the Specialist's capability.
- **Intermediate — Musculoskeletal and trauma care:** Set simple fractures or dislocations where appropriate, improvise or apply splints, manage significant wounds, and distinguish common complications.
- **Advanced — Advanced diagnosis and procedures:** Evaluate complex injury or illness, perform demanding treatment, manage infection risk, and undertake invasive procedures within the setting's medical capability.
- **Master — Surgery and comprehensive care:** Perform major surgery and sophisticated treatment, coordinate recovery from severe disease or trauma, and use appropriate medicines to restore health to the limits allowed by the Health system.

#### Boundaries and Synergy

**Apothecary** creates medicine; Medicine uses it on a patient. **Alchemy** handles genuinely supernatural restoration. **Poisons** handles toxicology.

Common Synergies include **Medicine + Apothecary**, **Medicine + Poisons**, **Medicine + Chemistry**, **Medicine + Anatomy-related knowledge if later introduced**, and **Medicine + Empathy** where patient communication materially matters.

Medicine does not regrow limbs or perform impossible regeneration without an explicit supernatural source.

Exact Vitality restoration, surgery risk, disease, infection, recovery time, and medical Conditions remain Health-system dependencies.

### Animal Handling:
> **Status:** ✅ CONFIRMED — absorbs Falconry; individual-animal handling/training identity and animal-skill Limited Substitution locked.

Animal Handling governs reading, approaching, calming, directing, conditioning, and training **individual animals or small working groups**, including birds of prey and other specialized trained animals.

- **Simple — Trained animal handling:** Safely approach and direct a well-trained familiar animal using commands it already knows.
- **Basic — Difficult trained animals:** Handle moderately trained, distracted, stressed, or unfamiliar animals and issue more demanding known commands.
- **Intermediate — Begin training:** Establish workable control with an untrained but trainable animal, introduce simple commands, and shape basic behavior through repeated practice.
- **Advanced — Complex training:** Teach moderately complex behaviors, chained commands, specialized work, or task-specific routines to suitable animals.
- **Master — Wild or exceptional training:** Establish a working relationship with wild, highly difficult, or unusually specialized animals and teach complex behavior when the creature is physically and mentally capable of learning it.

The former **Falconry** Skill is fully absorbed here.

#### Animal-skill boundaries

**Animal Handling** trains and directs individual animals.
**Riding** governs remaining mounted on and directing a rideable creature while actually riding it.
**Animal Husbandry** governs long-term care, breeding, health, feeding, and population management.

#### Limited Substitution

Training in one of these three animal Skills may provide **Simple Limited Substitution** into another when the task is a narrow, ordinary overlap rather than the other Skill's defining specialty.

Examples:
- Animal Handling may provide Simple Riding for a familiar, well-trained mount under calm conditions.
- Riding may provide Simple Animal Handling for ordinary mount commands from the ground.
- Animal Husbandry may provide Simple Animal Handling for routine care or movement of domesticated stock.
- Animal Handling may provide Simple Animal Husbandry for immediate ordinary care of a familiar individual animal.

Actual Training always supersedes substitution.

Common Synergies include **Animal Handling + Riding**, **Animal Handling + Animal Husbandry**, **Animal Handling + Transportation (Specified)** for animal-drawn vehicles, and **Animal Handling + Hunting** for trained hunting animals.

Exact training times, animal intelligence, morale, and command limits remain creature/training dependencies.

### Housekeeping:
> **Status:** ✅ CONFIRMED — maintenance, cleaning, organization, and household-staff coordination locked.

Housekeeping governs cleaning, organizing, maintaining, stocking, and operating lived-in spaces and their routine domestic systems.

- **Simple — Routine cleaning:** Dust, sweep, mop, wash, dispose of ordinary refuse, and perform basic tidying.
- **Basic — Everyday organization:** Return obviously misplaced items, maintain simple storage systems, track ordinary household supplies, and establish routine cleaning schedules.
- **Intermediate — Property maintenance:** Clean and maintain a medium residence or workspace efficiently or coordinate a small household staff.
- **Advanced — Complex organization:** Restore order to badly disorganized spaces, design sensible storage/workflow, manage delicate furnishings, and coordinate several domestic functions.
- **Master — Large-estate operation:** Maintain or oversee substantial portions of large estates, institutions, inns, or comparable properties while directing staff, schedules, supplies, standards, and recurring maintenance.

**Administration** may support large staffs and scheduling; **Finance** may support household budgets; **Cooking**, **Sewing**, or other domestic crafts remain separate.

Housekeeping should stay light mechanically unless a campaign actually cares about estate or household operation.

### Lip Reading:
> **Status:** ✅ CONFIRMED — visual speech interpretation and unknown-language sound-reproduction boundary locked.

Lip Reading governs interpreting visible speech from mouth shape, tongue position, throat movement, facial motion, and contextual cues when sound cannot be heard clearly.

- **Simple — Isolated familiar words:** Identify many clearly articulated familiar words from one visible speaker under good conditions.
- **Basic — Connected speech:** Recover most ordinary words from a clearly visible speaker or a small number of speakers when context is available.
- **Intermediate — Fine articulation analysis:** Use lips, tongue, jaw, throat, and surrounding facial movement to distinguish ambiguous sounds and improve accuracy.
- **Advanced — Conversation reading:** Follow most of a visible conversation among several speakers when sight lines, language familiarity, and pacing permit it.
- **Master — Phonetic reconstruction:** Reconstruct likely spoken sounds from unfamiliar speech patterns and reproduce them approximately even without knowing the language.

Master Lip Reading does **not** confer comprehension of an unknown language. It may allow the Specialist to repeat what was likely said for someone else who understands it.

Common Synergies include **Lip Reading + Mimicry**, **Lip Reading + Local Culture/language knowledge**, **Lip Reading + Spot**, and **Lip Reading + Questioning** when observing a conversation covertly.

Distance, visibility, facial obstruction, accents, speed, and language familiarity determine difficulty.

### Local Culture (Specified):
> **Status:** ✅ CONFIRMED — area-specific customs, ritual, etiquette, and cultural transfer boundary locked.

Local Culture (Specified) represents familiarity with the customs, rituals, social expectations, taboos, traditions, everyday etiquette, and communal practices of one defined culture or region.

- **Simple — Public customs:** Follow ordinary visible customs and avoid obvious everyday breaches.
- **Basic — Minor rituals:** Participate correctly in common ceremonies, hospitality practices, greetings, meals, mourning, celebration, and other routine social forms.
- **Intermediate — Cultural guidance:** Explain expected behavior, correct ordinary mistakes, and recognize when a situation carries social meaning outsiders may miss.
- **Advanced — Anticipate expectations:** Predict likely etiquette or ritual expectations in unfamiliar situations within the culture and instruct others reliably.
- **Master — Related-culture transfer:** Recognize structural similarities in related cultures and cautiously infer likely customs outside the specified area without treating them as identical.

Each culture/region is a separate specification.

Common Synergies include **Local Culture + Diplomacy**, **Local Culture + Seduction**, **Local Culture + Merchant**, **Local Culture + Dancing**, **Local Culture + Heraldry**, and **Local Culture + Public Speaking** where cultural form materially matters.

### Meteorology:
> **Status:** ✅ CONFIRMED — weather observation and forecasting progression locked.

Meteorology governs interpreting atmospheric conditions, seasonal patterns, clouds, wind, pressure signs, moisture, temperature trends, and other evidence to understand or forecast weather.

- **Simple — Obvious weather signs:** Distinguish common cloud and weather types and identify clear signs of imminent ordinary rain, wind, or temperature change.
- **Basic — Storm movement:** Determine general direction, speed, and likely local arrival of visible weather systems.
- **Intermediate — Short-term forecast:** Combine cloud development, wind, humidity, season, pressure signs, and local patterns to predict likely changes over the near term.
- **Advanced — Subtle-pattern forecast:** Read weak or conflicting indicators, recognize unusual developments, and make useful forecasts farther ahead or under difficult conditions.
- **Master — Expert weather sense:** Rapidly synthesize very subtle atmospheric evidence and established patterns to anticipate significant change before it becomes obvious.

Meteorology is evidence-based; Master Training is not supernatural precognition.

Common Synergies include **Meteorology + Geography**, **Meteorology + Navigation**, **Meteorology + Camping**, **Meteorology + Transportation (Specified)** for vessels or exposed travel, and **Meteorology + Farming**.

Exact storm severity, environmental hazards, and forecast horizons remain travel/world dependencies.

### Questioning:
> **Status:** ✅ CONFIRMED — combines legacy Question and Interrogation into one information-elicitation Skill.

Questioning governs obtaining information from other people through deliberate inquiry, conversational structure, rapport, discretion, contradiction, pressure, and selection of the right person or topic.

- **Simple — Direct inquiry:** Ask clear questions, gather straightforward information from cooperative people, and keep the conversation focused on the desired subject.
- **Basic — Sensitive questioning:** Recognize touchy subjects, phrase questions tactfully or discreetly, and avoid unnecessarily closing off a cooperative source.
- **Intermediate — Source and inconsistency recognition:** Identify who is likely to know useful information, establish conversational baselines, and recognize obvious evasion, contradiction, or gaps.
- **Advanced — Resistant subjects:** Structure follow-up questions, revisit details, compare answers, shift between rapport and pressure, and adapt to guarded or deliberately deceptive subjects.
- **Master — Complex elicitation:** Conduct extended, subtle, or high-stakes questioning across multiple people or information threads while managing rapport, pressure, corroboration, secrecy, and the actual objective.

#### Boundaries and Synergy

Questioning covers both ordinary interviews and what the legacy rules called **Interrogation**; setting and motivation change the difficulty and supporting Skills rather than creating a separate Skill.

**Empathy** reads emotional reaction. **Bluff** supports deceptive questioning. **Intimidate** supports threats. **Torture** may support coercive suffering. **Researching** supplies facts used to test answers.

Common Synergies include **Questioning + Empathy**, **Questioning + Researching**, **Questioning + Bluff**, **Questioning + Intimidate**, **Questioning + Diplomacy**, and situational **Questioning + Torture**.

A successful Questioning check does not guarantee that a source's statement is true; corroboration still matters.

### Riding:
> **Status:** ✅ CONFIRMED — broad rideable-creature scope, command-capability boundary, and animal-skill Limited Substitution locked.

Riding governs remaining mounted on and directing a **creature physically capable of carrying the Specialist as a rider and capable of receiving or responding to rider input or commands**.

The creature need not be an ordinary living animal. Undead, constructs, magically animated creatures, or other unusual mounts may be rideable if their design, training, binding, intelligence, control system, or magic actually allows them to respond to a rider. If a creature can carry the Specialist but has no means of receiving or acting on commands, Riding may help the Specialist **remain mounted**, but it does not create a control channel that does not exist.

- **Simple — Trained mount:** Ride a well-trained familiar mount under ordinary conditions and issue simple commands it already knows.
- **Basic — Active riding:** Control speed, direction, stopping, starting, ordinary obstacles, and more demanding known commands on a trained mount.
- **Intermediate — Difficult or unfamiliar mount:** Remain mounted and maintain control on a poorly trained, unfamiliar, agitated, or unusual creature when it is willing or able to accept rider direction.
- **Advanced — Hazardous riding:** Control a suitable mount through combat, difficult terrain, high speed, jumps, abrupt maneuvers, or other dangerous circumstances.
- **Master — Exceptional mounted control:** Ride highly difficult, exotic, wild-trained, flying, climbing, aquatic, or otherwise unusual mounts and coordinate complex mounted maneuvers when the creature's anatomy and control capability make them possible.

#### Boundaries and Synergy

**Animal Handling** trains and directs individual animals generally. **Riding** governs mounted control. **Animal Husbandry** governs long-term care and breeding. Non-creature conveyances use **Transportation (Specified)**.

The confirmed Simple Limited Substitution among Riding, Animal Handling, and Animal Husbandry applies only to narrow ordinary overlaps; actual Training supersedes it.

Common Synergies include **Riding + Animal Handling**, **Riding + Animal Husbandry**, **Riding + Balance**, **Riding + Acrobatics**, and **Riding + Combat Skills/Martial rules** where mounted combat is explicitly supported.

Mounted combat, mount actions, creature morale, and unusual control interfaces remain later dependencies.

### Search:
> **Status:** ✅ CONFIRMED — deliberate examination kept distinct from rapid Spot.

Search governs deliberately examining an area, object, container, structure, or scene to locate hidden, concealed, unusual, valuable, dangerous, or out-of-place details.

- **Simple — Obvious anomalies:** Find large, poorly concealed, obviously displaced, or conspicuous details when deliberately looking.
- **Basic — Basic hidden features:** Find ordinary concealed compartments, obvious trap triggers, intentionally hidden small objects, or straightforward irregularities.
- **Intermediate — Well-hidden evidence:** Locate secret doors, moderately concealed objects, subtle tampering, layered hiding places, or careful but imperfect concealment.
- **Advanced — Expert concealment:** Find cleverly hidden traps, mechanisms, caches, tracks, tampering, or evidence designed to withstand deliberate inspection.
- **Master — Minute inconsistency:** Detect extremely subtle physical irregularities, misplaced objects, blending artifacts, construction discrepancies, or other meaningful details from thorough examination.

**Spot** is rapid visual noticing; **Search** is deliberate investigation.

Common Synergies include **Search + Spot**, **Search + Listening**, **Search + Engineering**, **Search + Trap Making**, **Search + Archaeology**, and **Search + Counterfeiting** when authenticity clues are being examined.

Search requires time and access. Meticulous use is especially natural; large spaces may use extended checks.

### Tracking:
> **Status:** ✅ CONFIRMED — sign-following progression with strict evidence boundary locked.

Tracking governs detecting, interpreting, and following physical or environmental signs left by moving creatures, vehicles, or groups.

- **Simple — Fresh obvious trail:** Follow clear recent signs such as footprints in snow, cart ruts in mud, broken vegetation, blood, or disturbed debris.
- **Basic — Careful target:** Follow fresher but less obvious signs left by a target that moved cautiously or through less receptive terrain.
- **Intermediate — Aged or intermittent trail:** Reconstruct a route from older, partial, scattered, or periodically lost signs.
- **Advanced — Degraded trail:** Follow subtle signs despite weather, changing surfaces, deliberate concealment, traffic, or environmental disruption when meaningful evidence survives.
- **Master — Minute-trace reconstruction:** Detect and connect extremely small or widely separated surviving signs and infer likely movement between them.

#### Evidence boundary

Tracking never follows a trail from **no evidence at all**. Age alone does not make a trail possible or impossible; what matters is whether meaningful traces survived.

Common Synergies include **Tracking + Hunting**, **Tracking + Listening**, **Tracking + Search**, **Tracking + Geography**, **Tracking + Local Geography**, and **Tracking + Meteorology** when weather materially affects the trail.

The former **Trapping** Skill is removed. Choosing where to place animal traps based on prey behavior belongs to **Hunting**; constructing and calibrating the trap belongs to **Trap Making**.

## Stamina

### Construction:
> **Status:** ✅ CONFIRMED — full progression developed; structure-execution identity and Architecture/Engineering/material-craft boundaries locked.

Construction governs turning plans, materials, labor, sequencing, and site conditions into completed **structures**. It represents the practical execution and coordination of building work rather than the design of the building or the fabrication of every component.

- **Simple — Basic assembly:** Execute straightforward structural work from clear plans or established practice: prepare a simple site, lay out work, assemble basic framing or supports, and coordinate a small build using ready materials.
- **Basic — Conventional structure:** Sequence ordinary foundations, framing, enclosure, access, roofing, and finishing work; recognize obvious build-order problems; and coordinate several trades on a modest project.
- **Intermediate — Complex build coordination:** Manage larger crews, multiple material systems, staging, temporary supports, difficult sequencing, and changes in site conditions while keeping the project aligned with plans.
- **Advanced — Difficult construction:** Execute unusual structures, difficult sites, large spans, substantial heights, constrained access, major renovations, or builds requiring close coordination among several specialist crafts and engineered systems.
- **Master — Major project execution:** Plan the practical build sequence and coordinate materials, labor, temporary works, logistics, specialist trades, contingencies, and site conditions for exceptionally large or complex structures.

#### Boundaries and Synergy

**Architecture** designs the building and produces plans. **Engineering** designs or understands specialized structural/mechanical systems. **Construction** turns the design into a physical structure.

**Carpentry, Masonry, Blacksmithing, Armoring, Sewing, Rope Use**, and other crafts make or install components when their specific expertise is required.

Common Synergies include **Construction + Architecture**, **Construction + Engineering**, **Construction + Carpentry**, **Construction + Masonry**, **Construction + Administration**, **Construction + Mathematics**, and material-specific crafts.

Construction is **not** a universal “roll once to build a castle” Skill. Large builds should be staged projects whose interesting decisions depend on the final Crafting/Construction framework.

Exact labor productivity, material quantities, build time, structural Quality, Durability, costs, and failure consequences remain major Crafting dependencies. These should be designed for table usefulness rather than simulation bookkeeping.

### Animal Husbandry:
> **Status:** ✅ CONFIRMED — long-term animal care, breeding, population management, and animal-skill Limited Substitution locked.

Animal Husbandry governs long-term care and management of domesticated or managed animal populations: feeding, shelter, breeding, health observation, lifecycle planning, population balance, and routine herd/flock maintenance.

- **Simple — Small-group care:** Feed, water, shelter, clean, monitor, and maintain a small familiar group of ordinary animals.
- **Basic — Breeding and routine management:** Manage breeding, births, basic population replacement, routine health observation, and care of a moderately sized group.
- **Intermediate — Multiple related groups:** Maintain several similar groups or species while balancing feed, shelter, breeding cycles, space, sanitation, and common health concerns.
- **Advanced — Mixed-stock management:** Manage several substantially different animal populations with different needs, breeding patterns, housing, diets, and uses.
- **Master — Complex population stewardship:** Sustain and deliberately manage diverse large animal populations over generations while balancing genetics, productivity, health, resources, environment, and long-term population stability.

**Animal Handling** works with individual animals; **Riding** handles mounted use.

The confirmed **Simple Limited Substitution** among Animal Husbandry, Animal Handling, and Riding applies only to narrow ordinary overlaps. Actual Training supersedes substitution.

Common Synergies include **Animal Husbandry + Animal Handling**, **Animal Husbandry + Riding**, **Animal Husbandry + Medicine** where animal health care overlaps, **Animal Husbandry + Farming** for mixed agricultural operations, and **Animal Husbandry + Administration** for large facilities.

Exact breeding timelines, animal disease, feed economics, and population accounting are optional world dependencies and should remain abstract unless the campaign actually needs them.

### Climbing:
> **Status:** ✅ CONFIRMED — body-on-surface movement identity and Rope Use boundary locked.

Climbing governs ascending, descending, traversing, and maintaining position on steep or vertical surfaces using natural holds, body technique, and climbing equipment.

- **Simple — Abundant holds:** Climb surfaces with frequent secure handholds and footholds under ordinary conditions.
- **Basic — Protected climbing:** Use ordinary climbing equipment, anchors, pitons, harnesses, or prepared lines to climb straightforward non-overhanging surfaces safely.
- **Intermediate — Sparse holds:** Climb surfaces with limited natural holds, awkward body positions, exposure, or moderate technical difficulty, with or without suitable equipment.
- **Advanced — Sheer technical climbing:** Ascend or traverse very steep, sheer, smooth, fragile, or otherwise difficult surfaces using appropriate tools and advanced movement technique.
- **Master — Extreme climbing:** Climb overhangs, complex faces, unusual structures, or exceptionally demanding routes when physically viable holds, friction, equipment, or anchors exist.

#### Boundary with Rope Use

**Climbing** governs the Specialist's body movement and placement on the surface. **Rope Use** designs, ties, tensions, anchors, and manages rope systems.

Climbing retains the legacy ability to **set up ordinary climbing protection and use pitons** as part of the climbing task. Sophisticated anchor networks, hauling systems, rescue rigging, multi-rope systems, or complex tension management belong to Rope Use.

Common Synergies include **Climbing + Rope Use**, **Climbing + Balance**, **Climbing + Acrobatics**, and **Climbing + Geography/Local Geography** where route reading materially contributes.

Climbing does not permit scaling a truly featureless surface without friction, tools, magic, Traits, or another plausible physical mechanism.

### Farming:
> **Status:** ✅ CONFIRMED — absorbs Gardening; plant cultivation from garden scale through field agriculture locked.

Farming governs cultivating useful plants through soil preparation, planting, propagation, irrigation, pruning, weeding, pest management, harvest, crop rotation, and long-term soil care. The former **Gardening** Skill is fully absorbed here.

- **Simple — Hardy plants and harvest:** Recognize ordinary ripeness, harvest straightforward crops, plant and maintain very hardy garden or field plants, and perform routine watering/weeding.
- **Basic — Routine cultivation:** Grow common food or utility plants reliably, use ordinary hand tools or agricultural equipment, manage planting depth/spacing, and handle conventional harvest methods.
- **Intermediate — Crop health and irrigation:** Manage irrigation, soil condition, pruning, pests, disease signs, seasonal timing, and moderately delicate fruits, vegetables, flowers, or field crops.
- **Advanced — Difficult cultivation:** Grow demanding or fragile plants and maintain production in poor soil, difficult terrain, marginal climate, limited water, or other unfavorable but survivable conditions.
- **Master — Agricultural systems:** Plan crop rotation, soil recovery, planting density, mixed cultivation, seasonal succession, and land use for long-term productivity; establish highly delicate crops where environmental conditions can be made suitable.

#### Boundaries and Synergy

Farming governs **plants**, not the entire operation of a farm as an organization.

**Animal Husbandry** governs livestock. **Administration** governs workers, schedules, inventories, and organization. **Finance** governs budgets. **Herbology** identifies plants and natural properties.

Common Synergies include **Farming + Herbology**, **Farming + Meteorology**, **Farming + Geography**, **Farming + Animal Husbandry** for mixed agricultural systems, **Farming + Administration**, and **Farming + Chemistry/Apothecary** where soil treatments or plant preparations genuinely matter.

Farming does **not** grant Limited Substitution into Animal Husbandry merely because both occur on farms.

Exact crop yields, seasons, acreage, food economics, and soil simulation are later world dependencies and should remain abstract unless gameplay makes them relevant.

### Prospecting:
> **Status:** ✅ CONFIRMED — deposit locating/extraction identity and Geology/Explosives boundaries locked.

Prospecting governs locating, exposing, following, and extracting useful mineral, ore, and gem deposits in the field using practical mining judgment and excavation tools.

- **Simple — Basic extraction:** Safely break and recover accessible ore or mineral-bearing material from exposed rock using ordinary hand tools.
- **Basic — Assisted excavation:** Use standard excavation equipment and correctly employ already-prepared blasting charges or other excavation aids when another Skill/system has supplied them.
- **Intermediate — Follow a deposit:** Expose and follow veins or concentrations of useful minerals while choosing practical excavation direction and minimizing needless loss.
- **Advanced — Delicate extraction:** Recover fragile or high-value crystals, gems, or complex deposits while reducing breakage and preserving useful material.
- **Master — Difficult-field extraction:** Continue useful excavation with limited, improvised, or damaged tools and interpret the working face well enough to pursue valuable deposits under difficult conditions.

**Geology** predicts and interprets deposits. Prospecting physically finds/follows/extracts them. **Explosives** creates, places, and controls explosive charges; Prospecting does not.

Common Synergies include **Prospecting + Geology**, **Prospecting + Explosives**, **Prospecting + Engineering**, **Prospecting + Construction**, and **Prospecting + Metallurgy** when ore quality materially matters.

Mining hazards, extraction rates, deposit values, and material yields remain world/Crafting dependencies.

### Swimming:
> **Status:** ✅ CONFIRMED — absorbs Aquabatics; flotation, propulsion, diving, maneuvering, and advanced aquatic body control locked.

Swimming governs keeping oneself afloat and moving, diving, turning, orienting, maneuvering, and controlling the body in water. The former **Aquabatics** Skill is fully absorbed here.

- **Simple — Stay afloat:** Tread water, float intentionally, recover to the surface in calm conditions, and move short distances with elementary strokes.
- **Basic — Practical swimming:** Swim reliably through calm water, control breathing, enter and exit the water safely, tow or carry small loads when physically reasonable, and perform ordinary turns or dives.
- **Intermediate — Efficient aquatic movement:** Sustain useful travel, maneuver underwater, dive with control, change orientation quickly, and swim through moderate current, waves, or restricted water.
- **Advanced — Difficult water:** Remain functional in turbulent water, strong current, surf, significant waves, or other hazardous aquatic conditions while preserving direction and breath control.
- **Master — Aquatic mastery:** Swim at a strong practical pace, maneuver precisely above or below water, perform complex turns/rolls/dives, and make progress against difficult current when physical strength and conditions permit it.

**Acrobatics + Swimming** may provide Synergy for genuinely acrobatic underwater performances, but ordinary aquatic rolls, dives, turns, and orientation belong to Swimming itself.

Common Synergies include **Swimming + Endurance/health rules where relevant**, **Swimming + Acrobatics**, **Swimming + Medicine** for water rescue, **Swimming + Rope Use** for aquatic rescue rigging, and **Swimming + Transportation (Specified)** around small craft.

Exact swim speed, breath holding, drowning, currents, armor penalties, and aquatic combat remain Movement/Health dependencies.

## Toughness

### Armoring:
> **Status:** ✅ CONFIRMED — consolidates Armor Smithing and Leather Armoring; material-agnostic protective-equipment craft locked.

Armoring governs designing, fitting, assembling, repairing, reinforcing, and modifying worn protective equipment whose primary purpose is reducing harm. It is **material-agnostic**: metal, leather, hide, bone, chitin, shell, wood, stone, layered cloth, composite construction, and setting-specific materials may all be used when their physical properties make them viable.

- **Simple — Maintenance and repair:** Inspect, maintain, patch, refit, replace straightforward components, and repair uncomplicated damage to familiar armor constructions.
- **Basic — Conventional armor construction:** Assemble and fit established armor designs from prepared components and suitable materials, including straightforward rigid, flexible, layered, or segmented protection.
- **Intermediate — Complex protection:** Construct fitted armor requiring multiple material layers, articulation, overlapping pieces, shaped components, reinforced joints, or specialized distribution of protective coverage.
- **Advanced — Specialized armor:** Modify or build armor for unusual anatomy, environments, movement requirements, damage threats, or material combinations while preserving mobility and protection.
- **Master — Original armor design:** Design and construct new complex protective systems from suitable materials, integrating articulation, weight distribution, coverage, reinforcement, fastening, and unusual physical properties within the Crafting rules.

#### Boundaries and Synergy

Armoring owns the **protective design and assembly** of armor. It does not automatically grant mastery of every material process used to create its components.

Common Synergies include:
- **Armoring + Blacksmithing** for difficult forged metal components.
- **Armoring + Leatherworking** for shaped, hardened, layered, or fitted leather components.
- **Armoring + Sewing** for textile, padded, quilted, or layered cloth construction.
- **Armoring + Wood Carving/Carpentry** for specialized wooden plates, laminates, or fittings.
- **Armoring + Metallurgy** for unusual alloys.
- **Armoring + Jeweler** for fine articulated fittings where genuinely relevant.
- **Armoring + Anatomy/creature knowledge** where later rules support unusual bodies.

The former **Armor Smithing** and **Leather Armoring** Skills are removed and fully consolidated here.

Exact armor dice, mitigation, encumbrance, material statistics, Quality, Durability, repair, and exotic-material rules remain major Armor/Crafting dependencies.

### Blacksmithing:
> **Status:** ✅ CONFIRMED — general forged-metal goods craft kept distinct from Metallurgy, Armoring, and Weapon Crafting.

Blacksmithing governs heating, forging, drawing, bending, upsetting, punching, drifting, welding, quenching, grinding, filing, and finishing metal into practical non-specialist objects and components.

- **Simple — Basic metal handling:** Pour or work prepared metal in simple molds, straighten or reshape uncomplicated pieces, and perform routine maintenance on basic forged goods.
- **Basic — Simple forged tools:** Produce straightforward hooks, nails, tongs, brackets, hinges, straps, spikes, and other common functional metal pieces from prepared stock.
- **Intermediate — Refined functional work:** Cut, grind, file, polish, join, fit, and finish durable tools or components requiring controlled shape and reliable dimensions.
- **Advanced — Stock and complex forms:** Draw, flatten, taper, bend, forge-weld, and prepare sheet, bar, round stock, complex fittings, and demanding tool shapes for further use.
- **Master — Advanced forging:** Design and forge exceptionally strong or complex practical metal objects, control heat treatment and quenching appropriately, and solve unusual fabrication problems within the properties of available metal.

**Metallurgy** makes, refines, and understands the metal. Blacksmithing shapes it.

**Armoring** owns armor design/construction. **Weapon Crafting** owns weapons. Blacksmithing may provide Synergy where difficult forged components materially contribute.

Common Synergies include **Blacksmithing + Metallurgy**, **Blacksmithing + Armoring**, **Blacksmithing + Weapon Crafting**, **Blacksmithing + Engineering**, **Blacksmithing + Farrier**, and **Blacksmithing + Construction**.

Material properties, tool Quality, heat-treatment bonuses, Durability, and work times remain Crafting dependencies.

### Farrier:
> **Status:** ✅ CONFIRMED — corrected legacy name from Furrier; hoof care and shoeing craft locked.

Farrier governs maintaining the hooves of suitable working or riding creatures and manufacturing, fitting, adjusting, applying, and removing protective shoes or comparable hoof fittings.

- **Simple — Routine shoe handling:** Safely remove and replace an ordinary properly fitted shoe on a cooperative familiar animal and perform basic hoof cleaning.
- **Basic — Nails and ordinary fit:** Prepare or shape suitable nails/fittings, recognize obvious poor fit or wear, and make modest adjustments to standard shoes.
- **Intermediate — Corrective modification:** Trim and balance ordinary hooves within the Farrier's scope, modify existing shoes for fit, wear, terrain, or minor conformational needs, and recognize problems requiring medical attention.
- **Advanced — Forge specialized shoes:** Produce shoes or hoof fittings from appropriate material for particular animals, terrain, work, injury accommodation, or unusual hoof shapes.
- **Master — Comprehensive farriery:** Design, forge, fit, and maintain highly specialized hoof protection for unusual mounts, heavy workloads, difficult terrain, or exceptional anatomy when the creature's feet can physically accept such treatment.

The legacy heading **Furrier** was a naming error; its entire content described farriery.

Common Synergies include **Farrier + Blacksmithing**, **Farrier + Animal Handling**, **Farrier + Animal Husbandry**, **Farrier + Riding**, and **Farrier + Medicine** when hoof injury or pathology genuinely overlaps.

Farrier is not full veterinary Medicine.

### Jumping:
> **Status:** ✅ CONFIRMED — leap generation/placement identity and Acrobatics boundary locked.

Jumping governs generating and controlling deliberate leaps: takeoff, height, distance, trajectory, clearing obstacles, and landing placement.

- **Simple — Running long jump:** Perform controlled horizontal leaps with a run-up and ordinary landing area.
- **Basic — Running high/obstacle jump:** Convert a run-up into vertical clearance or clear substantial ordinary obstacles while maintaining a planned landing.
- **Intermediate — Standing long jump:** Generate meaningful horizontal distance without a run-up and control the landing within a useful area.
- **Advanced — Standing high jump and difficult descent:** Generate demanding vertical leaps from limited setup and use deliberate landing technique to reduce harm from intentional drops where a survivable physical landing exists.
- **Master — Precision jumping:** Aim for and land on very small viable targets, combine difficult height/distance with placement, and adapt takeoff or landing to unusual geometry when the jump itself is physically achievable.

**Acrobatics** governs complex body movement and recovery; Jumping governs the leap itself. **Balance** may govern remaining stable after landing on precarious support.

Common Synergies include **Jumping + Acrobatics**, **Jumping + Balance**, **Jumping + Climbing**, and combat applications under the integrated Skill maneuver rules.

Exact jump distance/height formulas, Size effects, intentional-fall mitigation, and movement costs remain Movement/Combat dependencies.

### Masonry:
> **Status:** ✅ CONFIRMED — stone/brick/mortar craft identity and Construction/Architecture boundaries locked.

Masonry governs selecting, shaping, laying, joining, repairing, and assessing stone, brick, block, mortar, concrete-like setting materials, and comparable mineral construction systems.

- **Simple — Basic masonry repair:** Mix ordinary mortar or binder, reset loose units, patch straightforward damage, and construct simple low walls, hearths, or foundations from prepared material.
- **Basic — Conventional masonry:** Lay brick, block, or dressed stone to line, level, and bond; build ordinary walls, floors, steps, piers, arches from established patterns, and maintain consistent joints.
- **Intermediate — Structural masonry:** Build and repair substantial load-bearing walls, foundations, retaining structures, vaults, chimneys, and mixed masonry systems while identifying obvious structural weakness.
- **Advanced — Difficult stonework:** Shape and place large or irregular stone, execute demanding arches/vaults, repair historic or damaged masonry, and work on complex structural forms.
- **Master — Advanced masonry construction:** Design the practical masonry execution of exceptionally complex stone/brick systems, fit difficult pieces, reconstruct unusual work from surviving evidence, and identify subtle material or load-path problems within the Masonry domain.

**Construction** coordinates the whole structure. **Architecture** designs the building. **Engineering** handles specialized structural/mechanical analysis beyond masonry craft.

Common Synergies include **Masonry + Construction**, **Masonry + Architecture**, **Masonry + Engineering**, **Masonry + Geology**, and **Masonry + Mathematics**.

The legacy Masonry ability to build entire huts/cabins is narrowed: those structures may involve Masonry, but whole-building execution belongs to Construction.

Exact structural strength, mortar curing, material Quality, and project time remain Crafting dependencies.

### Weapon Crafting:
> **Status:** ✅ CONFIRMED — renamed and broadened from Weapon Smithing; material-agnostic conventional weapon craft locked.

Weapon Crafting governs designing, constructing, repairing, balancing, modifying, and finishing **conventional weapons** from suitable materials. It is not limited to metal.

Viable materials may include metal, wood, stone, bone, horn, chitin, shell, composite laminates, and setting-specific materials where their physical properties support the intended weapon.

- **Simple — Maintenance and basic components:** Inspect, sharpen, straighten, haft, bind, regrip, rebalance, and repair straightforward damage to familiar weapons; produce very simple weapon components from prepared material.
- **Basic — Conventional weapon construction:** Construct established simple weapons from suitable prepared materials, fit heads/blades/hafts/handles, and reproduce ordinary designs reliably.
- **Intermediate — Complex weapons and material integration:** Construct multi-component weapons requiring precise fit, balance, reinforcement, shaping, and combination of several materials.
- **Advanced — Specialized weapons:** Modify or build weapons for unusual anatomy, fighting style, reach, target, environment, delivery requirement, or material property while preserving safe function.
- **Master — Original weapon design:** Design and prototype new conventional weapons or highly unusual variants, balancing geometry, mass distribution, grip, durability, reach, striking/cutting function, and material limits within the Martial/Crafting rules.

#### Boundaries and Synergy

The former **Weapon Smithing** Skill is renamed because the craft is no longer metal-only.

**Bowyer** remains the specialist craft for bows and crossbows. **Fletching** remains the specialist craft for arrows, bolts, and related shafted ammunition. Weapon Crafting does **not** absorb either.

**Blacksmithing** may forge difficult metal components. **Metallurgy** handles alloys. **Wood Carving/Carpentry** may support specialized wooden components. Other material crafts may support unusual weapons.

Common Synergies include **Weapon Crafting + Blacksmithing**, **Weapon Crafting + Metallurgy**, **Weapon Crafting + Wood Carving/Carpentry**, **Weapon Crafting + Jeweler** for fine mechanisms/fittings where relevant, **Weapon Crafting + Engineering** for unusual mechanical weapon systems, and **Weapon Crafting + Armoring** when paired design considerations genuinely matter.

Exact weapon profiles, Quality, Durability, material effects, balance bonuses, and crafting costs remain Martial/Crafting dependencies.
