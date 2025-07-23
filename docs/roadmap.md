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
This roadmap is a long-term plan, <u>not a list of promises</u>.
We're doing this for free, and we've got life to tend to as well.
Please be patient with us!

If you would like to help code some of these features, feel free to offer us a hand
in our Discord server (see above for links).
:::

## Essentials

- [ ] Initial prototype/proof of concept
  - [x] Multi-mod loader support
  - [x] Multi-version support
  - [ ] Test APWorld
  - [ ] First connection from 1.21.8
  - [ ] First connection from 1.12.2
  - [ ] First item/location send
  - [ ] Modular project structure
- [ ] Initial APWorld template
  - [ ] `.apmcbundle` generation
  - [ ] Basic headless server hosting
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
- [ ] Advancementsanity
- [ ] Boss slaying goals
  - [ ] Ender Dragon goal
  - [ ] Wither goal
  - [ ] All bosses
- [ ] Egg shards
- [ ] Spawn all end gateways by default
- [ ] Structure randomizer/compasses
- [ ] Increased structure spawn rate
- [ ] Bee trap
- [ ] Mob sending
- [ ] Custom Nether/End village structures
- [ ] Increased Wither Skull drop rates

### Sanities
- [ ] Mobsanity
  - [ ] Also randomize mob pools
- [ ] Blocksanity
  - [ ] Also lock blocks from dropping
  - [ ] Also randomize block drops
- [ ] Itemsanity
- [ ] Huntsanity (like block/itemsanity but limited to a specific list of items)
  - [ ] Item hunt
  - [ ] Block hunt
  - [ ] Custom maximum amount of items to find

### Gamemodes

- [ ] Bingo
  - [ ] Customizable grid size

### Traps
- [ ] Anvil trap

### Goals
- [ ] Huntsanity: Find all items

### Links
- [ ] Mob sending
- [ ] Ring link (with experience points instead of rings)
- [ ] Gifting API
  - [ ] Stardew Valley support
  - [ ] Timespinner support
  - [ ] EarthBound support
  - [ ] Lunacid support

## Mod Support
- [ ] Individual mod support for the vanilla APWorld via content packs
- [ ] Vanilla backport to 1.21.1 to support major mods; option to choose version
- [ ] KubeJS integration for Core Client
- [ ] Documented API and modding guide

## Developer Experience
- [ ] Content pack system for APWorld templates
- [ ] APWorld template generation

## Backport Requests

These backports should eventually become available when we stabilize the core and vanilla APIs.

- [ ] Forge 1.16.5 + KubeJS Addon for Create Above and Beyond (@Treeways)
- [ ] Cursed Fabric Loader 1.5.2 for Better Than Wolves: Community Edition (@Patchwork)
  - [BTW CE Repository](https://github.com/BTW-Community/BTW-Public?tab=readme-ov-file)
- [ ] Forge 1.7.10 for GregTech New Horizons (multi-developer effort; we need to put together a team for this)
  - [1.7.10 ExampleMod](https://github.com/GTNewHorizons/ExampleMod1.7.10) | [GTNH Modding Guide](https://gtnh.miraheze.org/wiki/Development)

## For Future Consideration
- [ ] Sanities: Biomesanity (cannot enter specific biome without its item)
- [ ] DX: DSL for representing large logic chains in Archipelago worlds
