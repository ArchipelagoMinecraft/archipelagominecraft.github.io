---
sidebar_position: 2
---

# Roadmap

:::warning

This project is in a heavy pre-production state.
All information on this wiki is subject to change!

Please leave any feedback at https://discord.gg/archipelago
(find us in
[`#minecraft` in the Minecraft Client 2.0 thread](https://discord.com/channels/731205301247803413/1394782863135608832/1394783006849368065)).

:::

Feel free to suggest new feature ideas in the Archipelago Discord server.
You can find us in the `#minecraft` channel's "Minecraft Client v2.0" thread.

:::info
This roadmap is a long-term plan, not a list of promises.
All of this is free, and good software takes time to develop. Please be patient!

If you are interested in contributing, feel free to give us a hand.
:::

## Essentials

- [ ] Initial prototype/proof of concept
  - [x] Multi-mod loader support
  - [x] Multi-version support
  - [ ] Test APWorld
  - [ ] First connection from 1.21.8
  - [ ] First connection from 1.12.2
  - [ ] First item/location send
  - [ ] Fully modularized project structure

### APWorld
- [ ] Initial APWorld template
  - [ ] Content pack system for APWorld templates
  - [ ] `.apmcbundle` generation
  - [ ] Basic headless server hosting

### Core Client
- [ ] Initial Core Client (interfaces without Minecraft implementation details)
  - [ ] Location checking
  - [ ] Item receiving
  - [ ] Bounce packets
  - [ ] Death link packets
  - [ ] Gifting packets
  - [ ] Ring link packets
  - [ ] Implement the rest of the Archipelago server API

## Vanilla

### Original Randomizer Parity
- [ ] [Sanities](#sanities): Advancementsanity
  - [ ] [Sanities](#sanities): Include legacy achievements
- [ ] [Goals](#goals): Boss slaying goals
  - [ ] [Goals](#goals): Ender Dragon goal
  - [ ] [Goals](#goals): Wither goal
  - [ ] [Goals](#goals): All bosses
- [ ] [Traps](#traps): Bee trap
- [ ] Egg shards
- [ ] Spawn all end gateways by default
- [ ] Structure randomizer/compasses
  - [ ] Increased structure spawn rate
- [ ] Mob sending
- [ ] Custom Nether/End village structures
- [ ] Increased Wither Skull drop rates

### Sanities
- [ ] Advancementsanity
  - [ ] Include legacy achievements
- [ ] Createsanity
  - [ ] Craftsanity
    - [ ] More crafting unlock tiers/categories
      - [ ] Neat toggleable categories, such as "essentials", or more specific randomization options
      - [ ] Crafting table
      - [ ] Storage
      - [ ] Lights
      - [ ] Ore tiers (iron/diamond/netherite etc.)
      - [ ] Cooking
      - [ ] Logistics
        - [ ] Transportation
        - [ ] Redstone
      - [ ] Decor
  - [ ] Smeltsanity
    - [ ] Logic for all furnaces, including campfires
  - [ ] Enchantsanity
    - [ ] Cursesanity
  - [ ] Brewsanity
- [ ] Mobsanity
  - [ ] Also randomize mob pools
  - [ ] Wither Skulls are items
- [ ] Farmsanity
  - [ ] Cropsanity
  - [ ] Fishsanity
- [ ] Exploresanity
  - [ ] Dimensionsanity
    - [ ] Lock nether and end access
  - [ ] Biomesanity
    - [ ] Biome compass
    - [ ] Exclude Rare Biomes
  - [ ] Structuresanity
- [ ] Blocksanity
  - [ ] Block mining/block drops and gate them behind tools/tiers (fist, pickaxe, shovel, etc.)
    - [ ] Also lock by material type, such as iron, diamond, netherite, etc.
  - [ ] Also lock blocks from dropping
  - [ ] Also randomize block drops
- [ ] Itemsanity
  - [ ] Discsanity
- [ ] Animalsanity
  - [ ] Breedsanity
  - [ ] Tamesanity
- [ ] Tradesanity
  - [ ] Trade slot lock
- [ ] Huntsanity (like block/itemsanity but limited to a specific list of items)
  - [ ] Item hunt
  - [ ] Block hunt
  - [ ] Custom maximum amount of items to find

### Gamemodes

- [ ] Bingo
  - [ ] Customizable grid size

### Traps
- [ ] Anvil trap
- [ ] Potion effect trap
  - [ ] Poison, blindness, etc.
- [ ] Mob trap
  - [ ] Bee trap
  - [ ] Creeper trap
  - [ ] Chicken jockey trap
  - [ ] Warden trap
- [ ] Nighttime trap

### Buffs and Filler
- [ ] Permanenent status boosts
  - [ ] Progressive health
  - [ ] Progressive inventory (9/18/27 slots)
  - [ ] Progressive speed
- [ ] Various effects like Strength, Speed II, Haste III, etc.
- [ ] Blocks
  - [ ] Dirt
- [ ] Resources
  - [ ] Gold/iron nuggets
  - [ ] Bones

### Goals
- [ ] Boss slaying goals
  - [ ] Ender Dragon goal
  - [ ] Wither goal
  - [ ] Elder Guardian
  - [ ] All bosses
- [ ] Huntsanity: Find all items
- [ ] Netherite Hoe goal

### Links
- [ ] Mob sending
- [ ] Ring link (with experience points instead of rings)
- [ ] Gifting API
  - [ ] Stardew Valley support
  - [ ] Timespinner support
  - [ ] EarthBound support
  - [ ] Lunacid support

### Randomization
- [ ] Randomize mob spawns
- [ ] Structure randomizer
  - [ ] Structure compass
  - [ ] Chest lock for chests in structures
  - [ ] More randomized structures
    - [ ] Igloo
    - [ ] Ocean monument
    - [ ] Mansion
    - [ ] Ancient city
    - [ ] Mineshaft
    - [ ] Dungeon
    - [ ] Jungle temple
    - [ ] Desert pyramid
    - [ ] Modded structure support?

### World Generation Options
- [ ] Seed
- [ ] Superflat
- [ ] Amplified
- [ ] Large biomes
- [ ] Random biomes
- [ ] Equal biome chances
- [ ] Structures in any biome

### Custom Achievements
- [ ] Furnace% tribute
  - [ ] 37 furnaces
  - [ ] 37 blast furnaces
  - [ ] 37 stacks of furnaces
  - [ ] 37 stacks of blast furnaces

## Mod Support
- [ ] Individual mod support for the vanilla APWorld via content packs
- [ ] Vanilla backport to 1.21.1 to support major mods; option to choose version
- [ ] KubeJS integration for Core Client
- [ ] Documented API and modding guide

## Backport Requests

These backports should eventually become available when we stabilize the core and vanilla APIs.

- [ ] Forge 1.16.5 + KubeJS Addon for Create Above and Beyond (@Treeways)
- [ ] Cursed Fabric Loader 1.5.2 for Better Than Wolves: Community Edition (@Patchwork)
  - [BTW CE Repository](https://github.com/BTW-Community/BTW-Public?tab=readme-ov-file)
- [ ] Forge 1.7.10 for GregTech New Horizons (multi-developer effort; we need to put together a team for this)
  - [1.7.10 ExampleMod](https://github.com/GTNewHorizons/ExampleMod1.7.10) | [GTNH Modding Guide](https://gtnh.miraheze.org/wiki/Development)

## For Future Consideration
- [ ] APWorld: Template generator
- [ ] Sanities: Biomesanity (cannot enter specific biome without its item)
- [ ] DX: DSL for representing large logic chains in Archipelago worlds