# Daggerforged Design Specification

Daggerforged is an additive asset pack that brings Daggerheart's character system into the Sundered Isles rules engine. The goal: play something that feels like Daggerheart—class identity, ancestry, community, domain abilities, progression—while Sundered Isles handles all the underlying mechanics.

This document is the working spec. It is designed to give enough context to execute conversion work without relitigating design decisions.

---

## Source Material

Both repositories are canonical. Don't invent or approximate when source text is available.

- Daggerheart SRD: [github.com/seansbox/daggerheart-srd](https://github.com/seansbox/daggerheart-srd)
- Sundered Isles / Starforged dataforged: [github.com/tbsvttr/datasworn](https://github.com/tbsvttr/datasworn)

---

## Core Premise

Sundered Isles is the rules engine. Daggerheart is the character content system.

SI rules stay untouched: action rolls, momentum, oracles, progress tracks, clocks, bonds, harm. All of it works exactly as written.

Most Daggerheart mechanics get dropped: Hope/Fear duality dice, Stress, Hit Points, Armor, damage thresholds, the leveling system. SI already handles what these mechanics do.

Hope survives as a spendable resource, but with a new earning trigger tied to SI's action roll (details below). This lets Daggerheart abilities that cost Hope work as written.

The Loadout/Vault system survives in spirit. Domain abilities use a 5-ability active loadout with momentum-based recall, adapting Daggerheart's Stress-based recall to SI's economy.

What survives from Daggerheart is character *identity*: who a character is, what they can do, how they feel to play. Class names, subclass names, ancestry names, community names, domain card names—all preserved as closely as possible. A Daggerheart player should recognize their character in Daggerforged immediately.

---

## Additive Design

Daggerforged is additive, not replacement. No SI content is removed or modified.

Groups wanting pure fantasy can use Daggerforged assets and ignore nautical/ship content. Groups wanting nautical fantasy can use Daggerforged alongside the full SI ship system. Nothing needs to be stripped out. Unused content just goes unused.

---

## Sundered Isles Assets: Coexistence

Standard SI assets (Paths, Companions, Deeds, etc.) aren't removed, but they're not the primary character-building tool in Daggerforged.

Daggerforged assets are primary. Players build from the Daggerforged pool. That's the expected default.

Standard SI assets are supplemental. The full SI pool remains available as opt-in. If a player finds an SI asset that fits their concept and doesn't conflict with their Daggerforged assets, they can take it. When conflicts exist, Daggerforged takes precedence.


---

## Character Creation

A starting Daggerforged character takes five assets:

| Asset | Source | Abilities at Start |
|---|---|---|
| Ancestry | Daggerheart ancestry | 2 (both features, always active) |
| Community | Daggerheart community | 1 (always active) |
| Class | Daggerheart class | 2 (Hope Feature + Class Feature, always active) |
| Subclass | Daggerheart subclass | 1 (Foundation only) |
| Domain (×2) | Daggerheart domains | 2 total (player's choice from level 1 abilities across both domains) |

This gives a starting character 8 active abilities. That's higher than a standard SI character (usually 4), but the cognitive load stays manageable:

- Ancestry, Community, and Class abilities are static. They don't change or expand. Many are passive or simple triggers rather than active decisions.
- The Domain asset has many abilities printed on it, but only 2 are active at start. The rest are visible future progression, not current decisions.
- Real active decision count at the table is closer to 3-4, comparable to standard SI play.

When designing Ancestry and Community assets, prefer passive effects and simple triggers over complex active abilities. Active decision weight should concentrate in Class, Subclass, and Domain assets where players expect it.

### Class Domain Access

Each class grants access to two domains:

- Bard: Grace & Codex
- Druid: Arcana & Sage
- Guardian: Blade & Valor
- Ranger: Bone & Sage
- Rogue: Grace & Midnight
- Seraph: Splendor & Valor
- Sorcerer: Arcana & Midnight
- Warrior: Blade & Bone
- Wizard: Codex & Splendor

When selecting domain abilities (at character creation and when spending XP), players choose from either of their class's two domains. The 5-ability loadout limit applies across both domains combined, not per domain.

---

## Asset Types

### Ancestry Asset

Each Daggerheart ancestry becomes an Ancestry asset.

- Ability 1: top ancestry feature, unlocked at character creation
- Ability 2: bottom ancestry feature, unlocked at character creation

Both abilities start unlocked and remain the only abilities on the asset. Ancestry features are static from character creation with no further progression.

Mixed ancestry is supported. Declare a mixed ancestry and take Ability 1 from one Ancestry asset and Ability 2 from a different one. You can't take both abilities from the same ancestry when playing mixed.

---

### Community Asset

Each Daggerheart community becomes a Community asset.

- Ability 1: core community feature, unlocked at character creation

The single ability starts unlocked and remains the only ability on the asset. Community features are static from character creation with no further progression.

---

### Class Asset

Each Daggerheart class becomes a Class asset containing the abilities that define the class at its broadest level:

- Hope Feature: costs Hope to activate (see Hope section)
- Class Feature(s): one or more features that define the class's core identity

All abilities are unlocked at character creation. Most classes have one Hope Feature and one Class Feature, but some (Druid, Rogue, Sorcerer, Warrior, Wizard) have multiple Class Features that are all converted and available from the start.

The Class asset also contains the Hope track (0-6), used to fuel Hope Features and other abilities that cost Hope.

---

### Subclass Asset

Each Daggerheart subclass becomes a Subclass asset with three sequentially gated abilities. Each ability represents a tier and bundles all features gained at that tier into a single text block. This keeps every subclass on a standard 3-ability card regardless of how many individual features exist at each tier.

- Ability 1 (Foundation): unlocked at character creation. Contains all Foundation features.
- Ability 2 (Specialization): XP unlock, requires Ability 1. Contains all Specialization features.
- Ability 3 (Mastery): XP unlock, requires Ability 2. Contains all Mastery features.

Sequential gating is enforced. Ability 2 can't be taken before Ability 1, and Ability 3 can't be taken before Ability 2. This recreates Daggerheart's Foundation/Specialization/Mastery progression using native SI XP mechanics.

When a tier has multiple features, they are all gained simultaneously when that tier is unlocked. The bundled format makes this explicit — unlocking Specialization gives you everything in the Specialization text block, not individual features to cherry-pick.


---

### Domain Asset

Domain assets are the most complex and most important part of Daggerforged. They closely mirror how domain cards work in Daggerheart, adapted into SI terms.

#### Structure

Each domain (Arcana, Blade, Bone, Codex, Grace, Midnight, Sage, Splendor, Valor) is its own Domain asset. A Domain asset contains all abilities from that domain, printed in full. Each ability has a level requirement (1-10)—a player can't unlock an ability above their current tier.

Each domain has around 21 abilities spread across levels 1-10, with 2-3 options at each level. Players don't unlock all of them. They choose which abilities to purchase as they progress, just as Daggerheart players choose one card per level from available options.

A character has access to the two Domain assets corresponding to their class's domains (e.g., a Warrior has access to Blade and Bone).

#### Tier Tracking

The Domain asset includes a Tier track (1-10). When a player spends 3 XP to advance a tier, they mark the next tier box and immediately unlock one domain ability of their choice at that tier level (included in the 3 XP cost). If a character has two Domain assets, they share the same tier—mark both when advancing.

This mirrors how SI assets work: spending 3 XP for a new asset includes the first ability. Advancing a tier is like "buying" access to that tier's abilities, with one ability included.

#### Loadout Limit

A player may have a maximum of 5 domain abilities active at any time across all domains. This is the loadout. All other unlocked abilities are in the vault.

- Swapping at rest: players may freely rearrange their active 5 abilities when they make camp or equivalent rest.
- Swapping mid-session: a player may swap a vaulted ability into their active loadout by paying the ability's Recall Cost in momentum (1:1 conversion from Daggerheart's Stress-based Recall Cost). The Recall Cost for each ability is defined on the asset.

Starting characters begin at Tier 1 with 2 active domain abilities of their choice from the level 1 abilities available in their class's domains.

---

## Progression

Daggerforged uses the standard SI experience system with one addition: tiers.

### Earning Experience

Earn 2 XP each time you fill a legacy box (4 ticks) on any legacy track—Quests, Bonds, or Discoveries. Unchanged from standard SI.

### Tiers

Daggerforged characters have a tier (1-10) that determines which domain abilities they can purchase. A Tier 1 character can only buy level 1 domain abilities. A Tier 5 character can buy level 1-5 abilities. And so on.

All characters start at Tier 1. Advancing to the next tier costs 3 XP and includes one domain ability at that tier (player's choice). Tier is tracked on the Domain asset(s).

### Spending Experience

| Purchase | Cost | Notes |
|----------|------|-------|
| Advance one tier | 3 XP | Includes one domain ability at that tier |
| Unlock additional domain ability (at or below your tier) | 2 XP | Beyond the one included with tier advance |
| Unlock Subclass Specialization | 2 XP | Requires Foundation |
| Unlock Subclass Mastery | 2 XP | Requires Specialization |

Standard SI purchases remain available:

| Purchase | Cost |
|----------|------|
| Add a new SI asset (Companion, Path, Deed, etc.) | 3 XP |
| Upgrade an SI asset | 2 XP |

### Progression Math

A character who fills all 30 legacy boxes (maximum progression) earns 60 XP. If they spend it on Daggerforged progression:

- Tiers 2-10: 27 XP (9 advances × 3 XP, each including one domain ability = 9 abilities)
- Starting domain abilities: 2 (free at character creation)
- Subclass Specialization + Mastery: 4 XP
- Total: 31 XP for full Daggerforged progression (11 domain abilities + full subclass)

This leaves 29 XP surplus for personal expression:
- Additional domain abilities (2 XP each)—adds vault options, still limited to 5 active
- Multiclassing (6+ XP for new Class + Subclass)
- SI assets (Companions, Deeds, Paths, vehicles)

The 5-ability loadout limit keeps cognitive load manageable regardless of how many domain abilities are unlocked. A fully progressed Daggerforged character has around 13 active abilities (8 from Ancestry/Community/Class/Subclass + 5 from domain loadout), compared to 20-24 for a typical max-level SI character. The surplus XP lets Daggerforged characters approach SI parity if desired, or invest in vault depth and flexibility.

### Multiclassing

A character may take a second class at Tier 5 or higher. To multiclass:

- Spend 3 XP to acquire a new Class asset (gain its Class Feature; the Hope Feature is not gained)
- Spend 3 XP to acquire a Subclass asset from the new class (Foundation unlocked)
- Gain access to one of the new class's domains

Domain abilities from the multiclass domain are unlocked at half your current tier (rounded up). The 5-ability loadout limit applies across all domains.


---

## Hope

Daggerheart uses Hope as a spendable resource that fuels class features, domain abilities, and other special effects. Daggerforged preserves Hope but changes how it's earned to integrate with SI's action roll system.

### The Hope Track

Every Daggerforged character has a Hope track on their Class asset card, ranging from 0 to 6.

- Starting Hope: Begin your first session with 2 Hope.
- Carrying Hope: Hope carries over between sessions. It doesn't reset unless something in the fiction would cause it to reset.

### Earning Hope

Hope is earned on both action rolls and progress rolls.

On an action roll, look at your action die (the d6):

- Action die shows 4, 5, or 6 → Gain +1 Hope (max 6)
- Action die shows 1, 2, or 3 → No Hope gained

This check happens on every action roll, independent of the outcome. You might roll a miss and still gain Hope. You might roll a strong hit and not gain Hope.

On a progress roll, use the number of filled progress boxes as your "action die" value:

- 6+ boxes filled → Gain +1 Hope (max 6)
- 5 or fewer boxes filled → No Hope gained

This rewards patience and proper pacing. Players who invest in a progress track before attempting to resolve it are more likely to earn Hope. It also ties Hope generation to meaningful narrative moments: completing vows, finishing fights, deepening connections.

Bonus Hope on matched strong hits: When you roll a strong hit with a match on any roll (action or progress), gain +2 Hope instead of +1. Matches are rare, and this windfall reflects the moment when everything aligns perfectly.

Hope is not earned on oracle rolls or other non-action, non-progress roll types.

### Hope Economy Projections

Pre-release analysis of 22 Sundered Isles sessions across 6 players provides baseline projections. These numbers are theoretical—actual Daggerforged play will differ because players will be spending Hope, which these sessions didn't account for.

Projected Hope Generation:

| Source | Per Session | Notes |
|--------|-------------|-------|
| Action rolls (4+ on d6) | ~4.6 | 59% of action dice showed 4+ |
| Progress rolls (6+ boxes) | ~0.9 | 95% of progress rolls had 4+ boxes |
| Match bonus | ~0.1 | Rare but memorable |
| Total | ~5.7 | |

Session Variance: Generation ranged from 1 Hope (unlucky dice) to 12 Hope (many rolls + lucky) across analyzed sessions. This variance is desirable—players can't always count on Hope being available, making spending decisions meaningful.

Spending Capacity: At ~5.7 Hope/session, players can sustain:
- 5-6 uses of 1-Hope abilities, OR
- 2-3 uses of 2-Hope abilities, OR
- 1-2 uses of 3-Hope abilities plus a smaller ability

High-cost abilities (4-5 Hope) require saving across sessions, which feels appropriate for dramatic, rare effects.

Self-Balancing Factors:
- Combat-heavy sessions generate more Hope (more rolls) to offset higher spending pressure
- The cap at 6 creates pressure for conservative players to spend
- Progress rolls tie Hope to narrative climax moments

> Playtesting Targets: Monitor for players consistently capped at 6 (generation too high), consistently at 0 (generation too low), or specific ability costs that feel unaffordable. Adjust the threshold (currently 4+) or match bonus if the economy proves unbalanced.

### Spending Hope

Abilities that cost Hope in Daggerheart keep their original Hope costs in Daggerforged. "Spend 1 Hope" remains "Spend 1 Hope." "Spend 3 Hope" remains "Spend 3 Hope." The economy is preserved because the earning rate matches Daggerheart.

### "Roll with Hope" and "Roll with Fear" Triggers

Some Daggerheart abilities trigger based on which die was higher, independent of success or failure. These are translated using the action die value:

| Daggerheart Trigger | Daggerforged Translation |
|---------------------|--------------------------|
| "On a roll with Hope" | When your action die shows 4+ |
| "On a roll with Fear" | When your action die shows 1-3 |
| "On a success with Hope" | On a hit (strong or weak), when your action die shows 4+ |
| "On a success with Fear" | On a hit (strong or weak), when your action die shows 1-3 |

This keeps the Hope/Fear check independent from the success/failure outcome, preserving Daggerheart's design where "Failure with Hope" or "Success with Fear" were distinct outcomes.

### Fear Translation (No Fear Track)

Daggerheart's Fear is a GM resource pool. Daggerforged doesn't add a Fear track—Fear references are translated case-by-case during ability conversion:

| Daggerheart Pattern | Daggerforged Translation |
|---------------------|--------------------------|
| "GM spends Fear to end this effect" | "Until the scene ends" / "Until you roll a miss" / "Until you suffer harm" |
| "Remove Fear from GM's pool" | Drop the effect, or grant "+1 momentum" |
| "Swap Hope and Fear dice" | "Turn a weak hit into a strong hit" (once per rest) |
| "GM gains Fear" | "The GM makes a move" or a narrative trigger |

These are guidelines. Each ability should be evaluated individually to find the most faithful expression of its original intent.


---

## Ability Translation

### General Approach

When converting a Daggerheart ability, the question isn't "which SI move does this modify?" but "what does this ability *do* to a moment at the table, and what's the most expressive SI way to produce that same moment?"

Fidelity to the *feel* of the original ability is the goal. Mechanical consistency across all assets is not.

### Available Mechanical Levers

Sundered Isles provides a rich surface to work with. Translations should use whatever combination of the following best serves the ability:

- Move outcomes: adding effects on strong hits, weak hits, or misses of any existing move
- Momentum: granting, burning, or manipulating momentum as a cost or reward
- Progress tracks: marking progress, resisting progress loss, or interacting with challenge resolution
- Asset tracks: custom counters on the asset card for resource pools, charges, or ongoing states
- Conditions: inflicting or clearing conditions on self, allies, or enemies
- Scene-level triggers: "once per scene," "when you enter a fight," "when you make camp"
- Narrative permissions: things the character is simply allowed to do that others can't
- Oracle prompts: abilities that invite or require an oracle roll to determine outcomes
- New moves: when nothing existing fits, define the ability as a wholly new move on the asset

### New Moves as First-Class Design

Defining new moves on assets isn't a fallback—it's one of the most powerful tools available. Many Daggerheart domain abilities are effectively standalone moves with their own trigger, roll, and branching outcomes. Expressing these as actual SI moves preserves their identity and gives them real mechanical weight at the table.

New moves, narrative permissions, asset tracks, and all other forms of ability expression are equally valid. The diversity of how abilities function across the full Daggerforged asset library—some modifying existing moves, some granting new ones, some providing narrative authority, some managing custom resource tracks—is what will make this body of work feel rich and true to Daggerheart's spirit.

Every ability translation is a judgment call. The right fit will sometimes be obvious and sometimes require iteration. The goal is always the most compelling and authentic expression of the original ability in SI terms, whatever form that takes.

### Translation Guidelines

The following guidelines provide consistent translations for common Daggerheart patterns.

#### Stress Costs

When a Daggerheart ability requires marking Stress as a cost, translate to Spirit:

- "Mark a Stress" → "Suffer -1 Spirit"
- "Mark 2 Stress" → "Suffer -2 Spirit"

Players may then choose to Endure Stress if they wish, or simply accept the Spirit loss.

#### Damage and Combat

SI uses progress tracks for combat rather than damage dice. Translate damage-dealing abilities based on their intended impact:

- Minor damage (1d6, 1d8) → "Mark progress"
- Moderate damage (2d8, 2d10) → "Mark progress twice"
- Heavy damage (3d10+, massive hits) → "Mark progress three times"
- Area damage → "Mark progress + momentum"

The exact translation depends on the ability's narrative weight. A signature nuke spell should feel more impactful than a minor damage rider.

#### Range

SI handles positioning narratively rather than with discrete range bands. Translate Daggerheart's ranges as follows:

- Melee / Very Close → "When you are in close quarters" or implies Iron-based approach
- Close / Far → "When you can see your target" or implies Edge-based approach
- Very Far → "Even at great distance"—narrative permission for extreme range

#### Conditions

SI doesn't have a formal condition system. Status effects are handled through fictional positioning and narrative consequences. When translating Daggerheart conditions consider:

| Daggerheart Condition | SI Approach |
|-----------------------|-------------|
| Vulnerable | Fictional positioning: "in a bad spot." +1 harm on Pay the Price, or require Face Danger to act freely |
| Restrained | Fictional barrier: must Face Danger or Secure an Advantage to break free before other actions make sense |
| Hidden | Narrative permission: can't be targeted until the fiction changes (you reveal yourself, they spot you, etc.) |
| Distracted | Impose -1 on their next relevant roll, or give +1 on their next roll against |
| Stunned | Narrative permission: "in control."; player gets a free moment to act |
| Frightened | Narrative constraint: must retreat or justify standing ground; could trigger Endure Stress |

The key difference: SI conditions are fictional states that inform what moves make sense and what consequences follow, not mechanical tags with fixed rules. Translate the *narrative effect* Daggerheart intended, not the mechanical label.


#### Rest and Recovery

Sundered Isles/Starforged doesn't have a "Make Camp" move. Recovery is handled through individual recover moves and the Sojourn move.

SI/SF Recovery Structure:
- Sojourn (roll +Heart): Recovery within a community. Strong hit: each ally chooses 2 recover moves (automatic strong hit). Weak hit: each ally chooses 1 recover move (max 3 total).
- Heal: Restore health (+3 on strong hit, +2 if clearing Wounded)
- Hearten: Restore spirit (+2 on strong hit, +1 if clearing Shaken)
- Resupply: Restore supply (+2 on strong hit, +1 if clearing Unprepared)
- Repair: Restore vehicle/equipment integrity

Daggerheart to SI/SF Mapping:

| Daggerheart | SI/SF Equivalent |
|-------------|------------------|
| Short rest downtime moves | Individual recover moves (Heal, Hearten, Resupply, Repair) made in the field |
| Long rest downtime moves | Sojourn in a community (automatic strong hits on recover moves) |
| Tend to Wounds / Tend to All Wounds | Heal |
| Clear Stress / Clear All Stress | Hearten |
| Repair Armor | Repair |
| Prepare (gain Hope) | No direct equivalent—could translate to +1 momentum or +1 Hope |
| Work on a Project | Advance a progress track or clock |

Translating Rest-Based Abilities:
- "Once per short rest" → "Once per scene" or "When you make a recover move"
- "Once per long rest" → "When you Sojourn" or "Once per session"
- "Until your next rest" → "Until the scene ends" or "Until you Sojourn"
- "Additional downtime move" → Bonus to a specific recover move, or extra benefit when making recover moves
- "Short rest gives long rest benefits" → Upgrade recover move results outside of Sojourn (weak hit → strong hit)

#### Difficulty and Modifiers

Daggerheart abilities often specify fixed difficulties (e.g., "Spellcast Roll (13)"). In SI, drop the fixed difficulty—the challenge dice provide variable difficulty naturally.

If an ability needs to feel harder or more demanding:
- Require a strong hit for full effect (weak hit = partial or complicated success)
- Apply -1 to the action roll
- Add a cost on weak hit (suffer harm, lose momentum, etc.)

Evaluate each ability individually to determine if additional difficulty is warranted.

#### Spellcast Rolls

Daggerheart's "Spellcast Roll" uses a trait determined by subclass. In SI, translate to an action roll using the stat that best fits the magical approach:

- Instinct-based magic → Roll +Wits/+Edge
- Presence-based magic → Roll +Heart
- Knowledge-based magic → Roll +Wits

The Subclass asset should note which stat is used for that subclass's spellcasting. When an ability says "make a Spellcast Roll," the player rolls using their subclass's designated spellcasting stat.

#### Attack Rolls

Daggerheart attack rolls translate to SI action rolls:

- Melee/Strength attacks → Roll +Iron
- Ranged/Finesse attacks → Roll +Edge
- Spell attacks → Roll using spellcasting stat (see above)

The outcome determines narrative effect and progress marked, per standard SI combat.

#### Stat Mappings

Daggerheart uses different stat names than SI:

| Daggerheart Stat/Roll | SI Stat |
|-----------------------|---------|
| Agility | +Edge |
| Strength | +Iron |
| Finesse | +Edge |
| Instinct | +Wits/+Edge |
| Presence | +Heart |
| Knowledge | +Wits |

When an ability references "Agility Rolls" or similar, translate to the appropriate SI stat.

#### Advantage and Disadvantage

Daggerheart's advantage/disadvantage system adds or subtracts a d6 from the roll total (average ±3.5). SI doesn't use this terminology. To achieve approximate mechanical parity:

- "Advantage" → +2 to the roll
- "Disadvantage" → -2 to the roll
- "Ignore disadvantage" → +2 in that situation (effectively cancels the -2)

A +2 bonus represents roughly 57% of Daggerheart's average advantage benefit, but provides a meaningful probability shift in SI's 2d10 challenge system (around 15 percentage points improvement on strong hits).

Note: Some abilities grant +1 bonuses that are NOT translations of advantage—these are intentionally smaller bonuses for effects that have costs (like spending Spirit) or are enhancements to existing moves. Reserve +2 for abilities that explicitly granted advantage in the original Daggerheart text.


#### Defensive Mechanics

SI is player-facing—enemies don't roll dice, and there are no defensive rolls or Evasion scores. Translate defensive abilities using these patterns:

| Daggerheart Pattern | SI Translation |
|---------------------|----------------|
| "+X to Evasion" | Reduce incoming harm by X, or +X when you React Under Fire |
| "Reaction roll" | Roll when reacting to a threat (Face Danger, React Under Fire) |
| "Force enemy to reroll attack" | Reroll the challenge dice on your defensive roll |
| "Enemy attacks have disadvantage" | +1 on rolls to avoid or resist attacks |

Remember: there are no "attacks against you" in SI. The player always rolls.

#### Complete Move Outcomes

When an ability becomes a new move (includes a roll), it must have outcomes for all three tiers:

- Strong hit: Full success, the ability works as intended
- Weak hit: Partial success with a cost or complication (suffer Spirit, put in a bad spot, reduced effect)
- Miss: Typically "Pay the Price" unless a specific failure mode is more appropriate

Incomplete moves (missing weak hit or miss results) create ambiguity at the table. Always define all three.

#### Trigger Clarity

Avoid vague triggers that reference Daggerheart terminology. Be specific about when abilities activate:

| Vague Trigger | Clear Trigger |
|---------------|---------------|
| "On an agility roll" | "When you roll +Edge" |
| "On a reaction roll" | "When you React Under Fire" |
| "When you attack" | "When you Strike or Clash" |
| "Rolls involving climbing" | "When you Face Danger while climbing" or "on any roll while climbing" |

Anchoring to specific SI moves is preferred. When broader application is intended, describe the fictional situation clearly.

#### Progress Tracks

SI uses a single progress track per combat or challenge, not per-enemy. Translate accordingly:

- "Deal damage to target" → "Mark progress"
- "Deal damage to multiple targets" → "Mark progress" (the track represents the overall fight)
- "Extra damage" → "Mark additional progress" or "Mark progress twice"

The fiction determines how progress is interpreted—marking progress against a group might represent wounding several foes, breaking their morale, or gaining tactical advantage.

#### Resource Cost Distribution

When translating abilities with costs, consider the full character loadout. A character whose abilities all drain Spirit will feel resource-starved. Distribute costs across available meters:

- Spirit: Mental/emotional exertion, stress, fear
- Health: Physical strain, pushing your body
- Momentum: Tactical cost, spending advantage
- Supply: Material cost, using resources
- Hope: Preserve original Hope costs from Daggerheart

During holistic review, check that a typical character's active abilities don't stack costs too heavily on any single meter.

---

## Planned Additions (Out of Scope for Initial Build)

- Oracle tables for Daggerheart's campaign frames (Age of Umbra, The Witherwild, etc.)
- Adversary move sets converted from Daggerheart monsters and adversary cards
- Campaign frame modules as standalone documents
- Custom progress track variants for fantasy play
- A proper public-facing README and licensing documentation

---

## Attribution

This is a fan project. All Daggerheart content is the property of Darrington Press. All Sundered Isles and Ironsworn/Starforged content is the property of Shawn Tomkin. Daggerforged is produced under their respective fan content policies and requires ownership of both source games to use.


---

## Conversion Progress

### Ancestries (18 total)
Status: Complete (First Pass)

All 18 ancestries converted with Daggerforged Ancestry Features sections added below the original Daggerheart content. Each file preserves the original text for reference.

| Ancestry | Status | Notes |
|----------|--------|-------|
| Clank | ✓ | Purposeful Design → +1 to chosen stat; Efficient → extra recover move on Make Camp |
| Drakona | ✓ | Scales → harm reduction; Elemental Breath → new move (+Heart, mark progress twice) |
| Dwarf | ✓ | Thick Skin → suffer Spirit to ignore harm; Increased Fortitude → Hope cost preserved |
| Elf | ✓ | Quick Reactions → +1 to next roll; Celestial Trance → extra recover move |
| Faerie | ✓ | Luckbender → reroll challenge dice; Wings → reroll challenge dice when reacting to attack |
| Faun | ✓ | Caprine Leap → narrative permission; Kick → mark progress + knockback |
| Firbolg | ✓ | Charge → new move; Unshakable → chance to ignore Spirit loss |
| Fungril | ✓ | Fungril Network → new move (+Wits); Death Connection → Spirit cost |
| Galapa | ✓ | Shell → passive harm reduction; Retract → defensive stance with tradeoffs |
| Giant | ✓ | Endurance → +1 max Health; Reach → narrative permission for extended range |
| Goblin | ✓ | Surefooted → +1 on terrain rolls; Danger Sense → force reroll once per scene |
| Halfling | ✓ | Luckbringer → party Hope at session start; Internal Compass → reroll 1s on action die |
| Human | ✓ | High Stamina → +1 max Spirit; Adaptability → reroll on miss with background |
| Infernis | ✓ | Fearless → Spirit cost to flip action die result; Dread Visage → +1 to Compel/intimidate |
| Katari | ✓ | Feline Instincts → reroll action die on +Edge; Retracting Claws → new move (vulnerable condition) |
| Orc | ✓ | Sturdy → +1 to all rolls at 1 Health; Tusks → Hope cost for extra progress |
| Ribbet | ✓ | Amphibious → narrative permission; Long Tongue → new move (+Edge) |
| Simiah | ✓ | Natural Climber → +1 while climbing; Nimble → +1 to React Under Fire |

Review Notes:
- Spirit costs are concentrated in ancestries due to Daggerheart's Stress-heavy design for ancestry features
- Will evaluate resource distribution holistically once all asset types are converted
- Several abilities became new moves with full strong/weak/miss outcomes

### Communities (9 total)
Status: Complete (First Pass)

All 9 communities converted with Daggerforged Community Features sections added below the original Daggerheart content. Each file preserves the original text for reference.

| Community | Status | Notes |
|-----------|--------|-------|
| Highborne | ✓ | Privilege → +2 to Compel, Gather Information, or social rolls with nobles/reputation |
| Loreborne | ✓ | Well-Read → +2 on +Wits moves involving history, culture, or politics |
| Orderborne | ✓ | Dedicated → record 3 values; once per session reroll action die when embodying them |
| Ridgeborne | ✓ | Steady → +2 to Face Danger, Undertake an Expedition, or survival/terrain rolls |
| Seaborne | ✓ | Know the Tide → +1 momentum when action die shows 1-3 |
| Slyborne | ✓ | Scoundrel → +2 on +Shadow moves with criminals, detecting lies, or hiding |
| Underborne | ✓ | Low-Light Living → +2 to hide, investigate, or perceive in low light/shadow |
| Wanderborne | ✓ | Nomadic Pack → spend 1 Hope to produce useful mundane item (once per session) |
| Wildborne | ✓ | Lightfoot → +2 on +Shadow moves to avoid detection or move quietly |

Review Notes:
- Most communities translated cleanly to +2 bonuses in specific situations (matching Daggerheart's advantage)
- Seaborne's token-accumulation mechanic simplified to momentum gain on low action die rolls
- Orderborne and Wanderborne preserve their narrative/roleplay hooks (values, pack contents)
- Hope cost preserved for Wanderborne's Nomadic Pack

### Classes (9 total)
Status: Complete (First Pass)

All 9 classes converted with Daggerforged features added directly after each original feature. Each file preserves the original text for reference.

| Class | Status | Notes |
|-------|--------|-------|
| Bard | ✓ | Make a Scene → +1 party-wide vs distracted target (scene); Rally → +2 momentum to party |
| Druid | ✓ | Evolution → free Beastform + stat +1; Beastform → Spirit cost, safety valve at 0 health; Wildtouch → narrative permission |
| Guardian | ✓ | Frontline Tank → restore 2 health or clear Wounded (self); Unstoppable → harm -1, +1 momentum on progress, immunity to movement/restraint |
| Ranger | ✓ | Hold Them Off → Gain Ground benefits on Strike/Clash hit; Ranger's Focus → 1 Hope for +1 vs target, reroll on miss |
| Rogue | ✓ | Rogue's Dodge → +2 defensive rolls until miss; Cloaked → enhanced stealth while stationary; Sneak Attack → +Shadow setup into double progress |
| Seraph | ✓ | Life Support → restore 2 health to ally or clear Wounded; Prayer Dice → 3-box track for +1 roll, -1 harm, or +1 Hope |
| Sorcerer | ✓ | Volatile Magic → reroll action die to upgrade/downgrade hit; Arcane Sense → narrative permission; Minor Illusion → new move (+Wits); Channel Raw Power → vault ability for Hope or progress |
| Warrior | ✓ | No Mercy → +1 offensive combat moves (scene); Attack of Opportunity → upgrade Gain Ground at close quarters; Combat Training → +1 cascade on strong hits |
| Wizard | ✓ | Not This Time → reroll challenge dice on combat miss; Prestidigitation → narrative permission; Strange Patterns → chosen number triggers Hope/Spirit gain |

Review Notes:
- Classes with multiple features retained all features with individual conversions
- Scaling mechanics (tier-based dice, level bonuses) simplified to flat bonuses or momentum
- Resource pools (Prayer Dice, Unstoppable Die) converted to asset tracks or scene-based effects
- New moves created for Minor Illusion with full strong/weak/miss outcomes
- Narrative permissions preserved for flavor abilities (Prestidigitation, Wildtouch, Arcane Sense)
- Hope Features balanced around 3 Hope cost: scene-duration bonuses (+1), instant effects (healing, rerolls), or risky gambits (Volatile Magic)
- Guardian/Seraph healing differentiated: Guardian is self-only, Seraph is ally-only

### Subclasses (18 total)
Status: Complete (First Pass)

All 18 subclasses converted with Daggerforged sections added below the original Daggerheart content. Each file preserves the original text for reference.

| Subclass | Class | Status | Notes |
|----------|-------|--------|-------|
| Call of the Brave | Warrior | ✓ | Courage → Hope on miss with low action die; Battle Ritual → Spirit/Hope boost; Rise to the Challenge → +2 combat at low health; Camaraderie → take ally's harm + Aid bonus |
| Call of the Slayer | Warrior | ✓ | Slayer → 4-box track, spend for +1/box on attacks; Weapon Specialist → Hope for extra progress; Martial Preparation → party Slayer tokens on Sojourn |
| Stalwart | Guardian | ✓ | Unwavering/Unrelenting/Undaunted → scaling harm reduction (1/2/3); Iron Will → supply for harm reduction; Partners-in-Arms → protect allies; Loyal Protector → Spirit to take ally's harm |
| Vengeance | Guardian | ✓ | At Ease → +1 max Spirit; Revenge → Spirit to mark progress when harmed; Act of Reprisal → +1 vs foe who harmed ally; Nemesis → weak hits become strong hits vs marked target |
| Nightwalker | Rogue | ✓ | Shadow Stepper → Spirit to teleport between shadows; Dark Cloud → new move (+Edge) with full outcomes; Adrenaline → extra progress when in bad spot; Fleeting Shadow → +1 React Under Fire; Vanishing Act → instant hide |
| Syndicate | Rogue | ✓ | Well-Connected → narrative permission for contacts; Contacts Everywhere → 1/session benefits (supply, +2, progress); Reliable Backup → 3/session + harm reduction + social bonus |
| Troubadour | Bard | ✓ | Gifted Performer → 3 songs (health, bad spot, Hope); Maestro → Rally gives Hope/Spirit option; Virtuoso → songs 2x per session |
| Wordsmith | Bard | ✓ | Rousing Speech → +2 Spirit to allies; Heart of a Poet → Hope for +1 after roll; Eloquent → 1/session ally benefits; Epic Poetry → Rally +3 momentum, Aid +2 |
| Warden of the Elements | Druid | ✓ | Elemental Incarnation → Spirit to channel element with combat benefits; Elemental Aura → 1/scene aura effects; Elemental Dominion → enhanced element benefits |
| Warden of Renewal | Druid | ✓ | Clarity of Nature → distribute +3 Spirit; Regeneration → 3 Hope for +2 health; Regenerative Reach → range extension; Warden's Protection → 2 Hope for party healing; Defender → protect allies in Beastform |
| Beastbound | Ranger | ✓ | Companion → full companion subsystem with 4 health, command roll (+Edge), upgrade options; Expert/Advanced Training → additional upgrades; Battle-Bonded → +2 React Under Fire; Loyal Friend → take each other's harm |
| Wayfinder | Ranger | ✓ | Ruthless Predator → Spirit for extra progress; Path Forward → narrative permission; Elusive Predator → +2 vs Focus; Apex Predator → Hope for momentum vs Focus |
| Winged Sentinel | Seraph | ✓ | Wings of Light → flight + Spirit to carry + Hope for extra progress; Ethereal Visage → +2 Heart while flying; Ascendant → harm reduction; Power of the Gods → enhanced flight damage |
| Divine Wielder | Seraph | ✓ | Spirit Weapon → ranged melee attack (+Iron), Spirit for multi-target; Sparing Touch → 1/session heal; Devout → Prayer Dice efficiency + 2x Sparing Touch; Sacred Resonance → triple progress on matched strong hit |
| Elemental Origin | Sorcerer | ✓ | Elementalist → element shaping + Hope for +2 or extra progress; Natural Evasion → Spirit + action die for harm reduction; Transcendence → 1/session transformation with 2 benefits |
| Primal Origin | Sorcerer | ✓ | Manipulate Magic → Spirit for spell modification (range, +2, extra progress, multi-target); Enchanted Aid → +2 when aiding magic + 1/session reroll; Arcane Charge → charge state for burst damage |
| School of Knowledge | Wizard | ✓ | Prepared/Accomplished/Brilliant → extra domain abilities at each tier; Adept → Spirit for doubled experience bonus; Perfect Recall → reduced recall cost; Honed Expertise → free experience use on 5+ |
| School of War | Wizard | ✓ | Battlemage → +1 max health; Face Your Fear → extra progress on low action die (scales 1→2→3 with tier); Conjure Shield → +1 React Under Fire with 2+ Hope; Thrive in Chaos → Spirit for extra progress |

Review Notes:
- Spellcast stats preserved in original text but not added to Daggerforged sections (stats written into individual features as needed)
- All features at each tier bundled into a single ability (Foundation/Specialization/Mastery = 3 abilities per card)
- Tag Team Roll → Aid Your Ally with bonuses
- d20 Hope Die mechanics → flat +2 bonuses in relevant situations
- Proficiency scaling → dropped or converted to flat bonuses
- Resource pools (Slayer Dice) → asset tracks with similar economy
- Companion subsystem simplified but functional
- "Roll with Fear" triggers → action die shows 1-3
- Damage scaling (1d10 → 2d10 → 3d10) → progress scaling (1 → 2 → 3 additional)

### Beastforms (24 total)
Status: Not Started

Beastforms are used by the Druid's Beastform class feature. Each beastform will need:
- Stat bonuses mapped to SI (Agility → Edge, Strength → Iron, Instinct → Wits, etc.)
- Evasion bonus dropped (SI doesn't use Evasion)
- Attack stats dropped (SI uses progress tracks)
- Advantages translated to +2 on related rolls
- Features converted using standard translation patterns

### Domains (9 total, ~189 abilities)
Status: Not Started