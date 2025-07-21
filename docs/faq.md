---
sidebar_position: 3
---

# FAQ

:::warning

This project is in a heavy pre-production state.
All information on this wiki is subject to change!

Please leave any feedback at https://discord.gg/archipelago
(find us in
[`#minecraft` in the Minecraft Client 2.0 thread](https://discord.com/channels/731205301247803413/1394782863135608832/1394783006849368065)).

:::

## What's the basic TL;DR of this project?

This is a project that aims to make the Minecraft randomizer more flexible for a variety of different randomizers.

We're doing this so that it's easier to maintain and port to different versions in the long run.
We also want to support a wide variety of different modpacks, so we're working on a very cohesive framework.

## Who's working on this?

Currently:
- `@Treeways` working on this wiki and planning
- `@LelouBil` on the initial client code and planning
- `@studkid` with planning

Feel free to check out our [GitHub organization](https://github.com/ArchipelagoMinecraft).

Thanks to everyone who's given us support and feedback over the course of development!

## When will this be done?

There is lots to be designed and implemented, so it's impossible to tell at the moment. When it's done, it's done.

## How can I help?

Thanks for asking.
Feel free to skim through the documentation - there is plenty to work on at the moment.

If you'd rather work with modpacks later on,
you can let us know what version you want to see a backport for.

If you think you could help, let us know what you want to work on at
https://discord.gg/archipelago (`#minecraft` in the "Minecraft Client 2.0" thread).
We are very open to feedback!

## Will you consolidate with the current NeoForge fork of Kono's randomizer?

A port of that client would certainly be possible to integrate with our
[core client](/docs/architecture/client/core) (by design);
however, using our framework is not in their best interest at the moment,
so we are working on our own vanilla implementation in Kotlin.

Regardless, they're working on supporting Archipelago 0.6.2,
so look forward to that at some point.

For now, we're planning our vanilla APWorld rewrite to have full parity with the original randomizer,
implement more features, fix old problems, and work on top of an implementation that's easier to maintain,
and backed by more research.

See the [roadmap](/docs/roadmap) for more details.

## How do I play/where can I find more about the original randomizer?

Please see the
[AP Minecraft FAQ Google Doc](https://docs.google.com/document/d/1AMcototDovob8YJ7w4UFKAiUMCV21uQjJqzw_dr-sJQ/).

## Could you add a new feature, or port the client to support a modpack I want to work on?

We'd be happy to add new vanilla features and provide additional modded support.
We also have a list of features to implement, and a few backports to support,
as listed on the [roadmap](/docs/roadmap).

Definitely let us know at
https://discord.gg/archipelago (`#minecraft` in the "Minecraft Client 2.0" thread).
