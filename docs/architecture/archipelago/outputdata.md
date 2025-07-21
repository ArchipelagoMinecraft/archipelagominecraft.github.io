---
sidebar_position: 3
---

# Output Data

Once game generation is finished, output data will be written into a data file,
which is placed in the [`.apmcbundle` file](/docs/architecture/archipelago/apmcbundle).

The output data is parsed on runtime by the [core client](/docs/architecture/client/core)
to send the right locations and provide item rewards.

## List of Types

:::warning
Types and their namespaces are reserved for their respective mod,
and should not be registered internally more than once.
If you need to interpret an item call, please initialize your own mod's handler for that purpose.
:::

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