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
We also want to support a wide variety of different modpacks.
These goals require a well-designed framework.

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

The code architecture between these two Archipelago clients is very different under the hood,
and the goals we have aren't aligned.

(In technical terms: Due to our modular philosophy, much of the original client code would need
a big split and refactor to work with the data model we've implemented.)

Nevertheless, we respect the fork's maintainers immensely for their efforts on bringing it back soon,
and we're excited to see the release of their mod when it's ready.
They're currently working on supporting Archipelago 0.6.2, so please look forward to it!

We're rewriting the vanilla APWorld alongside the mod client (which is being written in Kotlin)
to maintain full parity with the original randomizer,
with added features, better version support,
and further improvements on a new implementation that is more futureproof.

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
