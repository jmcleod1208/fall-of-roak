# Game Design Document Index

Read this file first in any new chat, space, or assistant workflow.

## Project Frame

**Project:** Fall of Ro'ak

**Genre:** Story-driven fantasy auto-battler RPG.

**Tone:** High-fantasy, dark, Witcher-adjacent, grounded but mythic.

**Relationship to Lore Bible:** The lore bible owns setting, history, characters, factions, locations, terminology, and narrative canon. This GDD owns player experience, mechanics, progression, economy, UI, technical requirements, balance, and implementation-facing rules.

## Collaboration Workflow

The GDD uses the same lock-in workflow as the lore bible.

1. The assistant reads this index first.
2. The user chooses a numbered GDD file.
3. The assistant asks numbered design questions.
4. The user answers with letters, short text, or corrections.
5. The assistant drafts complete design prose inline.
6. The user says `lock in` when approved.
7. The assistant updates the file and preserves open questions.

## Hard Rules for Assistants

- Do not infer missing gameplay decisions.
- Ask direct questions instead of filling blanks.
- Do not overwrite locked decisions without explicit approval.
- Keep mechanics separate from lore.
- No emojis.
- No italics.
- No image generation as part of this workflow.
- Use plain Markdown.
- Maintain zero-padded file names.
- Track unresolved decisions in each file.

## Locked Continuity Constraints from Lore Bible

These are lore constraints that can affect mechanics, but the GDD should not rewrite them.

- **Valerian** is the locked spelling.
- **Mothers** wield no magic.
- **Ro'ak** is the only surviving Mother-child.
- **Vallen** is a Skye.
- **Dragons** are Creator-made natives except Vorthak.
- **Crownhaven / year dating** is locked at 500 AC.
- **Mother's Hearth** is Noctheris's prison and the final battle location.
- **Ro'ak's death** occurs in Ro'ak's High Hall.

## File Map

- `00_overview.md` — Product pillars, target player, platform assumptions, design goals.
- `01_core_loop.md` — Session loop, meta loop, reward loop, fail states.
- `02_player_progression.md` — Account progression, party growth, unlocks, difficulty curve.
- `03_combat_system.md` — Combat rules, round flow, targeting, win/loss conditions.
- `04_auto_battler_systems.md` — Board rules, formations, synergies, traits, drafting.
- `05_heroes_units.md` — Hero mechanics, unit roles, stats, abilities, rarity or upgrade rules.
- `06_enemies_encounters.md` — Enemy mechanics, encounter types, bosses, challenge design.
- `07_items_equipment.md` — Gear, artifacts, consumables, crafting, itemization rules.
- `08_world_campaign.md` — Campaign structure, regions, travel, map progression.
- `09_economy_rewards.md` — Currencies, rewards, shops, sinks, pacing, monetization stance.
- `10_ui_ux.md` — Screen map, input model, HUD, accessibility, onboarding.
- `11_technical_design.md` — Engine assumptions, data structures, saves, tools, deployment.
- `12_content_pipeline.md` — How new heroes, enemies, items, levels, and events are authored.
- `13_balance_qa.md` — Balance methods, test cases, telemetry, QA checklist.
- `14_glossary.md` — Mechanical terms, acronyms, stat names, and locked naming.

## Recommended Build Order

Start with these files in order:

1. `00_overview.md`
2. `01_core_loop.md`
3. `03_combat_system.md`
4. `04_auto_battler_systems.md`
5. `02_player_progression.md`
6. `09_economy_rewards.md`
7. `10_ui_ux.md`
8. `11_technical_design.md`

## Current Status

All files are initialized as templates. No new mechanics are locked by this setup unless explicitly labeled as a locked continuity constraint from the lore bible.

