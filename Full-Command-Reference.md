This is a summary of all of Vortex's commands. Arguments surrounded by `<>` are required, and arguments surrounded by `[]` are optional. Do not include `<>` nor `[]` when running commands!

## 📄 General Commands
### `>>about`
Shows information about the bot, including its version number, some features, and a few statistics.

### `>>invite`
Provides Vortex's invite link. If you are having trouble inviting Vortex, make sure you are correctly logged in at https://discordapp.com/login

### `>>ping`
Checks Vortex's latency. 

### `>>serverinfo`
Shows information about the server this command is used in. 

### `>>userinfo [user]`
Shows information about the provided user, or yourself if you don't include any arguments.

## 📄 Moderation Commands
### `>>kick <@users or user IDs...> [reason]`
Kicks all of the provided users (or user IDs). If a reason is included, that reason is used in the audit log and moderation log.

### `>>ban <@users or user IDs...> [time] [reason]`
Bans all of the provided users (or user IDs). If a length of time is included, the users will be unbanned after the provided time. If a reason is included, that reason is used in the audit log and moderation log.

### `>>softban <@users or user IDs...> [reason]`
Bans and then immediately unbans all the provided users. This is useful to simultaneously kick a user and clean all of their recent messages. If a reason is included, that reason is used in the audit log and moderation log.

### `>>clean <parameters>`
Cleans all messages in the current channel matching the given parameters. See [[Cleaning Messages]] for more detailed information about this command.

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

### `>>reason [case number] <reason>`
Edits a reason in the Moderation Log. If no case number is provided, Vortex will search the log for the most-recent case that has no provided reason.

## 📄 Settings Commands

## 📄 Automod Commands