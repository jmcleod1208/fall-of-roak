# 04 Auto-Battler Systems

## Purpose

Define the systems that make team-building, drafting, positioning, and synergy decisions matter.

## Status

**Design State:** Locked initial auto-battler systems.

**Last Locked Update:** 2026-06-10

## Locked Inputs

- **Project:** Fall of Ro'ak.
- **Genre Frame:** Auto-battler and town-management idle RPG.
- **Combat Input:** Strictly automatic setup-only combat.
- **Battle Format:** One player party versus one enemy party.
- **Hero Structure:** Four fixed main heroes, with optional recruited followers supporting them.
- **Lore Source:** Lore bible remains the source of truth for canon.

## Auto-Battler Summary

The auto-battler layer in **Fall of Ro'ak** focuses on preparation, placement, party composition, and simple role synergies.

The player always deploys the four fixed heroes and may add up to four optional recruited followers. Combat happens on a grid board. The player positions the party before battle, then combat resolves automatically using the locked combat rules from `03_combat_system.md`.

## Board Layout

Battles use a **grid board**.

The recommended first prototype layout is a **4x4 player deployment grid** mirrored against a **4x4 enemy deployment grid**.

This gives:

- **Player side:** 4 columns x 4 rows.
- **Enemy side:** 4 columns x 4 rows.
- **Total battlefield:** 4 columns x 8 rows if displayed vertically, or 8 columns x 4 rows if displayed horizontally.

The 4x4 player side gives enough room for the four heroes plus up to four followers without filling every space. It is also more readable for PC, Steam, mobile, and web than a larger board. The grid should support formation decisions without becoming too tactical or fiddly for a fully automatic combat system.

The grid should support:

- Frontline and backline positioning.
- Protecting vulnerable units.
- Placing tanks where they can absorb pressure.
- Keeping healers and ranged units safer.
- Formation-based preparation without mid-battle repositioning.

The exact visual orientation is not locked in this file. It can be handled later in UI/UX or prototype implementation.

## Party Size

The player always deploys the four fixed heroes as the core party.

The player can also bring up to **four optional recruited followers** into normal battles.

Locked structure:

- **Four fixed heroes:** Always deployed and always central to the party and story.
- **Up to four optional followers:** Recruited support units that expand strategy.
- **Maximum normal party size:** Eight units total.

Followers are optional because the four heroes remain the narrative core. Followers add tactical flexibility, risk, and build variety.

## Pre-Battle Setup

Before battle, the player decides:

- Which followers to bring.
- Where each hero and follower is placed on the grid.
- Which gear and loadouts are equipped.
- Which role synergies are active.
- Whether the party has enough healing items and supplies to continue.

Once battle begins, the player does not move units, activate abilities, retarget enemies, or issue commands. The player's meaningful auto-battler decisions happen during setup.

## Role-Based Synergies

Synergies are bonuses created by party composition.

The first version of synergies should be **simple role synergies**. These bonuses come from bringing certain role combinations into battle.

Heroes and followers both count toward role synergies.

First role categories:

- **Tank:** Protects the party and benefits from taunt or defensive abilities.
- **Healer:** Restores health or improves recovery during combat.
- **Damage Dealer:** Focuses on killing enemies quickly.
- **Support:** Buffs allies, weakens enemies, or improves party performance.

Role synergies should be easy to understand. They should reward preparation without forcing the player to memorize a large trait web.

Example synergy directions:

- Two tanks improve party survivability.
- Two healers improve healing output or healing item efficiency.
- Multiple damage dealers improve offensive pressure.
- Support units improve cooldowns, defense, or party consistency.
- Balanced teams gain a small bonus for including multiple role types.

These examples are not final numbers. They define the intended style.

## Follower Acquisition

Followers are acquired through **Homefront systems and story progress**.

Story progress can unlock new follower types, while Homefront recruitment systems allow the player to recruit or replace followers.

This supports the locked progression model:

- Campaign story gates new content.
- Homefront buildings handle recruitment and rebuilding systems.
- Followers can be injured or killed.
- Replacing followers should connect back to the Homefront.

## Relationship to Locked Combat Rules

This file builds on `03_combat_system.md`.

Locked combat rules that apply here:

- Combat is strictly automatic.
- Battles are one player party versus one enemy party.
- Units auto-cast abilities on cooldown.
- Targeting is random by default.
- Taunt makes all enemies more likely to attack the taunting unit.
- The first combat model uses simple RPG stats.
- Speed affects attack rate and cooldown recovery.
- Defense reduces all incoming damage.

The grid, party size, and role synergies should work with those combat rules rather than replacing them.

## Lore Cross-Reference

This system supports the lore bible by keeping the four heroes fixed, always deployed, and central while allowing recruited followers to represent the broader survivor and rebuilding effort.

The grid board should make the heroes and followers feel like a prepared war party marching east, not disposable pieces in a disconnected tactics puzzle. Followers can add strategy and risk, but they should not replace the lore importance of Vallen, Runlan, Calypsa, and Van.

Homefront-based recruitment supports the rebuilding theme established in the GDD. Story-based follower unlocks allow new regions and campaign beats to introduce new kinds of people joining the cause without inventing lore outside the lore bible.

## Locked Design Decisions

- Battles use a grid board.
- Recommended first prototype grid is 4x4 player side versus 4x4 enemy side.
- Exact visual orientation is not locked yet.
- The four fixed heroes are always deployed.
- The four fixed heroes are always the party core.
- Heroes count toward role synergies.
- The player may bring up to four optional recruited followers.
- Maximum normal party size is eight units.
- Followers are optional support units.
- The player positions units before battle.
- Units cannot be repositioned during battle.
- Synergies are simple role-based bonuses.
- First synergy categories are Tank, Healer, Damage Dealer, and Support.
- Followers are acquired through Homefront systems and story progress.
- Story progress can unlock new follower types.
- Homefront systems handle recruitment and replacement.

## Open Questions

None for this file.
