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

Some of the configuration settings listed below will have a star (<img src="https://cdn-icons-png.flaticon.com/512/616/616489.png" width="16" height="16" />) marker next to them. This will serve as a recommendation for new or returning users who are configuring a server may need the following settings to be changed if applicable.

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
```

-----
## **NoCheat** <img src="https://cdn-icons-png.flaticon.com/512/616/616489.png" width="16" height="16" />
Enables/Restricts console access in-game for public use.

Example:
```go
//Console access available to the public. Set by default. NOT RECOMMENDED!
nocheat false
//Restricts console access to the public. Only available if using RCON Login.
nocheat true
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

**_NOTE: The more players there are on the server at once, the more CPU the server consumes._**

Example:
```go
//Sets manximum amount of players that can be online at once. 16 is set by default.
maxplayers 16
//Recommended amount for public servers.
maxplayers 32
```

-----
## **Password**
Sets the password for the server. 

Example:
```go
//By default, no password is set.
password
//ONLY make up a password if you are setting the server up for private uses or for other reasons.
password Sup3r5tr0ngP4ssw0rd
```

-----
## **RconPassword** <img src="https://cdn-icons-png.flaticon.com/512/616/616489.png" width="16" height="16" />
Sets the RCON console password. Used to gain "Administration" power via command "/rcon (password)" in the multiplayer chat.

Example:
```go
//By default, there is no password set. NOT RECOMMENDED FOR PUBLIC SERVER!!!
rconpassword
//HIGHLY recommended to set a password for PUBLIC SERVERS!
rconpassword Sup3r5tr0ngP4ssw0rd
```

-----
## **JumpMode**
Enable/Disable the jumping feature in-game. However, players can jump into unplayable zones if enabled.

Example:
```go
//Enables the jumping feature in game. Set by default.
jumpmode true
//Disables the jumping feature in game.
jumpmode false
```

-----
## **Difficulty**
Changes the difficulty of the game in the server.

Example:
```go
//Set the server difficulty to SAFE(Easy). Set by default.
difficulty safe
//Set the server difficulty to EUCLID(Normal).
difficulty euclid
//Set the server difficulty to KETER(Hard).
difficulty keter
```

-----
## **Breach** <img src="https://cdn-icons-png.flaticon.com/512/616/616489.png" width="16" height="16" />
Enable/Disable the Breach gamemode.

Example:
```go
//Disables the Breach gamemode. Set by default.
breach false
//Enables the Breach gamemode.
breach true
```

-----
# <img src="https://cdn-icons-png.flaticon.com/512/4789/4789514.png" width="26" height="26" /> **Advanced**

These sets of options are more technical and can impact how the server functions.

-----
## **IntroEnabled**
Enable/Disable the game introduction (This option is similar to the singleplayer introduction).

Example:
```go
//Disables the game introduction. Set by default.
introenabled false
//Enables the game introduction.
introenabled true
```

-----
## **Timeout**
Changes the time value required before a player to times out.

Example:
```go
//Set by default.
timeout 60000 //60000 (milliseconds) <-> 60 (seconds)
```

-----
## **KeepInventory**
Enable/Disable keep inventory feature.

Example:
```go
//Disables keep inventory feature. Set by default.
keepinventory false
//Enables keep inventory feature.
keepinventory true
```

-----
## **MapSize**
Changes the size of the map generation.

Example:
```go
//Set by default.
mapsize 4
//Recommended for smaller and quicker gameplay.
mapsize 2
```

-----
## **GameState**
Changes the game state of the server.

Example:
```go
//By default, there is no state set.
gamestate
//Sets the game state to "OPEN".
gamestate Open
//Sets the game state to "STARTED".
gamestate Started
```

-----
## **Description**
Sets the description of the server.

Example:
```go
//By default, there is no description set.
description
//Set the description text. 
description This is an awesome server!
```

-----
## **WebURL**
Sets the server web url.

Example:
```go
//By default, there is no website url set.
weburl
//Set the link of the url.
weburl https://google.com/
```

-----
## **CustomMap**
Sets and loads a custom map into the server. Performance will vary.

Example:
```go
//By default, there is no map set.
custommap
//Set the name of the map to load.
custommap big.cbmap2
```

-----
## **Script**
Sets and loads a script into the server.

Example:
```go
//By default, there is no script set.
script
//Set the name of the script to load.
script nameofthefile.gsc
//or...
scripttext nameofthefile.gsc
```

-----
# <img src="https://cdn-icons-png.flaticon.com/512/2195/2195441.png" width="26" height="26" /> **Expert**
This options are optional, and shouldn't be change unless needed.

-----
## **TickRate**
Changes the tick speed of the server. Performance will vary.

Example:
```go
//Set by default.
tickrate 64
```

-----
## **Gravity**
Changes the gravity on server, mainly affecting `jumpmode`.

Example:
```go
//Avoid using high numbers. DO NOT change unless you know what you are doing! Set by default.
gravity 0.0023
```

-----
## StackSize
Sets the stack size in server.

Example:
```go
//By default, there is no size set.
stacksize
//Set the stack size.
stacksize 8192
```

-----
## VoiceQuality
Sets the voice quality for the server.

**_NOTE: This feature has been locked and fixed to output the maximum quality._**

Example:
```go
//Set by default.
voice_quality 44000
```

-----
## LogsOff
Enable/Disable log saves for the server.

Example:
```go
//Enables log saving. Set by default.
logsoff false
//Disables log saving.
logsoff true
```

-----
## LongCulling
Disable culling system, NOT RECOMMENDED.

Example:
```go
//Set by default.
longculling 0
```

-----
# <img src="https://cdn-icons-png.flaticon.com/512/1100/1100349.png" width="26" height="26" /> **Breach Mode**

The configuration settings listed below are for `Breach Mode` only. 

This configuration requires [Breach](#breach-) to be `true`. Please ensure this is enabled for these settings to take effect.
{: .fs-4 .fw-300 .text-green-100 }

-----
## BreachLight
Enable/Disable brighter in Breach Mode within the facility.

Example:
```go
//Disables brighter light in Breach Mode. Set by default.
breachlight false
//Enables brighter light in Breach Mode.
breachlight true
```

-----
## BreachChat
Enable/Disable chatting in Breach Mode.

Example:
```go
//Enables chatting feature in Breach Mode. Set by default.
breachchat true
//Disables chatting feature in Breach Mode.
breachchat false
```

-----
## BreachTime
Sets the max time limit of Breach Mode per round.

Example:
```go
//Set by default.
breachtime 900000 // 900000 (milliseconds) <-> 900 (seconds) or 15 (minutes)
```

-----
## BreachOnlyDeathmatch
Enable/Disable the Breach Mode to deathmatch only.

Example:
```go
//Disable Deathmatch-only mode. Set by default.
breach_onlydeathmatch false
//Enables Deathmatch-only mode.
breach_onlydeathmatch true
```