---
layout: default
title: Server Configuration File
parent: Server Configuration
grand_parent: Server Information
nav_order: 1
---

# **Server Configuration File**
{: .fs-9 .fw-600 }
----

The `server.cfg` is a configuration file which can be modified to run the server. It is one of the core files to have and is required to run the server. This file is located in the **root** folder.

**_NOTE: For new users, please read thoroughly when setting up a server._**

-----
# <img src="https://cdn-icons-png.flaticon.com/512/4295/4295919.png" width="26" height="26" /> **Basic**

Some of the configuration settings listed below will have a star (<img src="https://cdn-icons-png.flaticon.com/512/616/616489.png" width="16" height="16" />) marker next to them. This will indicate as a requirement for new or returning users who are setting up a server needs to change the following settings.

-----
## **HostName**
Sets the name of the server that will be displayed in the Multiplayer Menu navigation screen.

Example:
```go
//This will be displayed on the front Multiplayer Page.
hostname SCP Vanilla Server
```

-----
## **Port**
Sets the server port number to broadcast to.

Example:
```go
//ONLY CHANGE THIS IF YOU ARE CREATING MORE THAN ONE (1) SERVER.
//Server 1 Config. Set by default.
port 50021
//Server 2 Config
port 50022
```

-----
## **MapSeed**
Sets the seed generation of the server, leave blank for a more random generation.

Example: 
```go
//By default, mapseed is not set.
mapseed
//You write anything in mapseed and the server will generate it. 
mapseed WhatEverTheSeedIWant
mapseed c93w99wf93ypw9
mapseed IT5M1N34N0M
```

-----
## **NoCheat** <img src="https://cdn-icons-png.flaticon.com/512/616/616489.png" width="16" height="16" />
Enables/Restricts console access in-game for public use.

Example: 
```go
//Console access available to the public. Set by default. NOT RECOMMENDED!
nocheat 0
//Restricts console access to the public. Only available if using RCON Login.
nocheat 1
```

-----
## **Voice**
Enable/Disable voice chat used in-game.

Example: 
```go
//Enables voice chat in-game. Set by default.
voice true
//Disables voice chat in-game.
voice false
```

-----
## **MaxPlayers** <img src="https://cdn-icons-png.flaticon.com/512/616/616489.png" width="16" height="16" />
Sets how many players can be on the server at one time. 

_TIP: The more players there are on the server at once, the more CPU the server takes._

Example: 
```go
//Sets manximum amount of players that can be online at once. 16 is set by default.
maxplayers 16
//Recommended amount for public servers.
maxplayers 32
```

-----
## **JumpMode**
Enable/Disable JUMP feature in-game. However, players can jump into unplayable zones in enabled. By default: true.

Example: `jumpmode true`

-----
## **Difficulty**
Changes the difficulty the server is running. By default: safe.

Example: `difficulty safe`

-----
## **Tickrate**
Changes the tick speed of the server. Impacts the performance. By default: 64.

Example: `tickrate 64`

-----
## **Breach**
Enables or disables the Breach gamemod. By default false.

Example: `breach true`

-----
# <img src="https://cdn-icons-png.flaticon.com/512/4789/4789514.png" width="26" height="26" /> **Advanced**
This options are not required for server to run, however they are useful.

-----
## **Introenabled**
Enable or disable the Intro. By default: 0.

Example: `introenabled 0`

-----
## **Timeout**
Changes the time required to time out. By default: 60000.

Example: `timeout 60000`

-----
## **Password**
Sets the password for the server. By default: Isn't set.

Example: `password SuperStrongPassword`

-----
## **Gravity**
Change gravity on server, avoid putting high numbers. By default: 0.0023.

Example: `gravity 0.0023`

-----
## **Rconpassword**
Enable/change the rcon console password. By default: Isn't set.

Example: `rconpassword StrongPassword123`

-----
## **Keepinventory**
Enable or disable keep inventory feature. By default: 0.

Example: `keepinventory 1`

-----
## **Mapsize**
Change the map size. By default: 4.

Example: `mapsize 2`

-----
## **Gamestate**
Change the game state of the server. By default: Isn't set.

Example: `gamestate Started`

-----
## **Description**
Add or change server description. By default: Isn't set.

Example: `description Join this super duper server.`

-----
## **Weburl**
Add or change the server web url. By default: Isn't set.

Example: `weburl https://google.com`

-----
## **Custommap**
Use custom map instead of randomly generated. Warning performance heavy. By default: Isn't set.

Example: `custommap big.cbmap2`

-----
## **Script**
Load server scripts. By default: Isn't set.

Example: `script script fun.gsc`

-----
# Breach mode - 💥
Settings that change breach gamemode a little, settings are not required.

This configuration requires [breach](#breach) to be `true`. Please ensure this is enabled for these settings to take effect.
{: .fs-4 .fw-300 .text-green-100 }

-----
## Breachlight
Makes facility brighter in breach mode. By default: false.

Example: `breachlight true`

-----
## Breachchat
Enables or disables chat in breach gamemod. By default: 1.

Example: `breachchat 1`

-----
## Breachtime
Change the time of the breach mode round. By default: 900000.

Example: `Breachtime 900000`

-----
## Breach_onlydeathmatch
Change breach gamemode to deathmatch one. By default: false.

Example: `breach_onlydeathmatch false`

-----
# Optional - 🔅
This options are optional, and shouldn't be change unless needed.

-----
## Stacksize
Change the stack size in server. By default: Isn't set.

Example: `stacksize 8192`

-----
## Voice_quality
Used to change the voice quality. By default: 44000.

Example: `voice_quality 44000`

-----
## Logsoff
Disable saving of the log file. By default: 0.

Example: `logsoff 0`

-----
## Longculling
Disable culling system, NOT RECOMMENDED. By default: Isn't set.

Example: `longculling 0`