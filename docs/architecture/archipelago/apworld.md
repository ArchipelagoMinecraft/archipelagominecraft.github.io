---
sidebar_position: 1
---

# APWorld

We're working on providing pluggable tools for generating APWorlds,
which allow for the swift bootstrapping of a modpack's randomizer.

## Template World

An APWorld template will eventually be provided that implements a base for the following features,
as well as a CLI to help bootstrap a new APWorld for your game version and mod loader.

## Raw Input Data

A data exporter will be ported to your game version. Raw data should include:

- Registry entries
  - Entities
    - Mob drops
  - Blocks
    - Block drops and their requirements
- Data entries
  - Crafting recipes
  - Achievements

This raw data can then be manipulated by the APWorld and randomized for your modpack.

:::warning

If you are building a randomizer for a mod that does not integrate into standard game or mod APIs,
especially for game versions &lt;=1.8.9, then our support may be limited.
You may have to export game data manually, or write your own exporter that is tailored for your mod.

:::

## Logic Paks

Standard Minecraft APWorlds will include isolated, modular portions of logic called logic paks.
All logic paks will be derived from a raw export of your modpack's data.
Then they will be combined into the final logic from the root of the APWorld with a mixin-esque system.
Paks are designed to be overridden or added onto by other paks when the need to do so arises.

## DSL Support

Currently in consideration for development is an external DSL made specifically for Archipelago
which works in tandem with logic paks.
It would be specially designed for implementing huge modpacks with a simple-yet-robust syntax.
