# Daggerforged

Daggerforged brings Daggerheart's character system into the Sundered Isles rules engine. Play something that feels like Daggerheart—class identity, ancestry, community, domain abilities, progression—while Sundered Isles handles all the underlying mechanics.

This is an additive asset pack, not a replacement. SI rules stay untouched. Daggerheart provides the character content.

## What's Here

Each file contains the original Daggerheart text followed by a "Daggerforged" section with the Sundered Isles conversion.

| Asset Type | Count | Status |
|------------|-------|--------|
| Ancestries | 18 | First pass complete |
| Communities | 9 | First pass complete |
| Classes | 9 | First pass complete |
| Subclasses | 18 | First pass complete |
| Domain Abilities | 189 | Not started |
| Beastforms | 24 | Not started |

## Project Structure

```
assets/
├── ancestries/    # Clank, Drakona, Dwarf, Elf, etc.
├── communities/   # Highborne, Loreborne, Orderborne, etc.
├── classes/       # Bard, Druid, Guardian, Ranger, etc.
├── subclasses/    # Call of the Brave, Nightwalker, Troubadour, etc.
├── domains/       # Arcana, Blade, Bone, etc. (structure only)
└── abilities/     # Domain abilities (not yet converted)
```

## Design Philosophy

See [DESIGN.md](DESIGN.md) for the full specification, including:
- How Hope works in Daggerforged
- The loadout/vault system for domain abilities
- Translation guidelines for converting Daggerheart mechanics to SI
- Progression and multiclassing rules

## Feedback Welcome

This is a work in progress. If you're from the Ironsworn community and have thoughts on the conversions, I'd love to hear them—especially on:
- Do the translations feel faithful to Daggerheart's intent?
- Are there SI mechanics I'm underusing or misusing?
- Does the Hope economy seem balanced?

## Attribution

This is a fan project. All Daggerheart content is the property of Darrington Press. All Sundered Isles and Ironsworn/Starforged content is the property of Shawn Tomkin. Daggerforged is produced under their respective fan content policies and requires ownership of both source games to use. And sourced from these two repos:

- [Daggerheart SRD](https://github.com/seansbox/daggerheart-srd)
- [Sundered Isles / Starforged Datasworn](https://github.com/tbsvttr/datasworn)
