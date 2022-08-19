---
layout: default
title: Script Creation
parent: Scripting Language
has_children: false
nav_order: 1
---

# **Script Creation**
{: .fs-9 .fw-600 }

Dedicated server package comes with script examples, and script compiling software. Almost every aspect of the server can be modified. You can also add new content to the server. However we can't guaranty stable server using scripts.

## **Create your own script**
Scripts use the custom programing language, called Skynet++. Skynet++ is based on Lua.

## Getting Started
First you will have to download server package in order to have examples and compiling software.

You can download server package on steam.

## Examples
You should be able to see the example script in scripts folder. It's called `example.gs`, and `playerscript.lua`.

Example scripts do nothing, but they can help you understand the language structure.

## Building the Script
Create your own script file, you can name it whatever you want.

First you will have to include variables from the multiplayer mod:

```cs
#include "includes\multiplayer_core.inc"
```

You can see all functions in here.
Once you made everything you need, you have to compile the script.
Open the compiler, don't mind the errors appeared, enter:

```cs
compile {scriptname}
```

Once you compiled the script, you can enable it in server config, using this setting:

```cs
script {FILENAME}
```

Don't forget that you have to put script file in the server folder(not scripts).