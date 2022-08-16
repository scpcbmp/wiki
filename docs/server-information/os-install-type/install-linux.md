---
layout: default
title: Linux Installation
parent: Server Installation
grand_parent: Server Information
nav_order: 2
---

# **Server Installation for Linux**
{: .fs-9 .fw-600 }
----

## Installation via SteamCMD with video card
---
1. Install Wine through the official website.
2. Log in anonymously on SteamCMD: `login anonymous`
3. Download the server using: `app_update 1801280`
4. Close SteamCMD: `quit`
5. Open the folder containing the dedicated server.
6. Set up the changes you want made to your `server.cfg` 
7. Run your server by clicking on the app titled: `server.exe`.

---
## Installing via SteamCMD without a video card
---
1. Install `Wine` through the official website .
2. Install `XVFB` using the install command through the terminal: `sudo apt install xvfb`.
3. Log in anonymously on SteamCMD with this CLI input: `login anonymous`
4. Download the server using: `app_update 1801280`
5. Close SteamCMD: `quit`
6. Open the folder containing the dedicated server.
6. Set up the changes you want made to your `server.cfg` 
8. Run it: `xvfb-run -a wine server.exe`