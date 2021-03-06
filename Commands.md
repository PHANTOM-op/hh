This is a summary of all of Vortex's commands. Arguments surrounded by `<>` are required, and arguments surrounded by `[]` are optional. Do not include `<>` nor `[]` when running commands!


## 📜 General Commands
### `>>about`
Shows information about the bot, including its version number, some features, and a few statistics.

### `>>invite`
Provides Vortex's invite link. If you are having trouble inviting Vortex, make sure you are correctly logged in at https://discordapp.com/login

### `>>ping`
Checks Vortex's latency. 

### `>>roleinfo <role>`
Shows information about a role.

### `>>serverinfo`
Shows information about the server this command is used in. 

### `>>userinfo [user]`
Shows information about the provided user, or yourself if you don't include any arguments.


## 📜 Moderation Commands
These commands can be run if a user's native Discord permissions would allow using the command, or if they have the designated mod role (see the Settings commands below).

### `>>kick <@users or user IDs...> [reason]`
Kicks all of the provided users (or user IDs). If a reason is included, that reason is used in the audit log and moderation log.

### `>>ban <@users or user IDs...> [time] [reason]`
Bans all of the provided users (or user IDs). If a length of time is included, the users will be unbanned after the provided time. If a reason is included, that reason is used in the audit log and moderation log.

### `>>softban <@users or user IDs...> [reason]`
Bans and then immediately unbans all the provided users. This is useful to simultaneously kick a user and clean all of their recent messages. If a reason is included, that reason is used in the audit log and moderation log.

### `>>silentban <@users or user IDs...> [time] [reason]`
Identical to `>>ban`, but no messages will be deleted

### `>>unban <@users or user IDs...> [reason]`
Unbans users.

### `>>clean <parameters>`
Cleans all messages in the current channel matching the given parameters. See [[Cleaning Messages]] for more detailed information about this command.

### `>>voicekick <@users or user IDs...>`
Creates a temporary voice channel, moves the provided users into it, and then deletes the channel, effectively kicking them from voice.

### `>>voicemove [channel]`
Puts Vortex into the specified voice channel (or your current channel if no arguments are provided) and waits. When you drag Vortex to a new channel, he will drag all users in the current channel to the new channel.

### `>>mute <@users or user IDs...> [time] [reason]`
Gives the 'Muted' role to all of the provided users. If a length of time is included, the users will be unmuted after the provided time. If a reason is included, that reason is used in the audit log and moderation log. 

### `>>unmute <@users or user IDs...> [reason]`
Removes the 'Muted' role from all of the provided users. If a reason is included, that reason is used in the audit log and moderation log. 

### `>>raidmode [ON | OFF] [reason]`
Enables or disables Anti-Raid Mode. If no arguments are included, it will show if Anti-Raid Mode is currently active. During Anti-Raid Mode, the server's verification will be increased (no higher than Tableflip) and all users that attempt to join the server will be informed that the server is under lockdown and then kicked. See [[Anti-Raid Mode]] for more information.

### `>>strike [number] <@users or user IDs...> <reason>`
Gives the specified number of strikes (or 1 if not specified) to the provided users. Each user will receive a private message warning them about the accumulated strikes and reason. 

### `>>pardon [number] <@users or user IDs...> <reason>`
Removes the specified number of strikes (or 1 if not specified) to the provided users. Each user will receive a private message letting them know of the pardon and reason.

### `>>check <user>`
Checks how many strikes a user has, as well as their current mute and/or ban status, if available.

### `>>reason [case number] <reason>`
Edits a reason in the Moderation Log. If no case number is provided, Vortex will search the log for the most-recent case that has no provided reason.


## 📜 Settings Commands
These commands control various Vortex settings. The Manage Server permission is needed to use these commands.

### `>>setup`
Performs server setup. See [[Getting Started]] for more information.

### `>>punishment <number> <action> [time]`
Sets the punishment to be given when a certain number of strikes is reached. Valid actions are **None**, **Mute**, **Kick**, **Softban**, and **Ban**. Mute and Ban can also have time values associated with them. See [[Strikes]] for more information.

### `>>messagelog <#channel or OFF>`
Sets the channel to which message edits and deletes will be logged.

### `>>modlog <#channel or OFF>`
Sets the channel to which moderation actions will be logged.

### `>>serverlog <#channel or OFF>`
Sets the channel to which server activity (joins, leaves, name changes) will be logged.

### `>>voicelog <#channel or OFF>`
Sets the channel to which voice joins, leaves and changes will be logged.

### `>>avatarlog <#channel or OFF>`
Sets the channel to which avatar changes of members are logged. This feature is only available with [[Vortex Pro]].

### `>>timezone <zone>`
Sets the timezone for the serverlog, messagelog, and modlog timestamps. See [[Log Timezone]] for more information.

### `>>modrole <role>`
Sets the moderation role for the server. Any user with this role can perform [[moderation commands|Commands#-moderation-commands]], even if they do not normally have the necessary permissions.

### `>>prefix <prefix or NONE>`
Sets a custom prefix for the server. The default prefix (`>>`) will still work and cannot be removed.

### `>>settings`
Shows the server's current settings.


## 📜 Automod Commands
Please see the [[Auto Moderation]] page for more in-depth descriptions of these features. All of these commands require the Manage Server permission to use.

### `>>antiinvite <strikes>`
Sets the number of strikes a user receives when they post a Discord invite link

### `>>anticopypasta <strikes>`
Sets the number of strikes a user receives when they post a copypasta

### `>>antieveryone <strikes>`
Sets the number of strikes a user receives when attempting to ping everyone/here

### `>>antireferral <strikes>`
Sets the number of strikes a user received for posting referral links and other malicious links.

### `>>maxmentions <number | OFF>`
Sets the maximum unique, non-bot mentions a user can send in a single message. Any message containing more than the maximum will be deleted, and users will receive one strike for every additional mention.

### `>>maxlines <number | OFF>`
Sets the maximum number of lines a message can be. Any message containing more than the maximum will be deleted, and users will receive one strike for every additional line.

### `>>maxmentions role <number | OFF>`
Sets the maximum unique, mentionable role mentions a user can send in a single message. Any message containing more than the maximum will be deleted, and users will receive one strike for every additional mention.

### `>>antiduplicate <strike threshold> [delete threshold] [strikes]`
Sets the values to control and punish duplicate messages. `<strike threshold>` determines when duplicate messages will start accumulating strikes. Once the strike threshold is met, users will receive `[strikes]` strikes (default 1) for each additional duplicate sent. Any duplicate exceeding the `[delete threshold]` will be deleted.

### `>>autodehoist <character | OFF>`
Sets the character such that users setting their nickname (or username if they have no nickname) will be 'dehoisted,' or moved lower in the member list. This is useful for preventing people from using certain nicknames to put themselves higher in the member list.

### `>>resolvelinks <ON | OFF>`
Enables or disables resolving links (redirect links) for invite and referral links. This feature is only available with [[Vortex Pro]].

### `>>autoraidmode <ON | OFF | joins/seconds>`
Configures Vortex to automatically enable Anti-Raid Mode when it senses a raid. Setting `joins/seconds` will enable Anti-Raid Mode if there are at least `joins` new joins to the server within `seconds` seconds. Setting this to `ON` uses 10 joins in 10 seconds.

### `>>ignore <role | channel>`
Sets the Auto-Moderator to ignore all users with a specific role, or all messages in a specific channel. Run this command without arguments to show the current ignore list. See [[Ignoring Roles and Channels]] for more info.

### `>>unignore <role | channel>`
Removes a role or channel from the ignore list. See [[Ignoring Roles and Channels]] for more info.


## 📜 Tools Commands
These commands provide other useful tools for moderation and server management.

### `>>announce <#channel> <rolename> | <message>`
Pings a role with an announcement in the specified channel. If the role is not mentionable, it will make it mentionable in order to send the message, and then make it unmentionable again.<br>
Examples:
```
>>announce #updates UpdateRoleName | Hey guys this is an update
>>announce update_channel_name Role Name | This is an announcement!
>>announce #announcements Members | Hey members, check this out!!
```

### `>>audit <ALL | FROM | ACTION> [user or action]`
Finds recent audit log entries (all entries, entries from a certain user, or entries of a specific action type) and displays them in a mobile-friendly format.

### `>>dehoist [symbol]`
Modifies the nickname of any user using a symbol (such as `!`) to put their name at the top of the member list. By default, this will dehoist any member with names starting with `!`.

### `>>inviteprune [max uses]`
Deletes any invites with uses less than or equal to the provided number. By default, this will prune invites with 0 or 1 uses.

### `>>lookup <ID | invite>`
Finds information about a user or guild via ID (for either) or an invite code (for guilds only). All information found in this way is information that Discord makes publicly-available, and is not impacted by Vortex being in the guilds nor having mutual servers with the user.