---
sidebar_position: 1
---

# Core Client

The APMC Core Client is a generic interface for Archipelago written in Kotlin.
It relays signals from an Archipelago server to mods that integrate with its API.
Its generic nature makes it highly portable to various game versions and mod loaders.
Addon mods should implement calls from within their own version/loader's ecosystem.

:::info

The Core Client is middleware which does nothing on its own. It needs to be integrated with other mods to function.

:::

## Integration

On game load, the core client takes the [mappings](/docs/architecture/archipelago/mappings) of a multiworld
and registers its data correspondingly. Addon mods should register individual calls by namespace and type.
The client will then return a handler for a specified call,
sending and receiving multiworld items of its type to that handler.
