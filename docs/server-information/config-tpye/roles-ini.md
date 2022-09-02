---
layout: default
title: Roles Initialization File
parent: Server Configurations
grand_parent: Server Information
nav_order: 3
---

# **Roles Initialization File**
{: .fs-9 .fw-600 }
-----

The `roles.ini` is a initialization file which can be modified to optimize a character prefernces. It is one of the core files to have and is required to run the server. This file is located in the **ServerConfig** folder.

**_NOTE: Some configurations such as "HEALTH" and "SPEEDMULT" will only work if `fullsynchronization 1` is set in `server.cfg`._**

-----
# <img src="https://cdn-icons-png.flaticon.com/512/5009/5009866.png" width="32" height="32" /> **Key Functions**

This is a placeholder message to see how long this can present until we hit a limit to start break dancing all on the ground, YAAAYYYYYYYY!!!

-----
# <img src="https://cdn-icons-png.flaticon.com/512/2807/2807191.png" width="32" height="32" /> **Character Classes**

Listed below are the available classes that can be modified.

-----
## **MTF:**
Loadout class for MTF.

```cs
//Set by default.
[mtf]
health = 150
speedmult = 1.0
item1 = M4A4/m4a4,if random SPAS-12/spas12
item2 = Desert Eagle/deagle
item3 = Key Card Omni/key6
item4 = Radio Transceiver/radio
item5 = Grenade/grenade
item6 = Small First Aid Kit/finefirstaid
item7 = Night Vision Goggles/supernv,if scp-966 exists
item8 = Box of ammo/boxofammo
item9 = Handcuffs/handcuffs
item10 = null
```

-----
## **Guard:**
Loadout class for Guard.

```cs
//Set by default.
[guard]
health = 120
speedmult = 1.0
item1 = FN P90/p90,if random MP5-SD/mp5sd
item2 = USP Tactical/usp
item3 = Level 5 Key Card/key5
item4 = Radio Transceiver/radio
item5 = Grenade/grenade
item6 = Small First Aid Kit/finefirstaid
item7 = null
item8 = null
item9 = null
item10 = null
```

-----
## **Class-D:**
Loadout class for Class-D.

```cs
//Set by default.
[class d]
health = 100
speedmult = 1.0
item1 = null
item2 = null
item3 = null
item4 = null
item5 = null
item6 = null
item7 = null
item8 = null
item9 = null
item10 = null
```

-----
## **Scientist:**
Loadout class for Scientist.

```cs
//Set by default.
[scientist]
health = 100
speedmult = 1.0
item1 = Level 2 Key Card/key2
item2 = null
item3 = null
item4 = null
item5 = null
item6 = null
item7 = null
item8 = null
item9 = null
item10 = null
```

-----
## **SCP-173:**
Loadout class for SCP-173.

```cs
//Set by default.
[scp-173]
health = 5000
speedmult = 1.0
item1 = Level 5 Key Card/key5
item2 = null
item3 = null
item4 = null
item5 = null
item6 = null
item7 = null
item8 = null
item9 = null
item10 = null
```

-----
## **SCP-049:**
Loadout class for SCP-049.

```cs
//Set by default.
[scp-049]
health = 5000
speedmult = 1.0
item1 = Level 5 Key Card/key5
item2 = null
item3 = null
item4 = null
item5 = null
item6 = null
item7 = null
item8 = null
item9 = null
item10 = null
```

-----
## **Chaos (Insurgency) Soldier:**
Loadout class for Chaos (Insurgency) Soldier.

```cs
//Set by default.
[chaos soldier]
health = 150
speedmult = 1.0
item1 = M4A4/m4a4,if random SPAS-12/spas12
item2 = Desert Eagle/deagle
item3 = Key Card Omni/key6
item4 = Radio Transceiver/radio
item5 = Grenade/grenade
item6 = Small First Aid Kit/finefirstaid
item7 = Night Vision Goggles/supernv,if scp-966 exists
item8 = Box of ammo/boxofammo
item9 = Handcuffs/handcuffs
item10 = null
```

-----
## **Janitor:**
Loadout class for Janitor.

```cs
//Set by default.
[janitor]
health = 100
speedmult = 1.0
item1 = Level 1 Key Card/key1
item2 = null
item3 = null
item4 = null
item5 = null
item6 = null
item7 = null
item8 = null
item9 = null
item10 = null
```

-----
## **SCP-939:**
Loadout class for SCP-939.

```cs
//Set by default.
[scp-939]
health = 2000
speedmult = 1.0
item1 = Level 5 Key Card/key5
item2 = null
item3 = null
item4 = null
item5 = null
item6 = null
item7 = null
item8 = null
item9 = null
item10 = null
```

-----
## **SCP-106:**
Loadout class for SCP-106.

```cs
//Set by default.
[scp-106]
health = 5000
speedmult = 1.0
item1 = null
item2 = null
item3 = null
item4 = null
item5 = null
item6 = null
item7 = null
item8 = null
item9 = null
item10 = null
```

-----
## **SCP-966:**
Loadout class for SCP-966.

```cs
//Set by default.
[scp-966]
health = 3000
speedmult = 1.0
item1 = Level 5 Key Card/key5
item2 = null
item3 = null
item4 = null
item5 = null
item6 = null
item7 = null
item8 = null
item9 = null
item10 = null
```

-----
## **SCP-049-2:**
Loadout class for SCP-049-2.

```cs
//Set by default.
[scp-049-2]
health = 300
speedmult = 1.0
item1 = Level 5 Key Card/key5
item2 = null
item3 = null
item4 = null
item5 = null
item6 = null
item7 = null
item8 = null
item9 = null
item10 = null
```

-----
## **SCP-096:**
Loadout class for SCP-096.

```cs
//Set by default.
[scp-096]
health = 3000
speedmult = 1.0
item1 = Level 5 Key Card/key5
item2 = null
item3 = null
item4 = null
item5 = null
item6 = null
item7 = null
item8 = null
item9 = null
item10 = null
```