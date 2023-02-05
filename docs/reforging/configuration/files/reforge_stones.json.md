---
sidebar_position: 2
title: reforge_stones.json
---

# `reforge_stones.json: List<ReforgeStone>`

| Name | Type | Description |
| --- | --- | --- |
| id | `String` | The identifier of the reforge |
| item | `ItemWrapper` | The item |
| recipe | `Recipe` | The crafting recipe |

```json
[
  {
    "id": "WITHERED",
    "item": {
      "material": "WITHER_SKELETON_SKULL",
      "name": "%light_purple%Wither Blood",
      "lore": [
        "%gray%Use this item on a reforging anvil to",
        "%gray%obtain %light_purple%%bold%Withered %reset%%gray%reforge!"
      ]
    },
    "recipe": {
      "shape": [
        "gdg",
        "dnd",
        "gdg"
      ],
      "ingredients": {
        "g": "GOLD_BLOCK",
        "d": "DIAMOND_BLOCK",
        "n": "NETHER_STAR"
      }
    }
  },
  {
    "id": "TITANIC",
    "item": {
      "material": "ZOMBIE_HEAD",
      "name": "%green%Titan Head",
      "lore": [
        "%gray%Use this item on a reforging anvil to",
        "%gray%obtain %green%%bold%Titanic %reset%%gray%reforge!"
      ]
    },
    "recipe": {
      "shape": [
        "odo",
        "ded",
        "odo"
      ],
      "ingredients": {
        "o": "OBSIDIAN",
        "d": "DIAMOND_BLOCK",
        "e": "EMERALD_BLOCK"
      }
    }
  },
  {
    "id": "MURDEROUS",
    "item": {
      "material": "SKELETON_SKULL",
      "name": "%red%Cracked Skull",
      "lore": [
        "%gray%Use this item on a reforging anvil to",
        "%gray%obtain %red%%bold%Murderous %reset%%gray%reforge!"
      ]
    },
    "recipe": {
      "shape": [
        "igi",
        "gwg",
        "igi"
      ],
      "ingredients": {
        "i": "IRON_BLOCK",
        "g": "GOLD_BLOCK",
        "w": "WITHER_SKELETON_SKULL"
      }
    }
  },
  {
    "id": "PUPPETEER",
    "item": {
      "material": "STRING",
      "name": "%green%Puppeteer String",
      "lore": [
        "%gray%Use this item on a reforging anvil to",
        "%gray%obtain %green%%bold%Puppeteer %reset%%gray%reforge!"
      ]
    },
    "recipe": {
      "shape": [
        "cdc",
        "ded",
        "cdc"
      ],
      "ingredients": {
        "c": "COBWEB",
        "d": "DRAGON_BREATH",
        "e": "ELYTRA"
      }
    }
  },
  {
    "id": "EXPLOSIVE",
    "item": {
      "material": "GUNPOWDER",
      "name": "%red%Creeper Gunpowder",
      "lore": [
        "%gray%Use this item on a reforging anvil to",
        "%gray%obtain %red%%bold%Explosive %reset%%gray%reforge!"
      ]
    },
    "recipe": {
      "shape": [
        "gdg",
        "ded",
        "gdg"
      ],
      "ingredients": {
        "g": "GUNPOWDER",
        "d": "DIAMOND_BLOCK",
        "e": "ELYTRA"
      }
    }
  },
  {
    "id": "SPECTACULAR",
    "item": {
      "material": "ENDER_EYE",
      "name": "%red%All-Seeing Eye",
      "lore": [
        "%gray%Use this item on a reforging anvil to",
        "%gray%obtain %red%%bold%Spectacular %reset%%gray%reforge!"
      ]
    },
    "recipe": {
      "shape": [
        "ddd",
        "nen",
        "ddd"
      ],
      "ingredients": {
        "d": "DIAMOND_BLOCK",
        "n": "NETHER_STAR",
        "e": "ELYTRA"
      }
    }
  }
]
```