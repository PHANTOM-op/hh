## 🌀 Read This First
Unless you already know how to use Vortex, then **Vortex is likely not the bot for you**. It takes some effort to learn to use Vortex efficiently, and very little support will be provided beyond the documentation in this wiki. If you've never used Vortex, consider searching for a different moderation bot on https://discord.bots.gg

## 🌀 Requirements
There are some light requirements to using Vortex. These requirements are in place to help save resources. Your server must meet all of the requirements below, or Vortex will automatically leave your server.
* **30 or more human members** - Vortex is a moderation bot, and if you have fewer than 30 people, why do you need a bot to moderate anything?
* **More humans than bots** - Adding a lot of bots to a server just wastes resources, and making 'bot collection' servers is generally frowned upon. No server should need more bots than humans.
* **Strong knowledge of Discord and Discord bots, and the ability to read documentation** - Vortex is easy-to-use for admins and moderators, but only if they are willing to put in the time to read the documentation (this wiki). In general, asking for support for a question answered here will result in being redirected back to this wiki.
* **Follow Discord's Terms of Service** - While not automatically detected, if a server is reported for ToS violations, Vortex may be manually removed.
> ⚠ **Please read these requirements; Vortex may automatically leave your server if it does not meet them!**

## 🌀 Adding Vortex to Your Server
The first step is to make sure that Vortex is actually on your server! To add a bot to your server, you must have the **Manage Server** permission on the server. If you do, you can click this link to add Vortex to your server:

> ⚠ **Please read the requirements above this section; Vortex may automatically leave your server if it does not meet the requirements**

**https://discordapp.com/oauth2/authorize?client_id=240254129333731328&permissions=500559086&scope=bot**

If your server isn't listed, make sure you are correctly logged in by visiting https://discordapp.com/login

## 🌀 Check Vortex's Permissions
To operate correctly, Vortex needs the permissions to be able to complete necessary tasks. The easiest way to achieve this is to give the 'Vortex' role the Administrator permission and drag it to the top (or near the top) of the role list.

> ![RoleOrder](https://i.imgur.com/kJMIG8o.gif)

## 🌀 Settings

The next step is configuring vortex for your server! You can type `>>help settings` to see a full list of settings commands, `>>help automod` to see a full list of automod commands, or check out the [[Full Command Reference|Commands]]

### Muted Role
The Muted role is a role that (usually) can be applied to a user to prevent them from sending messages, adding reactions, speaking, and connecting to voice channels. To create a Muted role with this default functionality, run `>>setup muted`. You can also customize the permissions after creation to your liking (such as also causing it to remove Read Messages perms in some channels, or allowing sending messages in a "time-out" channel). 

### Logs
Vortex has various logs to keep track of different kinds of server activity. All commands for logs are found in the Settings commands, available via `>>help settings` or on the [[Full Command Reference|Commands]]. If your server is utilizing the [[strike system|Strikes]], it is recommended to enable (at minimum) the ModLog.

### Moderator Role
The Moderator Role is a role that allows a user with said role to use all Moderation commands. The full list of Moderation commands is available via `>>help mod` as well as on the [[Full Command Reference|Commands]]. To set a role to be the Moderator role, use `>>modrole <rolename>` (for example, if your moderator role is called "Staff", you'd run `>>modrole Staff`). To disable the Moderator role, run `>>modrole none`. 

If no Moderator role is set, Moderation commands can only be run if the user has sufficient permissions natively (they would only be able to ban someone with Vortex if and only if they could ban them via the Discord client as well).

Also, make sure to check out the [[Moderator Guide]] for helpful tips for moderating with Vortex!

### AutoMod
For full information about the AutoMod and its features, check out the [[Auto-Moderation]] page. You can set the default automod settings using `>>setup automod`.