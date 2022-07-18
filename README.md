# @leomotors/music-bot

[![](https://img.shields.io/npm/v/@leomotors/music-bot.svg?maxAge=3600)](https://www.npmjs.com/package/@leomotors/music-bot)
[![](https://img.shields.io/npm/dt/@leomotors/music-bot.svg?maxAge=3600)](https://www.npmjs.com/package/@leomotors/music-bot)
[![](https://github.com/Leomotors/music-bot/actions/workflows/test.yml/badge.svg)](https://github.com/Leomotors/music-bot/actions)

Music Bot components extracted from [harunon.js](https://github.com/CarelessDev/harunon.js)

## How to use

This package has 2 parts, the underlying mechanics and the part that consume it.

You likely only want to import complete Music Cog which is compatible to [cocoa-discord-utils](https://github.com/Leomotors/cocoa-discord-utils)

See Example at [tests/bot.js](./tests/bot.js)

Apart from that, if you can understand the code [src/voice.ts](src/voice.ts),
you can directly interact with api underneath, all of them is public.

### Installation

You don't need to install `cocoa-discord-utils` but use one that is shipped with this package, to avoid conflict

### Minimal Usage

- Clone this repository, build the package and run tests/bot.js

- Adjust and add some codes to personalize the bot

### Advanced Usage

- Import music module to existing bot that use [Cocoa Discord Utils](https://github.com/Leomotors/cocoa-discord-utils)
(See [harunon.js](https://github.com/CarelessDev/harunon.js) for example)

## Prerequisites

- node 16 (Minimum required by discord.js, What my bots are optimized for)

- **IMPORTANT** [Encoding Libraries](https://www.npmjs.com/package/@discordjs/voice#dependencies)
(This library does not ship these encoding libraries, so you can freely decide which one to install)

## ✨Features

- play from YouTube

- queue

- pause / resume

- Loop

- Remove from Queue and Clear

- Search with beautiful embeds

## 🖼️ Highlight

- ✨ Search Feature

![](./images/search1.png)

![](./images/search2.png)

*Note: It is known issues that search feature summon duplicate embed, I blame discord.js for this bug*

## Note

- This module has its cog named "Music", be sure to not creating a duplicate name

- Despite cocoa-discord-utils supports CommonJS, this module does not

- This module is still in beta, not implemented features includes but not limited to: Working in edge cases for example, user invoke command without being in voice channel
