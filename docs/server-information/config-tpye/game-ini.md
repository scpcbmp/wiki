---
layout: default
title: Game Initialization File
parent: Server Configuration
grand_parent: Server Information
nav_order: 2
---

# **Game Initialization File**
{: .fs-9 .fw-600 }
-----

The `game.ini` is a initialization file which can be modified to run the server. It is one of the core files to have and is required to run the server. This file is located in the **ServerConfig** folder.

**_NOTE: This settings can only be configured if `fullsynchronization 1` is set in `server.cfg`._**

-----
# <img src="https://cdn-icons-png.flaticon.com/512/2579/2579208.png" width="26" height="26" /> **Player Configurations**

The configurations listed below ONLY affects the player behaviors, and not the server.

-----
## Falldamage
Enable/Disable fall damage feautures for player.

Example:
```go
//Set by default.
falldamage = 0
```

-----
## Prediction
Enable/Disable server checks for prediction of players movement. 

Example:
```go
//Set by default.
prediction = 0
```

-----
## Interpolation
Enable/Disable smooth movements from player.

Example:
```go
//Set by default.
interpolation = 0
```

-----
## Playertoplayercollision
Enable/Disable collision between players in the server.

Example:
```go
//Set by default.
playertoplayercollision = 1
```

-----
# <img src="https://cdn-icons-png.flaticon.com/512/484/484562.png" width="26" height="26" /> **Server Configurations**

The configurations listed below affects the server behaviors. Performance may vary.

-----
## Framelimit
Sets the optimizatized framerate for the server.

Example:
```go
//Set by default.
framelimit = 5000
```

-----
## Throughwallsbulletanticheat
Enable/Disable anti-cheat for projectile bullets in the server.

Example:
```go
//Set by default.
throughwallsbulletanticheat = 0
```