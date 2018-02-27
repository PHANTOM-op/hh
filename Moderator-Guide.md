This is a guide for how to moderate a server using **Vortex**.

## 🔨 Introduction
Vortex has all the tools that you need to moderate effectively and efficiently. The first thing you'll want to do is check out what prefix Vortex is using on your server. You can always use the `>>` prefix, and use `>>settings` to see if the server has an additional prefix set (If you can't use the `>>settings` command, ask your admin or server owner if the server has an additional prefix enabled). Also check out the [[Moderation Commands section in the Full Command Reference|Commands#-moderation-commands]]

## 🔨 Moderation Commands
### Kicking, Banning, Softbanning, Muting
All of these commands are very straightforward. The syntax for each is `>>command <@users> [time] [reason]`. All of these can be used on multiple users at the same time, and supports user IDs instead of mentions if you prefer. Banning and muting support time aspects, and users will automatically be unbanned or unmuted after the amount of time has passed (kicking and softbanning do not support times). The reason is optional but highly recommended as it will be used in both Discord's Audit Log as well as Vortex's Moderation Log.

Examples:
```
>>kick @Looney#0001 @BeastInThaEast#0001 @Socrates#0001 raiding
>>mute @b1nzy#0851 @Shuu#0001 10 min Trolling
>>softban 103559217914318848
>>ban 120396406836953089 @Flam#0001
```

### Cleaning Messages
Vortex's `>>clean` command supports many options and filters. Check out the page on [[Cleaning Messages]] for a full overview of this feature.

### Managing Strikes
Some servers may heavily utilize the strike system, and others may not. Check with an admin or the server owner on the preference for using or not using the strike system. Check out the [[Strikes]] page for a full explanation of how strikes work!


## 🔨 The Moderation Log
The moderation log is a channel that keeps track of all moderator actions taken within the server. This log will track bans, unbans, softbans, timed bans, mutes, unmutes, timed mutes, kicks, cleaned messages, changes to the raid mode setting, and strikes, even if you don't use Vortex to perform the actions! When possible, make sure to provide reasons for all actions to keep the server organized!


## 🔨 Reasons
When banning or kicking someone with the Discord client, you're given a box in which to type a reason. Additionally, Vortex's commands support reasons for the actions that you may perform with them. However, sometimes you might not have time to write out a reason, and when the action gets put in the moderation log, it says `[no reason specified]`. Don't worry! You can update this reason retroactively with the `>>reason` command!

Usage:
```
>>reason [case number] <reason>
```
You can find the case number after the timestamp in the moderation log. If you don't provide a case number, Vortex will look for the most recent case that doesn't have a reason.

Examples:
```
>>reason 23 Spamming and being rude
>>reason Trolling
```