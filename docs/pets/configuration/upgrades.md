---
sidebar_position: 8
title: Upgrades
---

# `upgrades/<name>.json`

| Name | Type | Description |
| --- | --- | --- |
| id | `String` | The identifier |
| pet | `String` | The pet |
| rarity | `String` | The rarity |
| item | `ItemWrapper` | The item |
| recipe | `Recipe` | The crafting recipe |

```json
{
  "id": "TIGER_LEGENDARY_UPGRADE",
  "pet": "TIGER",
  "rarity": "LEGENDARY",
  "item": {
    "material": "EMERALD_BLOCK",
    "name": "%gold%Legendary Tiger Upgrade",
    "lore": [
      "%gray%Upgrades your %gold%Tiger %gray%to %gold%Legendary%gray%!",
      "%dark_gray%Right-click to use."
    ],
    "glowing": true
  },
  "recipe": {
    "shape": [
      "ded",
      "gng",
      "ded"
    ],
    "ingredients": {
      "d": "DIAMOND_BLOCK",
      "e": "EMERALD_BLOCK",
      "g": "GOLD_BLOCK",
      "n": "NETHER_STAR"
    }
  }
}
```
