---
layout: default
title: Global Variables
parent: Scripting Language
has_children: false
nav_order: 6
---

## <img src="https://cdn-icons-png.flaticon.com/512/2763/2763281.png" width="32" height="32" /> **Global Variables**
{: .fs-7 }

Tip: Adding the following command to your script `#include "includes\multiplayer_core.inc"` allows you to use variable names directly.
{: .fs-4 .fw-300 .text-green-100 }

| Game Limitations | Assigned Value |
|:-------------|:------------------|
| MAX_OBJECTS | 65535 |
| MAX_PLAYERS | 65 |
| MAX_ROOMS | 200 |
| MAX_DOORS | 500 |
| MAX_NPCS | 255 |
| MAX_EVENTS | 110 |
| MAX_ITEMS | 1000 |

| Miscellaneous Limitations | Assigned Value |
|:-------------|:------------------|
| MAX_PLUGINS | 64 |
| MAX_INCLUDES | 64 |

| Variable Limitations | Assigned Value |
|:-------------|:------------------|
| MAX_PLAYER_VARIABLES | 256 |
| MAX_VARIABLES | 512 |

| GUI Limitations | Assigned Value |
|:-------------|:------------------|
| MAX_DRAWS | 32 |
| MAX_TEXTS | 32 |

| Script Limitations | Assigned Value |
|:-------------|:------------------|
| MAX_PUBLICS | INFINITY |
| MAX_PUBLICS_TICKS | 64 |
| MAX_PUBLIC_PARAMS | 16 |

| Anticheat Limitations | Assigned Value |
|:-------------|:------------------|
| CHEAT_NOITEM | 1 |
| CHEAT_INCORRECT_ROLE | 2 |
| CHEAT_INCORRECT_POS | 3 |
| CHEAT_CONSOLE_USE | 4 |
| CHEAT_SPAWN_ITEM | 5 |
| CHEAT_INTERCOM | 6 |
| CHEAT_NORECOILORSPREAD | 7 |

| Plugins Types | Assigned Value |
|:-------------|:------------------|
| P_TYPE_BYTE | 1 |
| P_TYPE_SHORT | 2 |
| P_TYPE_INT | 3 |
| P_TYPE_FLOAT | 4 |
| P_TYPE_STRING | 5 |

| Player Animations | Assigned Value |
|:-------------|:------------------|
| PLAYER_SITTING_IDLIN | 5 |
| PLAYER_SITTING_WALKING_LEFT | 7 |
| PLAYER_SITTING_WALKING_RIGHT | 8 |
| PLAYER_SITTING_WALKING_BACK | 9 |
| PLAYER_SITTING_WALKING_FORWARD | 10  |
| PLAYER_IDLING | 11 |
| PLAYER_WALKING | 12 |
| PLAYER_RUNNING | 13 |
| PLAYER_CRYING | 14 |

| Player Armament | Assigned Value |
|:-------------|:------------------|
| GUN_USP | 1 |
| GUN_P90 | 2 |
| GUN_MP5SD | 3 |
| GUN_BAZOOKA | 4 |
| GUN_MINIGUN | 5 |
| GUN_MICROHID | 6 |
| GUN_DEAGLE | 7 |
| GUN_SHOTGUN | 8 |
| GUN_HKG36 | 9 |
| GUN_M4A4 | 10 |
| GUN_HANDCUFFS | 11 |
| GUN_KNIFE | 12 |
| GUN_GRENADE | 13 |
| GUN_GRENADEFLASHBANG | 14 |
| GUN_GRENADESMOKE | 15 |

| Class Types | Assigned Value |
|:-------------|:------------------|
| TYPE_SPECTATOR | 0 |
| TYPE_NTF | 1 |
| TYPE_GUARD | 2 |
| TYPE_CLASSD | 3 |
| TYPE_SCIENTIST | 4 |
| TYPE_173 | 5 |
| TYPE_049 | 6 |
| TYPE_CHAOS | 7 |
| TYPE_JANITOR | 8 |
| TYPE_JANITOR | 9 |
| TYPE_939 | 10 |
| TYPE_106 | 11 |
| TYPE_966 | 12 |
| TYPE_ZOMBIE | 13 |
| TYPE_096 | 14 |
| TYPE_860 | 15 |
| TYPE_035 | 16 |
| TYPE_LOBBY | 17 |

| Collisions | Assigned Value |
|:-------------|:------------------|
| HIT_MAP | 1 |
| HIT_PLAYER | 2 |
| HIT_ITEM | 3 |
| HIT_APACHE | 4 |
| HIT_DEAD | 6 |
| HIT_GRENADE | 8 |
| HIT_INVISIBLEWALL | 9 |
| HIT_DOOR | 11 |
| HIT_OLDMAN | 12 |


| Drawing Types | Assigned Value |
|:-------------|:------------------|
| DRAW_IMAGE  | 0 |
| DRAW_RECT | 1 |
| DRAW_OVAL | 2 |
| DRAW_IMAGE_STANDART_SIZE | -1 |