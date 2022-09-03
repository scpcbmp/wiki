---
layout: default
title: Server Callback API
parent: Server Functions
grand_parent: Scripting Language
nav_order: 1
---
# **Server Callback API**
{: .fs-9 .fw-600 }
A complete list of callbacks that can used when scripting for your server.

-----
## Server Callback Function:
{: .fs-4 .fw-600 }
Callbacks that only focus solely on the non-gameplay interactions between the client and server.

| Server Callback Functions | Description |
|:-------------|:------------------|
| [OnBadIncomingConnection](OnBadIncomingConnection) | Called when the Steam Authentication ticket recieved from the Central Server is bad. Client is rejected to join to server should this happen. |
| [OnConnectionResponse](OnConnectionResponse) | Executed when client establishes a brief connection to the server. |
| [OnIncomingConnection](OnIncomingConnection) | This callback acts as the first repsonse for when the player decides to join the server, even before steam authentication with the central servers happens. Executed when client sends the join request for the server. |
| [OnLostConnectionWithCentralServer](OnLostConnectionWithCentralServer) | Executes when server loses connection to a central server (Steam Authentication server).|
| [OnMapUpdate](OnMapUpdate) | Called on every map update (npcs, doors, events, players, etc...) |
| [OnScriptLoaded](OnScriptLoaded) | Executes when a script send loads. Executed after the "[...] loaded successfully" message has outputed to server console. |
| [OnCheatDetected](OnCheatDetected) | Called when server detects possible cheat by client/player. |
| [OnServerStart](OnServerStart) | Executes once when the server begins initial start or when round reset limits have been reached, and a full application restart happens. |
| [OnServerUpdate](OnServerUpdate) | A callback that is updated executed on the server every tick. |
| [OnReceiveRawPacket](OnReceiveRawPacket) | When server recieves a packet response from the server. Banks via packets are dropped from memory after finishing execution. |
| [OnServerRestart](OnServerRestart) | Executed when a round restart finishes. Called after console outputs acknoledgement of round ending. |

| Player Callback Functions | Description |
|:-------------|:------------------|
| [OnPlayerConnect](OnPlayerConnect) | Called after client recieves sucessful authentication repsonse from the server and finally makes a full connection to the server. |
| [OnPlayerChat](OnPlayerChat) | Called every time a client sends a chat message to the server. |
| [OnPlayerConsole](OnPlayerConsole) | Called when a player sends a console commands to the server (F3 Console via Client).  |
| [OnPlayerDownloadFile](OnPlayerDownloadFile) | Called when the client is downloading a file. |
| [OnPlayerBotConnect](OnPlayerBotConnect) | Called when a FakePlayer "joins" the game. Used with `CreateFakePlayer` function.|
| [OnPlayerDisconnect](OnPlayerDisconnect) | Called when the client sends a disconnet request to the server. |
| [OnPlayerMouseHit](OnPlayerMouseHit) | Called when client sends in mouse information. |
| [OnPlayerRequestFiles](OnPlayerRequestFiles) | Called when a player requests the downloading of a file. |
| [OnPlayerUpdate](OnPlayerUpdate) | Called when a client sends back an update to the server. |
| [OnPlayerRconIncorrect](OnPlayerRconIncorrect) | Called when inputting in the RCON login information incorrectly. |
| [OnPlayerRconAuthorized](OnPlayerRconAuthorized) | Called when inputting in the RCON login correctly. |

## Game Callback Function:
{: .fs-4 .fw-600 }
Callbacks that only focus solely on the gameplay interactions between the client and server.

| Player Callback Functions | Description |
|:-------------|:------------------|
| [OnPlayerSpeaking](OnPlayerSpeaking) |  |
| [OnPlayerTriggered096](OnPlayerTriggered096) | |
| [OnPlayerShoot](OnPlayerShoot) | |
| [OnPlayerShootRocket](OnPlayerShootRocket) | |
| [OnPlayerRequestNewRole](OnPlayerRequestNewRole) | |
| [OnPlayerHitPlayer](OnPlayerHitPlayer) | |
| [OnPlayerKillPlayer](OnPlayerKillPlayer) | |
| [OnPlayerActivateFemurBreaker](OnPlayerActivateFemurBreaker) | |
| [OnPlayerRequestExplosion](OnPlayerRequestExplosion) | |
| [OnPlayAnnouncement](OnPlayAnnouncement) | |
| [OnPlayerRequestUnlockExits](OnPlayerRequestUnlockExits) | |
| [OnPlayerSpawnItem](OnPlayerSpawnItem) | |
| [OnPlayerTakeItem](OnPlayerTakeItem) | Called when player picks up an item. |
| [OnPlayerDropItem](OnPlayerDropItem) | Called when player drops an item. |
| [OnPlayerClickButton](OnPlayerClickButton) | Called when players interact with doors. |
| [OnPlayerRotateLever](OnPlayerRotateLever) | Called when a player rotates a lever. |
| [OnPlayerReleaseSound](OnPlayerReleaseSound) | Called when a player makes sounds of anykind that the client sends to the server to broadcast to other players. |
| [OnPlayerUseItem](OnPlayerUseItem) | Called when players use consumable or one-time items. |
| [OnPlayerUse1162](OnPlayerUse1162) | |
| [OnPlayerRequestNoTarget](OnPlayerRequestNoTarget) | |
| [OnPlayerCreateDecal](OnPlayerCreateDecal) | |
| [OnPlayerDropGrenade](OnPlayerDropGrenade) | Called when player throws an unspecified grenade. |
| [OnPlayerGetNewRole](OnPlayerGetNewRole) | Called when a player switches to a new playertype. |
| [OnPlayerEscape](OnPlayerEscape) | Called for when specific playertypes escape through correct escape exits. |
| [OnPlayerEscapeButDead](OnPlayerEscapeButDead) | Called for when specific playertypes escape through incorrect escape exits. |
| [OnPlayerCuffPlayer](OnPlayerCuffPlayer) | Called when players attempt to cuff other players. |
| [OnPlayerDeactivateWarheads](OnPlayerDeactivateWarheads) | Called when players deactivates Warheads. |
| [OnPlayerActivateWarheads](OnPlayerActivateWarheads) | Called when players activates Warheads.|
| [OnPlayerSCPContained](OnPlayerSCPContained) | Called when a player kills a player with an SCP playertype, or dies from enviromental effects. |

| Spawn Callback Functions | Description |
|:-------------|:------------------|
| [OnSpawnMTF](OnSpawnMTF) | Called for when spawnwave for MTF occurs. |
| [OnSpawnChaos](OnSpawnChaos) | Called for when spawnwave for Chaos occurs. |

| Warhead Callback Functions | Description |
|:-------------|:------------------|
| [OnActivateWarheads](OnActivateWarheads) | Called when Warheads just become active, either by players or events. |
| [OnDeactivateWarheads](OnDeactivateWarheads) | Called when Warheads just become deactivated, either by players or events. |
| [OnWarheadsExplosion](OnWarheadsExplosion) | Called when Warheads reach a specific time for it to explode.  |

| "Entity Generation" Callback Functions | Description |
|:-------------|:------------------|
| [OnCreateNPC](OnCreateNPC) | Called when a new NPC is spawned into the server. |
| [OnCreateItem](OnCreateItem) | Called when a new item is created. |
| [OnItemRefine](OnItemRefine) | Called when SCP-914 is triggered. Specifically called at the end of SCP-914 event state. |

| Server Only Callback Functions | Description |
|:-------------|:------------------|
| [OnGenerateWorld](OnGenerateWorld) | Called when world generation for the server occurs. |
| [OnRoundStarted](OnRoundStarted) | Called when server lobby time reaches 0 to begin the game. |
