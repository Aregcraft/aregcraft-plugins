---
sidebar_position: 4
title: reforges.json
---

# `reforges.json: List<Reforge>`

| Name | Type | Description | Optional |
| --- | --- | --- | --- |
| id | `String` | The identifier | No |
| name | `String` | The name | No |
| attributes | `Map<Attribute, double>` | The attributes with their amounts | No |
| ability | `String` | The identifier of the ability | Yes |

```json
[
  {
    "id": "WITHERED",
    "name": "%light_purple%Withered",
    "attributes": {
      "GENERIC_MAX_HEALTH": 10,
      "GENERIC_ATTACK_DAMAGE": 10,
      "GENERIC_ATTACK_SPEED": 0.2,
      "GENERIC_ARMOR": 4,
      "GENERIC_ARMOR_TOUGHNESS": 2
    },
    "ability": "WITHER"
  },
  {
    "id": "HEALING",
    "name": "%red%Healing",
    "attributes": {
      "GENERIC_MAX_HEALTH": 8,
      "GENERIC_ATTACK_DAMAGE": 2,
      "GENERIC_ATTACK_SPEED": -0.1,
      "GENERIC_ARMOR": 2
    },
    "ability": "REGENERATION"
  },
  {
    "id": "FROST",
    "name": "%blue%Frost",
    "attributes": {
      "GENERIC_MAX_HEALTH": -2,
      "GENERIC_ATTACK_DAMAGE": 2,
      "GENERIC_ARMOR": 4,
      "GENERIC_MOVEMENT_SPEED": -0.025
    },
    "ability": "FREEZE"
  },
  {
    "id": "OUTRAGEOUS",
    "name": "%red%Outrageous",
    "attributes": {
      "GENERIC_MAX_HEALTH": -4,
      "GENERIC_ATTACK_DAMAGE": 4,
      "GENERIC_ATTACK_SPEED": 0.2,
      "GENERIC_MOVEMENT_SPEED": 0.025
    },
    "ability": "RAGE"
  },
  {
    "id": "CLOUDY",
    "name": "%gray%Cloudy",
    "attributes": {
      "GENERIC_MAX_HEALTH": -4,
      "GENERIC_ATTACK_DAMAGE": 6,
      "GENERIC_ATTACK_SPEED": 0.1
    },
    "ability": "STORM"
  },
  {
    "id": "SHIELDED",
    "name": "%green%Shielded",
    "attributes": {
      "GENERIC_MAX_HEALTH": 8,
      "GENERIC_ARMOR": 4,
      "GENERIC_ARMOR_TOUGHNESS": 2,
      "GENERIC_ATTACK_DAMAGE": -2
    },
    "ability": "SHIELD"
  },
  {
    "id": "TITANIC",
    "name": "%green%Titanic",
    "attributes": {
      "GENERIC_MAX_HEALTH": 6,
      "GENERIC_ARMOR": 6,
      "GENERIC_ARMOR_TOUGHNESS": 3,
      "GENERIC_ATTACK_SPEED": -0.2,
      "GENERIC_MOVEMENT_SPEED": -0.025
    },
    "ability": "SEISMIC_WAVE"
  },
  {
    "id": "MURDEROUS",
    "name": "%red%Murderous",
    "attributes": {
      "GENERIC_ATTACK_DAMAGE": 4,
      "GENERIC_ATTACK_SPEED": 0.2,
      "GENERIC_MAX_HEALTH": -2
    },
    "ability": "THROW"
  },
  {
    "id": "PUPPETEER",
    "name": "%green%Puppeteer",
    "attributes": {
      "GENERIC_MAX_HEALTH": 8,
      "GENERIC_ARMOR": 6,
      "GENERIC_MOVEMENT_SPEED": 0.025
    },
    "ability": "PAWN"
  },
  {
    "id": "STEALTHY",
    "name": "%green%Stealthy",
    "attributes": {
      "GENERIC_MAX_HEALTH": -2,
      "GENERIC_MOVEMENT_SPEED": 0.025,
      "GENERIC_ATTACK_SPEED": 0.1
    },
    "ability": "TELEPORT"
  },
  {
    "id": "WICKED",
    "name": "%gray%Wicked",
    "attributes": {
      "GENERIC_ATTACK_DAMAGE": 2,
      "GENERIC_MAX_HEALTH": -4,
      "GENERIC_ATTACK_SPEED": 0.2
    },
    "ability": "POTION"
  },
  {
    "id": "INFERNAL",
    "name": "%gold%Infernal",
    "attributes": {
      "GENERIC_ATTACK_DAMAGE": 5
    },
    "ability": "FIRE"
  },
  {
    "id": "VENGEFUL",
    "name": "%gray%Vengeful",
    "attributes": {
      "GENERIC_ATTACK_DAMAGE": 4,
      "GENERIC_ATTACK_SPEED": 0.1,
      "GENERIC_MOVEMENT_SPEED": 0.025,
      "GENERIC_MAX_HEALTH": -3
    },
    "ability": "EVOKER"
  },
  {
    "id": "AGILE",
    "name": "%green%Agile",
    "attributes": {
      "GENERIC_MAX_HEALTH": 4,
      "GENERIC_MOVEMENT_SPEED": 0.025
    },
    "ability": "DASH"
  },
  {
    "id": "ENLIGHTENED",
    "name": "%blue%Enlightened",
    "attributes": {
      "GENERIC_MAX_HEALTH": 6
    },
    "ability": "REVEAL"
  },
  {
    "id": "EXPLOSIVE",
    "name": "%red%Explosive",
    "attributes": {
      "GENERIC_MAX_HEALTH": 10,
      "GENERIC_ARMOR": 8,
      "GENERIC_ARMOR_TOUGHNESS": 2
    },
    "ability": "EXPLOSION"
  },
  {
    "id": "SHARP",
    "name": "%green%Sharp",
    "attributes": {
      "GENERIC_MAX_HEALTH": -2,
      "GENERIC_ATTACK_DAMAGE": 2
    },
    "ability": "THORNS"
  },
  {
    "id": "LIGHTWEIGHT",
    "name": "%green%Lightweight",
    "attributes": {
      "GENERIC_MOVEMENT_SPEED": 0.025,
      "GENERIC_ATTACK_DAMAGE": 2
    },
    "ability": "FLY"
  },
  {
    "id": "SPECTACULAR",
    "name": "%red%Spectacular",
    "attributes": {
      "GENERIC_MOVEMENT_SPEED": 0.025,
      "GENERIC_MAX_HEALTH": 8,
      "GENERIC_ARMOR": 8,
      "GENERIC_ARMOR_TOUGHNESS": 4,
      "GENERIC_ATTACK_DAMAGE": 4
    },
    "ability": "SPECTATE"
  },
  {
    "id": "PROTECTED",
    "name": "%green%Protected",
    "attributes": {
      "GENERIC_MAX_HEALTH": 6,
      "GENERIC_ARMOR": 6,
      "GENERIC_ARMOR_TOUGHNESS": 2
    },
    "ability": "COCOON"
  }
]
```