## Version 2.1
`May 13, 2018`
### Command Changes
* Added `unban` command to unban users
* Added `announce` command to ping a role with a message in a specified channel
* Added `audit` command to see recent audit log entries
* Modified dehoisting characters as Discord has blocked more invisible characters that were previously used for dehoisting.


## Version 2.0-Beta
`April 20, 2018`
### Command Changes
* Added `lookup` command to find info about users and guilds that Vortex can't see
* Added invite pruning to prune low-use invites
* `userinfo` command now works with more than mentions and user IDs
* `roleinfo` command added
* All moderation commands now accept user mentions, broken user mentions, and ids as valid input for users
* Bans and mutes can now be timed
* Because mod commands allow IDs as input, `>>hackban` is now just an alias of `>>ban`
* Several settings commands were added or updated

### AutoMod Changes
* All automod actions now utilize the new strikes system, so punishments are now centralized
  * Enabling/disabling features controls whether or how many strikes will be given for each action, and punishments are set separately through the `>>setstrikes` command
* Invite link detection improved
* Duplicate message detection improved
* Auto anti-raid mode threshold is now configurable
* Added automatic and by-command dehoisting of members (prevent using names/nicknames to increase position in online list)

### Settings Changes
* Configurable prefix (default prefix will always work and cannot be removed)
* Added server activity logs, message edit/delete logs, and moderation logs
* Customizable log timezone
* Customizable 'Moderator Role' which can use all Moderation commands regardless of the role's native permissions

### Backwards Compatibility
This is a bit tricky, because the setup is vastly different from the previous version of Vortex. If a server uses or has ever set settings on Beta, those settings will be transferred. If a server has not used Beta and has settings on Vortex 1.X, some settings will be transferred and modified to fit 2.0's feature set.