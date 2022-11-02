---
layout: default
title: Game Initialization File
parent: Server Configurations
grand_parent: Server Information
nav_order: 2
---

# **Game Initialization File**
{: .fs-9 .fw-600 }
-----

The `game.ini` is a initialization file which can be modified to run the server. It is one of the core files to have and is required to run the server. This file is located in the **ServerConfig** folder.

**_NOTE: This settings can only be configured if `fullsynchronization 1` is set in `server.cfg`._**

-----
# <img src="/assets/icons/wizard.png" width="32" height="32" /> **Player Configurations**

The configurations listed below ONLY affects the player behaviors, and not the server.

-----
## **FallDamage**
Enable/Disable fall damage feautures for player.

Example:
```go
//Set by default.
falldamage = 0
```

-----
## **Prediction**
Enable/Disable server checks for prediction of players movement. 

**_NOTE: This feature does not work and is no longer in use!!_**

Example:
```go
//Set by default. 
prediction = 0
```

-----
## **Interpolation**
Enable/Disable smooth movements from player. May impact performance.

Example:
```go
//Disables smooth player movement. Set by default.
interpolation = 0
//Enables smooth player movement.
interpolation = 1
```

-----
## **PlayerToPlayerCollision**
Enable/Disable collision between players in the server. 

**_NOTE: This feature only works if `interpolation = 1` is set._**

Example:
```go
//Disables collision between players. Set by default.
playertoplayercollision = 0
//Enables collision between players. Recommended for public servers.
playertoplayercollision = 1
```

-----
# <img src="/assets/icons/gear.png" width="32" height="32" /> **Server Configurations**

The configurations listed below affects the server behaviors. Performance will vary.

-----
## **FrameLimit**
Sets the optimizatized framerate for the server.

**_Note: If the framelimit is set below 60, the server may experience some bugs from collision!_**

Example:
```go
//Set by default.
framelimit = 300
```

-----
## **ThroughWallsBulletAntiCheat**
Enable/Disable anti-cheat for projectile bullets in the server.

Example:
```go
//Set by default.
throughwallsbulletanticheat = 0
```
-----
## **ItemsRaycastCollision**
Sets the Raycasting Collision for items.

**_NOTE: This feature has been locked and fixed to output the maximum quality._**

Example:
```go
//Set by default.
itemsraycastcollision = 1
```

-----
## **FixedTimeSteps**
Sets fixed time steps.

Example:
```go
//Set by default.
fixedtimesteps = 0
```

-----
## **DeltaLimit**
Sets how many actions will happen during a lag. 

Example:
```go
//Set by default. DO NOT change unless you know what you are doing!
deltalimit = 5.0
```

-----
## **MaxPlayersSpawn**
Sets how many players will spawn as either MTF or Chaos during a spawn wave.

Example:
```go
//Sets to spawn 8 players during the spawn wave. Set by default.
maxplayersspawn = 8
```

-----
## **FriendlyFire**
Enable/Disable friendly fire in the server.

Example:
```go
//Disables friendly fire. Set by default.
friendlyfire = 0
//Enables friendly fire.
friendlyfire = 1
```