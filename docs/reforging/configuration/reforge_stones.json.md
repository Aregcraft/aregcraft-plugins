---
sidebar_position: 5
title: Stones
---

# `stones/<name>.json`

| Name | Type | Description |
| --- | --- | --- |
| id | `String` | The identifier of the reforge |
| item | `ItemWrapper` | The item |
| recipe | `Recipe` | The crafting recipe |

```json
{
  "id": "MURDEROUS",
  "item": {
    "material": "SKELETON_SKULL",
    "name": "%red%Cracked Skull",
    "lore": [
      "%gray%Use this item on a reforging anvil to",
      "%gray%obtain %red%Murderous %reset%%gray%reforge!"
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
}
```
