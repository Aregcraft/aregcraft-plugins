---
sidebar_position: 6
title: abilities.json
---

# `abilities.json: List<Ability>`

| Name | Type | Description | Optional | Default |
| --- | --- | --- | --- | --- |
| base | `String` | The base from which to inherit other properties | No | N/A |
| id | `String` | The identifier | No | N/A |
| name | `String` | The name, can have colors | Yes | The identifier |
| description | `List<String>` | The description, can have colors | Yes | None |
| price | `Price` | The amount of health and hunger deducted from the player upon activation | No | N/A |
| cooldown | `long` | The cooldown in ticks (1 second = 20 ticks) | Yes | 0 |

```json
[
  {
    "base": "Projectile",
    "id": "WITHER",
    "name": "%red%Wither",
    "description": [
      "%gray%Shoots wither skulls!"
    ],
    "price": {
      "health": 4,
      "food": 4
    },
    "cooldown": 60,
    "type": "WITHER_SKULL",
    "velocity": {
      "x": 2,
      "y": 2,
      "z": 2
    }
  },
  {
    "base": "Effect",
    "id": "REGENERATION",
    "name": "%red%Regeneration",
    "description": [
      "%gray%Gives you regeneration 2 for 5 seconds!"
    ],
    "price": {
      "food": 8
    },
    "cooldown": 200,
    "type": "minecraft:regeneration",
    "duration": 100,
    "amplifier": 1,
    "hideParticles": true
  },
  {
    "base": "Freeze",
    "id": "FREEZE",
    "name": "%blue%Freeze",
    "description": [
      "%gray%Throws a snowball that freezes the",
      "%gray%hit entity for 5 seconds!"
    ],
    "price": {
      "health": 8,
      "food": 8
    },
    "cooldown": 200,
    "projectileType": "SNOWBALL",
    "projectileVelocity": {
      "x": 2,
      "y": 2,
      "z": 2
    },
    "duration": 100
  },
  {
    "base": "Rage",
    "id": "RAGE",
    "name": "%red%Rage",
    "description": [
      "%gray%Gives you strength 2 for 5 seconds",
      "%gray%but reflects 25% of the damage",
      "%gray%you deal!"
    ],
    "price": {
      "health": 4,
      "food": 4
    },
    "cooldown": 200,
    "duration": 100,
    "amplifier": 1,
    "multiplier": 0.25
  },
  {
    "base": "Storm",
    "id": "STORM",
    "name": "%gray%Storm",
    "description": [
      "%gray%Summons a circle of lighting bolts",
      "%gray%around you!"
    ],
    "price": {
      "health": 4,
      "food": 4
    },
    "cooldown": 200,
    "function": {
      "x": "2cos(t)",
      "z": "2sin(t)",
      "min": 0,
      "max": 6.28318530718,
      "delta": 0.78539816339
    }
  },
  {
    "base": "Shield",
    "id": "SHIELD",
    "name": "%green%Shield",
    "description": [
      "%gray%Makes you invincible to mobs and players",
      "%gray%but also prevents you from attacking them!"
    ],
    "price": {
      "health": 4,
      "food": 4
    },
    "cooldown": 200,
    "duration": 200,
    "function": {
      "x": "cos(10t)",
      "y": "t",
      "z": "sin(10t)",
      "min": 0,
      "max": 2,
      "delta": 0.1
    },
    "particle": "ENCHANTMENT_TABLE",
    "disableAttack": true
  },
  {
    "base": "SeismicWave",
    "id": "SEISMIC_WAVE",
    "name": "%green%Seismic Wave",
    "description": [
      "%gray%Damages and knocks back all mobs and",
      "%gray%players within five blocks!"
    ],
    "price": {
      "health": 4,
      "food": 4
    },
    "cooldown": 60,
    "function": {
      "x": "tcos(2t)",
      "z": "tsin(2t)",
      "min": 0,
      "max": 6.28318530718,
      "delta": 0.19634954084
    },
    "particle": "EXPLOSION_NORMAL",
    "knockback": {
      "x": 1,
      "y": 1,
      "z": 1
    },
    "height": 0.5,
    "damage": 5,
    "range": 5
  },
  {
    "base": "Throw",
    "id": "THROW",
    "name": "%red%Throw",
    "description": [
      "%gray%Throws your weapon for 2 seconds",
      "%gray%dealing 75% of its damage!"
    ],
    "price": {
      "health": 4,
      "food": 4
    },
    "cooldown": 100,
    "duration": 40,
    "velocity": {
      "x": 2,
      "y": 2,
      "z": 2
    },
    "damageMultiplier": 0.75
  },
  {
    "base": "Pawn",
    "id": "PAWN",
    "name": "%green%Pawn",
    "description": [
      "%gray%Summons two zombies with 150% of the",
      "%gray%health of a normal one attacking",
      "%gray%other players for 10 seconds!"
    ],
    "price": {
      "health": 6,
      "food": 6
    },
    "cooldown": 400,
    "duration": 200,
    "entity": {
      "type": "ZOMBIE",
      "name": "%red%%player%'s Pawn",
      "nameVisible": true,
      "attributeModifiers": {
        "GENERIC_MAX_HEALTH": [
          {
            "name": "minecraft.generic_max_health",
            "amount": 30
          }
        ]
      },
      "helmet": {
        "material": "LEATHER_HELMET"
      }
    },
    "number": 2
  },
  {
    "base": "Teleport",
    "id": "TELEPORT",
    "name": "%green%Teleport",
    "description": [
      "%gray%Teleports you in your looking direction",
      "%gray%up to 4 blocks!"
    ],
    "price": {
      "health": 4,
      "food": 4
    },
    "cooldown": 60,
    "distance": 4
  },
  {
    "base": "Potion",
    "id": "POTION",
    "name": "%gray%Potion",
    "description": [
      "%gray%Throws a potion with poison 1 for 5",
      "%gray%seconds!"
    ],
    "price": {
      "health": 4,
      "food": 4
    },
    "cooldown": 100,
    "type": "minecraft:poison",
    "duration": 100,
    "amplifier": 0,
    "hideParticles": false,
    "velocity": {
      "x": 1,
      "y": 1,
      "z": 1
    }
  },
  {
    "base": "Fire",
    "id": "FIRE",
    "name": "%gold%Fire",
    "description": [
      "%gray%Summons a vortex of fire that ignites",
      "%gray%everyone on its way for 5 seconds!"
    ],
    "price": {
      "health": 4,
      "food": 4
    },
    "cooldown": 100,
    "function": {
      "x": "0.5tcos(6t)",
      "y": "0.5tsin(6t)",
      "z": "t",
      "min": 0,
      "max": 3.14159265359,
      "delta": 0.09817477042
    },
    "particle": "FLAME",
    "fireDuration": 100
  },
  {
    "base": "Evoker",
    "id": "EVOKER",
    "name": "%gray%Evoker",
    "description": [
      "%gray%Summons 16 evoker fangs in your looking",
      "%gray%direction!"
    ],
    "price": {
      "health": 4,
      "food": 4
    },
    "cooldown": 100,
    "number": 16
  },
  {
    "base": "Dash",
    "id": "DASH",
    "name": "%green%Dash",
    "description": [
      "%gray%Rapidly moves you in your looking",
      "%gray%direction!"
    ],
    "price": {
      "food": 4
    },
    "cooldown": 60,
    "velocity": {
      "x": 2,
      "y": 2,
      "z": 2
    }
  },
  {
    "base": "Reveal",
    "id": "REVEAL",
    "name": "%blue%Reveal",
    "description": [
      "%gray%Reveals all invisible mobs and players",
      "%gray%within ten blocks!"
    ],
    "price": {
      "health": 4,
      "food": 4
    },
    "cooldown": 200,
    "range": 10
  },
  {
    "base": "Explosion",
    "id": "EXPLOSION",
    "name": "%red%Explosion",
    "description": [
      "%gray%Creates an explosion around you without",
      "%gray%destroying the block below you!"
    ],
    "price": {
      "health": 6,
      "food": 6
    },
    "cooldown": 200,
    "power": 5
  },
  {
    "base": "Thorns",
    "id": "THORNS",
    "name": "%green%Thorns",
    "description": [
      "%gray%Reflects 25% of the damage you receive",
      "%gray%for 5 seconds!"
    ],
    "price": {
      "health": 4,
      "food": 4
    },
    "cooldown": 200,
    "duration": 100,
    "multiplier": 0.25
  },
  {
    "base": "Fly",
    "id": "FLY",
    "name": "%green%Fly",
    "description": [
      "%gray%Boosts you in your looking direction",
      "%gray%and makes you glide as if you were",
      "%gray%wearing elytra!"
    ],
    "price": {
      "food": 8
    },
    "cooldown": 400,
    "duration": 200,
    "velocity": {
      "x": 4,
      "y": 4,
      "z": 4
    }
  },
  {
    "base": "Spectate",
    "id": "SPECTATE",
    "name": "%red%Spectate",
    "description": [
      "%gray%Gives you spectator mode for 5 seconds",
      "%gray%but returns you to your initial location!"
    ],
    "price": {
      "health": 10,
      "food": 10
    },
    "cooldown": 400,
    "duration": 100
  },
  {
    "base": "Cocoon",
    "id": "COCOON",
    "name": "%green%Cocoon",
    "description": [
      "%gray%Puts you inside an obsidian cocoon",
      "%gray%without breaking existing blocks!"
    ],
    "price": {
      "health": 8,
      "food": 8
    },
    "cooldown": 400,
    "block": "OBSIDIAN"
  }
]
```