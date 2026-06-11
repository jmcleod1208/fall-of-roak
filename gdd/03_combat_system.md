# 03 Combat System

## Purpose

Define the tactical combat rules that every battle follows.

## Status

**Design State:** Locked initial combat system.

**Last Locked Update:** 2026-06-10

## Locked Inputs

- **Project:** Fall of Ro'ak.
- **Genre Frame:** Auto-battler and town-management idle RPG.
- **Combat Input:** Strictly automatic setup-only combat.
- **Battle Format:** One player party versus one enemy party.
- **Hero Structure:** Four fixed main heroes, with recruited followers supporting them.
- **Lore Source:** Lore bible remains the source of truth for canon.

## Combat Summary

Combat in **Fall of Ro'ak** is strictly automatic. The player prepares the party before battle, but does not activate abilities or issue commands once combat begins.

Each battle is one player party versus one enemy party. Units act automatically, use cooldown-based abilities, and choose targets through random targeting rules. Taunting abilities influence targeting by making all enemies more likely to attack the taunting unit.

## Battle Format

Battles use a **one party vs one party** structure.

The player's side consists of:

- The four fixed heroes.
- Any recruited followers assigned to the battle.
- Gear and loadout choices.
- Formation and preparation choices.

The enemy side consists of:

- One enemy party.
- Enemy units, elites, or bosses depending on the encounter.
- Enemy abilities and roles.

Campaign battles and repeat farming battles both follow this basic combat format unless a later document defines exceptions.

## Player Input During Combat

Combat is fully automatic.

Locked rules:

- The player does not activate abilities.
- The player does not issue commands.
- The player does not retarget units manually.
- The player does not reposition units mid-battle.
- The player's meaningful decisions happen before combat begins.

This supports the setup-only auto-battler design already locked in `01_core_loop.md`.

## Unit Actions

Units use **cooldown-based abilities**.

During combat, each unit:

- Performs basic attacks or default actions.
- Automatically casts abilities when cooldowns are ready.
- Follows its role and ability rules.
- Continues acting until defeated, disabled, or the battle ends.

The player does not manually trigger abilities. Ability timing is handled by the combat system.

## Targeting

Default targeting is **random**.

When a unit acts, it chooses a valid target randomly unless an ability, role, formation rule, or status effect changes that behavior.

### Taunt

Taunting abilities do not guarantee that enemies will always attack the taunting unit. Instead, taunt makes **all enemies more likely** to target that unit.

This keeps targeting unpredictable while still giving tanks and defensive followers meaningful control over enemy pressure.

## Stats

The first combat model uses **simple RPG stats**.

Core stats:

- **Health:** How much damage a unit can take before being defeated.
- **Attack:** The unit's basic offensive power.
- **Defense:** Reduces all incoming damage.
- **Speed:** Influences both basic attack rate and cooldown recovery.
- **Healing Power:** Improves healing abilities or healing item effects.

These stats are intentionally simple so combat can be prototyped, balanced, and understood before adding deeper systems.

## Down and Defeat Model

The four main heroes do not die. When a hero reaches 1 HP, they become downed rather than killed.

Downed handling is fully automatic and governed entirely by pre-battle setup:

- If a party member has a revive potion equipped, it is used automatically during combat to revive the downed party member to 5% HP.
- Revive potions are equipped before battle. Equipping a revive potion is a pre-battle decision, not a mid-combat command. The player never chooses whether or when to spend a revive potion during combat.
- If no revive potions remain and all party members are downed, the battle ends. The party retreats and recovers.

Recruited followers do not share the heroes' protection. Followers may still be injured or killed according to the locked follower rules in `01_core_loop.md` and `02_player_progression.md`.

## Victory and Defeat

A battle ends when one side is defeated.

The player wins when the enemy party is defeated.

The player loses when every party member is downed and no revive potions remain. Since the four main heroes cannot be killed, defeat causes retreat and recovery. Recruited followers may be injured or killed depending on the outcome.

## Lore Cross-Reference

This combat model supports the lore bible by keeping the four heroes central and protected from permanent death while allowing recruited followers to carry greater risk. The strictly automatic structure reinforces the GDD's preparation-focused design: victory comes from planning, gear, followers, formation, and supply support rather than reflexes.

Taunt fits the darker battlefield tone because defensive units can draw danger toward themselves, but cannot fully control chaos. Random targeting helps combat feel dangerous and imperfect without making outcomes fully uncontrollable.

## Locked Design Decisions

- Combat is strictly automatic.
- The player does not activate anything during battle.
- Battles are one player party versus one enemy party.
- Units auto-cast abilities on cooldown.
- Default targeting is random.
- Taunting abilities make all enemies more likely to attack the taunting target.
- The first combat model uses simple RPG stats.
- Core stats are Health, Attack, Defense, Speed, and Healing Power.
- Defense reduces all incoming damage.
- Speed affects both basic attack rate and cooldown recovery.
- Combat decisions happen before battle, not during battle.
- Heroes do not die; a hero at 1 HP becomes downed.
- A revive potion equipped before battle is used automatically to revive a downed party member to 5% HP.
- Revive potion equipping is a pre-battle decision, not a mid-combat command.
- If all party members are downed and no revive potions remain, the battle ends and the party retreats and recovers.
- Battle defeat leads to retreat and recovery for heroes.
- Followers can be injured or killed.

## Open Questions

None for this file.
