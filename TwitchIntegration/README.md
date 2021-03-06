# HunterPie - Twitch Integration

This plugin will create a Twitch bot client, adding Monster Hunter: World related commands to your Twitch chat.

**ATTENTION: THIS PLUGIN REQUIRES HUNTERPIE v1.0.3.97 OR GREATER.**

## Installation

1. Download the zipped plugin [here](https://cdn.discordapp.com/attachments/402557384209203200/758353714305171486/TwitchIntegration.zip);
2. Extract it's contents to `HunterPie/Modules`;
3. Edit the `HunterPie/Modules/TwitchIntegration/config.json` and set your bot information and channel name correctly. Read [Setting up your bot](#Setting-up-your-bot) if you need help.
4. Run HunterPie.

### Setting up your bot

This plugin has a `config.json` file to set your Bot information in order for it to connect to Twitch. Open it with a text editor and set the follow information accordingly:

```js
{
  "Username": "MyBotName",                  // This is your Bot username
  "OAuth": "oauth:myBotOauthToken1234",     // This is your bot OAuth token prefixed by oauth:, you can get one here: https://twitchapps.com/tmi/
  "Channel":  "Haato__"                     // This is your channel name
}
```

## Supported Commands

Here's a list of the current supported commands for this bot:

> **Note:** Commands are **case-insensitive**.

Command name | Description | Bot response
:-----------:|:--------------------------------------------------|:---------
!id,!session          | Sends your current session ID to your Twitch chat. | `Session Id: 1@a2SdxK63aW`
!build       | Sends your current build to your Twitch chat, the link is to Honey Hunters World, but it's shortened using Tinyurl. | `My current Bow build: https://tinyurl.com/y6av65mw`
!rank        | Sends your current character basic information to your Twitch chat. | `Lyss \| HR: 308 \| MR: 129 \| Playtime: 43.05:25:30`

## For more custom commands

HunterPie plugins have access to every information HunterPie tracks, see the [Plugin documentation here](https://docs.hunterpie.me/?p=Plugins/plugins.md), if you want to add more commands, you can find the source code for this plugin [here](https://github.com/Haato3o/HunterPie.Plugins/blob/master/TwitchIntegration/main.cs).

> **NOTE:** Don't forget to rename the `main.cs` to anything else after you've compiled it, otherwise HunterPie will compile it over and over every time you start it again.