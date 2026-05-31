# 01 Core Loop

## Purpose

Define what the player repeatedly does, why it is satisfying, and how each loop feeds the next.

## Status

**Design State:** Locked initial core loop.

**Last Locked Update:** 2026-05-30

## Locked Inputs

- **Project:** Fall of Ro'ak.
- **Genre Frame:** Auto-battler and town-management idle RPG.
- **Combat Input:** Setup-only auto-battler combat.
- **Homefront:** Gameplay/UI term for the broader rebuilding network that supports the party.
- **Lore Source:** Lore bible remains the source of truth for canon.

## Core Loop Summary

**Fall of Ro'ak** loops between story, Homefront rebuilding, preparation, caravan logistics, battle, loot, recovery, and repeat farming. The player receives lore or story for new objectives, manages Homefront production, resupplies the four fixed heroes and recruited followers, sends supplies by caravan, engages in setup-only auto-battler combat, loots rewards, and sends valuable supplies back to the Homefront.

The Homefront is the gameplay-facing term for the player's rebuilding network. It starts with the early survivor base, but it can expand as the game progresses because the player will eventually manage more than one rebuilding project. Individual settlements can still have lore names, but the management system is called the **Homefront**.

The Homefront and the marching party are connected through a safe caravan route. The caravan cannot be attacked and always completes its delivery, but it takes time to travel. In the early game, caravan travel should take about one minute. As the heroes travel farther east, caravan travel time increases because the party is farther from the Homefront.

## Moment-to-Moment Loop

The player's active decisions happen before and after battle, not during combat.

Before battle, the player:

- Reviews the current story beat, region pressure, or objective.
- Checks Homefront production and available supplies.
- Resupplies the four fixed heroes and any recruited followers.
- Sends needed supplies by caravan.
- Adjusts party composition, gear, followers, formation, and battle preparation.
- Chooses whether to push forward, recover, or run repeat farming battles.

During battle, combat resolves automatically based on preparation. The player does not issue normal commands during combat.

After battle, the player:

- Claims loot and resources.
- Sends valuable supplies back to the Homefront by caravan.
- Uses rewards to support rebuilding, resupply, upgrades, recovery, or future combat preparation.
- Advances story if the battle was a campaign objective.
- Continues repeat farming if the battle was a farming target and the party has enough resources.

## Encounter Loop

Each non-farming encounter follows this structure:

1. **Story or Objective Context:** The game frames why this fight matters, whether it is tied to a region, a supply need, Ro'ak's forces, the march east, or Homefront recovery.
2. **Homefront and Supply Check:** The player reviews production, available healing items, caravan status, and needed resources.
3. **Preparation:** The player chooses heroes, recruited followers, gear, formation, supplies, and battle plan.
4. **Caravan Delivery:** Needed supplies travel from the Homefront to the party. This always succeeds, but takes time.
5. **Automatic Battle:** The fight resolves without mid-combat input.
6. **Loot and Results:** The player receives resources, gear, supplies, and progression rewards.
7. **Send Supplies Back:** Valuable resources can be sent back to the Homefront by caravan.
8. **Next Decision:** The player chooses whether to push forward, farm, recover, upgrade, or focus on the Homefront.

## Repeat Farming Loop

Repeat farming uses repeatable battles with no story attached.

The player can start a repeat farming battle loop when they want resources and have enough supplies to sustain continued combat. Farming can be set and forget. The party continues running repeatable battles automatically as long as enough required resources remain.

Set-and-forget repeat farming consumes **healing items**. The player can stop repeat farming at any time. Repeat farming also stops if the party is defeated in battle.

Repeat farming should be useful for gathering resources, but it should not interrupt the lore or campaign pacing. Story does not play during repeat farming.

## Session Loop

A normal play session centers on three activities:

- **Send supplies:** Move resources, loot, and healing items between the Homefront and the heroes by caravan.
- **Get story:** Receive lore, character moments, campaign context, or regional updates when advancing new objectives.
- **Farm battles for resources:** Run repeatable battles to gather materials, loot, and supplies needed for Homefront growth and hero preparation.

A short session should still feel productive if the player only checks Homefront production, sends caravan supplies, and starts or stops repeat farming. A longer session can include several battles, multiple upgrade decisions, recovery, Homefront improvements, and a meaningful story step.

## Meta Progression Loop

The long-term loop is about turning battlefield success into regional recovery and better logistics.

The player gains power through:

- The four fixed heroes growing stronger.
- Recruited followers expanding party strategy.
- Stronger gear and loadouts.
- Better Homefront production.
- More healing items and supplies.
- Faster, larger, or more efficient caravan upgrades.
- Improved recovery options.
- Access to deeper eastern regions, harder battles, and more dangerous enemies.

Homefront growth and party strength feed each other. A stronger Homefront produces better supplies and healing items. Better supplies allow the party to survive longer, recover faster, farm more, and win harder battles. Harder battles return better loot, which helps the Homefront rebuild and support the march east.

## Caravan System

The caravan is the safe logistics bridge between the Homefront and the heroes.

Locked rules:

- The caravan moves supplies both ways between the Homefront and the party.
- The caravan cannot be attacked.
- The caravan always succeeds.
- The caravan takes time to travel.
- Early-game caravan travel takes about one minute.
- Caravan travel time increases as the party travels farther east.
- Caravan capacity is limited by item quantity.
- Caravan size upgrades and caravan speed upgrades unlock at different stages of the game.

Caravan upgrades should create long-term logistical progression. Size upgrades improve how many items can move per trip. Speed upgrades reduce travel time. These upgrades should not unlock all at once.

## Healing Item Economy

Healing items are split into two production sources:

- **Small healing items:** Produced by Calypsa.
- **Large healing items:** Produced in the Homefront.

Small healing items connect Calypsa directly to the party's ability to continue fighting, farming, and recovering. Large healing items connect Homefront production to deeper campaign pushes and longer periods away from safety.

Healing items are consumed by:

- Set-and-forget repeat farming.
- Recovery after defeat.
- Sustaining the party during extended combat loops.

## Recovery and Risk

Losing a battle causes the party to **retreat and recover**.

Recovery costs:

- **Time**
- **Healing items**

The four main heroes can be injured, but they cannot be killed. Recruited followers carry higher risk: they can be injured and can also be killed.

This makes followers strategically valuable but expendable in a way the four heroes are not. It also supports the dark tone from the lore bible without breaking the locked hero structure.

Failure should not erase campaign progress or destroy Homefront progress. Instead, it creates a recovery loop:

1. The heroes and recruited followers retreat.
2. The player reviews what failed.
3. Recovery consumes healing items and time.
4. The Homefront may need to produce or send more healing items.
5. The player adjusts gear, formation, followers, or resource investment.
6. The party returns better prepared.

Failure should feel serious because it drains time and healing resources. It should not feel permanently punishing.

## Narrative Loop

The story loop follows the lore bible's core direction: Fernfield falls, the survivors move east, Ro'ak's destruction leaves wounds behind, and the player's victories help restore what was broken.

Story appears through:

- New objectives.
- Region introductions.
- Campaign battles.
- Survivor needs.
- Rebuilding updates.
- Hero dialogue.
- Enemy discoveries.
- Reports from towns receiving supplies.
- Major milestones against Ro'ak's lieutenants and forces.

Story does **not** appear during repeat farming battles.

## Locked Design Decisions

- Combat is **setup-only**.
- The player does not issue normal commands during battle.
- The four core heroes stay the same.
- The four core heroes can be injured but cannot be killed.
- Followers can be recruited.
- Recruited followers can be injured and killed.
- The core loop includes story, Homefront production, resupply, caravan logistics, battle, loot, recovery, and sending supplies back to the Homefront.
- Supplies are sent between the Homefront and heroes by caravan.
- The caravan cannot be attacked.
- The caravan always succeeds.
- Caravan travel takes time.
- Early-game caravan travel takes about one minute.
- Caravan travel time increases as the party travels farther east.
- Caravan capacity is limited by item quantity.
- Caravan size and speed upgrades unlock at different stages of the game.
- Large healing items are produced in the Homefront.
- Small healing items are produced by Calypsa.
- Farming happens through repeatable battles.
- Repeat farming can be set and forget.
- Repeat farming consumes healing items.
- Repeat farming can be stopped by the player at any time.
- Repeat farming stops if the party is defeated.
- No story plays during repeat farming.
- Losing a battle means retreat and recover.
- Recovery costs time and healing items.
- Homefront recovery and the march east are mechanically connected.

## Lore Cross-Reference

This core loop follows the lore bible by keeping the four main heroes fixed, preserving their importance, and making them injurable but not killable. Recruited followers absorb the higher-risk role and can be injured or killed. The Homefront supports the lore direction of rebuilding what Ro'ak broke while the heroes continue the march east toward Ro'ak and Noctheris.

Calypsa's production of small healing items should be treated as a mechanics-facing expression of her role in sustaining the party. It should not overwrite lore bible canon about her character unless separately locked in the lore bible.

## Open Questions

- What caravan size upgrade unlocks first?
- What caravan speed upgrade unlocks first?
- Are small and large healing items the only healing item tiers?
- Can killed followers be replaced immediately, or does recruitment require Homefront resources, time, or story progress?
