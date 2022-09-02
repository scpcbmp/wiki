---
layout: default
title: Server Configuration File
parent: Server Configurations
grand_parent: Server Information
nav_order: 1
---

# **Server Configuration File**
{: .fs-9 .fw-600 }
-----

The `server.cfg` is a configuration file which can be modified to run the server. It is one of the core files to have and is required to run the server. This file is located in the **root** folder.

**_NOTE: For new users, please read thoroughly when setting up a server._**

-----
# <img src="https://cdn-icons-png.flaticon.com/512/4295/4295919.png" width="32" height="32" /> **Basic**

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
## **Port**
Sets the server port number to broadcast to.

Example:
```go
//ONLY CHANGE THIS IF YOU ARE CREATING MORE THAN ONE (1) SERVER.
//Server 1 Config. Set by default.
port 50021
//Server 2 Config.
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
## **MinPlayersToStart** <img src="https://cdn-icons-png.flaticon.com/512/616/616489.png" width="16" height="16" />
Sets how many players are needed to start the game. 

Example:
```go
//Sets the minimum needed requirement for the game to start. Set by default.
minplayerstostart 0
//Sets for recommended amount for public servers.
minplayerstostart 4
```

-----
## **MaxPlayers** <img src="https://cdn-icons-png.flaticon.com/512/616/616489.png" width="16" height="16" />
Sets how many players can be on the server at one time. 

**_NOTE: The more players there are on the server at once, the more CPU the server consumes._**

Example:
```go
//Sets manximum amount of players that can be online at once. Set by default.
maxplayers 16
//Set for recommended amount for public servers.
maxplayers 32
//Sets manximum amount of players that can be online at once.
maxplayers 64
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
# <img src="https://cdn-icons-png.flaticon.com/512/4789/4789514.png" width="32" height="32" /> **Advanced**

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
timeout 30000 //30000 (milliseconds) <-> 30 (seconds)
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
## **ResetTimerAfterConnect**
Enable/Disable the reset timer in the lobby countdown if someone joins the server.

Example:
```go
//Enables reset timer. Set by default.
resettimerafterconnect true
//Disables reset timer.
resettimerafterconnect false
```

-----
## **RoundsLimitPerStart**
Sets the number of rounds before the server application restarts.

Example:
```go
//Server application restarts after 2 rounds of gameplay. Set by default.
roundslimitperstart 2
```

-----
## **MapSize**
Changes the size of the map generation.

Example:
```go
//Recommended for smaller and quicker gameplay. Set by default.
mapsize 2
//Increases the size of of the map generation.
mapsize 4
```

-----
## **GameState**
Changes the game state of the server.

Example:
```go
//By default, there is no state set.
gamestate
//Sets the game state to "LOBBY".
gamestate Lobby
//Sets the game state to "STARTED".
gamestate Started
```

-----
## **DisableAuthKey**
Enable/Disable all incoming authorization keys on connection.

Example:
```go
//Enables all incoming authorization keys. Set by default.
disableauthkey false
//Disables all incoming authorization keys.
disableauthkey true
```

-----
## **DisableTimestamp**
Enable/Disable timestamps for the server logs.

Example:
```go
//Enables server timestamps. Set by default.
disabletimestamp false
//Disables server timestamps.
disabletimestamp true
```

-----
## **NoClipAntiCheat**
Enable/Disable anti-cheat for no clipping on the server.

Example:
```go
//Enables anti-cheat for no clipping. Set by default.
noclipanticheat true
//Disables anti-cheat for no clipping.
noclipanticheat false
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
## **FullSynchronization**
Enable/Disable synchronization for to match all server-side actions made from the connected clients.

Example:
```go
//Enables synchronization to match all server-side actions. Set by default.
fullsynchronization true
//Disables synchronization to match all server-side actions.
fullsynchronization false
```

-----
## **MenuHTML**
Sets the server HTML website when joining the server.

Example:
```go
//By default, there is no website url set.
menuhtml
//Set the link of the url.
menuhtml https://google.com/
```

-----
## **RestartMenuHTML**
Sets the server HTML website when the round is restarting on the server.

Example:
```go
//By default, there is no website url set.
restartmenuhtml
//Set the link of the url.
restartmenuhtml https://google.com/
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
# <img src="https://cdn-icons-png.flaticon.com/512/2195/2195441.png" width="32" height="32" /> **Expert**
This options are optional, and shouldn't be change unless needed.

-----
## **TickRate**
Changes the tick speed of the server. Performance will vary.

Example:
```go
//Set by default.
tickrate 128
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
## **StackSize**
Sets the stack size in server.

Example:
```go
//Set by default.
stacksize 512
```

-----
## **VoiceQuality**
Sets the voice quality for the server.

**_NOTE: This feature has been locked and fixed to output the maximum quality._**

Example:
```go
//Set by default.
voice_quality 48000
```

-----
## **LogsOff**
Enable/Disable log saves for the server.

Example:
```go
//Enables log saving. Set by default.
logsoff false
//Disables log saving.
logsoff true
```

-----
## **LongCulling**
Disable culling system, NOT RECOMMENDED.

Example:
```go
//Set by default.
longculling 0
```

-----
## **EventProb**
Sets the event probability, has no known use.

Example:
```go
//Set by default.
eventprob
```

-----
## **CentralServer**
Enable/Disable CentralServer or use SteamGameServer (needs Steam to use SteamGameServer) as an alternative, has no known use.

Example:
```go
//Enables between the CentralServer and dedicated server. Set by default.
centralserver true
//Disables between the CentralServer and dedicated server and uses SteamGameServer instead.
centralserver false
```

-----
## **CentralServerTCPRequest**
Sets central server incoming connection request to either TCP or UDP, has no known use.

Example:
```go
//Sets server to use TCP connections. Set by default.
centralservertcprequest tcp
//Sets server to use UDP connections.
centralservertcprequest udp
```

-----
## **SpeedHackRate**
Sets speedhack rates, has no known use.

Example:
```go
//Set by default.
speedhack_rate 100000.0  //Setting to 100000.0 will disable speedhack anticheat.
```

-----
# <img src="https://cdn-icons-png.flaticon.com/512/1100/1100349.png" width="32" height="32" /> **Breach Mode**

The configuration settings listed below are for `Breach Mode` only. 

This configuration requires [Breach](#breach-) to be `true`. Please ensure this is enabled for these settings to take effect.
{: .fs-4 .fw-300 .text-green-100 }

-----
## **BreachLight**
Enable/Disable brighter in Breach Mode within the facility.

Example:
```go
//Disables brighter light in Breach Mode. Set by default.
breachlight false
//Enables brighter light in Breach Mode.
breachlight true
```

-----
## **BreachChat** <img src="https://cdn-icons-png.flaticon.com/512/616/616489.png" width="16" height="16" />
Enable/Disable chatting in Breach Mode.

Example:
```go
//Disables chatting feature in Breach Mode. Set by default.
breachchat false
//Enables chatting feature in Breach Mode.
breachchat true
```

-----
## **BreachTime** <img src="https://cdn-icons-png.flaticon.com/512/616/616489.png" width="16" height="16" />
Sets the max time limit of Breach Mode per round.

Example:
```go
//Set by default.
breachtime 600000 // 600000 (milliseconds) <-> 600 (seconds) or 10 (minutes)
```

-----
## **BreachOnlyDeathmatch**
Enable/Disable the Breach Mode to deathmatch only.

Example:
```go
//Disable Deathmatch-only mode. Set by default.
breach_onlydeathmatch false
//Enables Deathmatch-only mode.
breach_onlydeathmatch true
```