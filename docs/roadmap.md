---
sidebar_position: 2
---

# Roadmap

:::warning

This project is undergoing heavy development. Plans and documentation may change on a whim!

:::

Feel free to suggest new feature ideas in the Archipelago Discord server.
You can find us in the `#minecraft` channel's "Minecraft Client v2.0" thread.

## Essentials

- [ ] Initial APWorld template
  - [ ] Basic headless server hosting
- [ ] Initial Core Client (interfaces without implementation details)
  - [ ] Location checking
  - [ ] Item receiving
  - [ ] Death link packets
  - [ ] Gifting packets
  - [ ] Ring link packets
  - [ ] Implement the rest of the Archipelago server API

## Vanilla

### Original Randomizer Parity
- [ ] Achievementsanity
- [ ] Boss slaying goals
  - [ ] Ender Dragon goal
  - [ ] Wither goal
  - [ ] All bosses
- [ ] Egg shards
- [ ] Structure randomizer/compasses
- [ ] Bee trap
- [ ] Mob sending

### Sanities
- [ ] Mobsanity
  - [ ] Also randomize mob pools
- [ ] Blocksanity
  - [ ] Also lock blocks from dropping
  - [ ] Also randomize block drops

### Traps
- [ ] Anvil trap

### Links
- [ ] Mob sending
- [ ] Ring link (with experience points instead of rings)
- [ ] Gifting API
  - [ ] Stardew Valley support
  - [ ] Timespinner support
  - [ ] EarthBound support
  - [ ] Lunacid support

## Mod Support
- [ ] Mod loader support
  - [ ] NeoForge
  - [ ] Forge
    - [ ] Forge legacy (&lt;=1.12.2)
  - [ ] Fabric
    - [ ] Fabric legacy (&lt;=1.12.2)
  - [ ] Quilt
- [ ] Individual mod support for the vanilla APWorld via content packs
- [ ] Vanilla backport to 1.21.1 to support major mods; option to choose version
- [ ] KubeJS integration for Core Client
- [ ] Documented API and modding guide

## Developer Experience
- [ ] Content pack system for APWorld templates
- [ ] APWorld template generation
- [ ] DSL for representing large logic chains in Archipelago worlds

## For Future Consideration
- [ ] Biomesanity (cannot enter specific biome without its item)
