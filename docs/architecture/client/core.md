---
sidebar_position: 1
---

# Core Client

The Core Client is a generic middleware interface for Archipelago.
It relays signals from an Archipelago server to mods that integrate
[mapping](/docs/architecture/archipelago/mappings) handlers with its API.

This makes the core client fully generic, making it highly portable to various game versions and mod loaders
without needing to port implementation details to different game versions for every supported modpack.

This mod is written in Kotlin, but does not require any Kotlin mod dependencies to run properly.

## Integration

[//]: # (TODO: Elaborate and verify this part)

When the player joins a world,
the core client reads the [mappings](/docs/architecture/archipelago/mappings) of a multiworld,
registering data correspondingly with addon mods that register these mapped-out calls.

For item mappings, the client will return a handler for a specified call
for the client integration mod to interpret and handle.

For location mappings, an event handler will be provided for sending that location.

:::warning
Types and their namespaces are reserved for their respective mod,
and should not be registered internally more than once.
If you need to interpret an item call, please initialize your own mod's handler for that purpose.
:::
