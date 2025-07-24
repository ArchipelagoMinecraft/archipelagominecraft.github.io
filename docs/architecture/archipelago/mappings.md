---
sidebar_position: 3
---

# Mappings

Once game generation is finished, mapping definitions for each item/location
will be written into a `.json` file,
which is placed in the [`.apmcbundle`](/docs/architecture/archipelago/apmcbundle).

This mapping is parsed on runtime by the [core client](/docs/architecture/client/core)
to send the right locations and provide proper item rewards.

## List of Types

### Vanilla Items

To be filled out when the API stabilizes.

[//]: # (TODO)

### Vanilla Locations

To be filled out when the API stabilizes.

[//]: # (TODO)

## Specification

```json
{
    "apItems": [
        {
            "id": 0, // ID of an "Item Storage" unlock item, for instance
            "type": [
                // Multiple types are allowed, including custom types
                "apvanilla:recipe",
                "apkubejs:celebration" // Namespace for the KubeJS addon, with a custom handler
            ],
            "data": {
                "recipe": [ "minecraft:chest", "minecraft:ender_chest", "#minecraft:shulker_box" ],

                // This data can be whatever you want, passed into your KubeJS payload
                "celebration": "playsound:yippee"
            },
        }
        {
            // ...
        },
    ],
    "apLocations": [
        {
            "id": 1, // ID for shooting a bow for the first time
            
            // TODO: Support for either predicates,
            // and/or multiple locations and logic gates
            "type": "apvanilla:achievement",
            "data": {
                "condition": "adventure/shoot_arrow",
            }
        },
        {
            // ...
        },
    ],
}
```