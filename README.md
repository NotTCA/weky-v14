<p align="center"><img width="100px"
   style="margin-bottom:-6px" src="https://cdn.discordapp.com/avatars/809496186905165834/7dbf02cb782c7111b817f329cac0257a.png" /></p>
<h1 align="center">Weky</h1>
<p align="center">
   <a href="https://www.npmjs.com/package/@nottca/weky"><img src="https://img.shields.io/npm/v/@nottca/weky.svg?style=flat-square" /></a>
   <a href="https://weky-docs.js.org/"><img src="https://img.shields.io/badge/Documentation-Yes-amiajokegreen.svg?style=flat-square" /></a>
   <a href="https://github.com/@nottca/weky/blob/main/LICENSE"><img src="https://nuggies.js.org/assets/img/license.ade17f5e.svg" /></a>
   <br>
   <a href="https://www.npmjs.com/package/@nottca/weky"><img src="https://nodei.co/npm/@nottca/weky.png?downloadRank=true&downloads=true&downloadRank=true&stars=true" /></a>
</p>

## What is weky?

- A fun npm package to play games within Discord with buttons!
- Looking for examples? [Click here!](https://github.com/NotTCA/weky-v14/tree/main/Examples)

## Features

- 🧑 Beginner friendly
- 🎉 Easy to use
- ✨ Simple
- 🔘 Discord Buttons
- 🤖 Supports Discord.js v12, v13, and v14!
- and much more!

## Install the package 📥

```sh
npm install @nottca/weky
```

## Usage 📚

```js
const { Calculator } = require("@nottca/weky");
await Calculator({
  message: message,
  embed: {
    title: "Calculator | Weky Development",
    color: "#5865F2",
    footer: "©️ Weky Development",
    timestamp: true,
  },
  disabledQuery: "Calculator is disabled!",
  invalidQuery: "The provided equation is invalid!",
  othersMessage: "Only <@{{author}}> can use the buttons!",
});
```

## Example ✏️

#### Discord.js v12

```js
const Discord = require("discord.js");
require("@weky/inlinereply");
const client = new Discord.Client();
const disbut = require("discord-buttons");
const { Calculator } = require("@nottca/weky");
disbut(client);

client.on("ready", async () => {
  console.log(`Logged in as ${client.user.tag}`);
});

client.on("message", async (message) => {
  if (message.content === "!calculator") {
    await Calculator({
      message: message,
      embed: {
        title: "Calculator | Weky Development",
        color: "#5865F2",
        footer: "©️ Weky Development",
        timestamp: true,
      },
      disabledQuery: "Calculator is disabled!",
      invalidQuery: "The provided equation is invalid!",
      othersMessage: "Only <@{{author}}> can use the buttons!",
    });
  }
});

client.login("DISCORD_BOT_TOKEN");
```

#### Discord.js v13

```js
const Discord = require("discord.js");
const client = new Discord.Client({
  intents: ["GUILDS", "GUILD_MESSAGES"],
});
const { Calculator } = require("@nottca/weky");

client.on("ready", async () => {
  console.log(`Logged in as ${client.user.tag}`);
});

client.on("messageCreate", async (message) => {
  if (message.content === "!calculator") {
    await Calculator({
      message: message,
      embed: {
        title: "Calculator | Weky Development",
        color: "#5865F2",
        footer: "©️ Weky Development",
        timestamp: true,
      },
      disabledQuery: "Calculator is disabled!",
      invalidQuery: "The provided equation is invalid!",
      othersMessage: "Only <@{{author}}> can use the buttons!",
    });
  }
});

client.login("DISCORD_BOT_TOKEN");
```

#### Discord.js v14

```js
const Discord = require("discord.js");
const client = new Discord.Client({
  intents: ["Guilds", "GuildMessages", "MessageContent"],
});
const { Calculator } = require("@nottca/weky");

client.on("ready", async () => {
  console.log(`Logged in as ${client.user.tag}`);
});

client.on("messageCreate", async (message) => {
  if (message.content === "!calculator") {
    await Calculator({
      message: message,
      embed: {
        title: "Calculator | Weky Development",
        color: "#5865F2",
        footer: "©️ Weky Development",
        timestamp: true,
      },
      disabledQuery: "Calculator is disabled!",
      invalidQuery: "The provided equation is invalid!",
      othersMessage: "Only <@{{author}}> can use the buttons!",
    });
  }
});

client.login("DISCORD_BOT_TOKEN");
```

## Result 📤

<img src="https://i.imgur.com/DEdhHHd.png">

## Contributing 🤝

- Contributions, issues and feature requests are welcome!
- Feel free to check **[issues page](https://github.com/NotTCA/weky-v14/issues)**.

## Developers 👨‍💻

- **[Face#5454](https://github.com/face-hh)**
- **[Sujal Goel#7602](https://github.com/sujalgoel)**
- **[rayz#4986](https://github.com/rayzdev)**
- **[TCA#7797](https://github.com/NotTCA)**

## Support ❔

<a href="https://discord.gg/ANzBrkcXZy"><img src="https://invidget.switchblade.xyz/ANzBrkcXZy" /></a>
