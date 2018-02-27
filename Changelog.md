## Version 2.0 (Beta)
`Feb 27, 2018`
### Command Changes
* Added `lookup` command to find info about users and guilds that Vortex can't see
* `userinfo` command now works with more than mentions and user IDs
* All moderation commands now accept user mentions, broken user mentions, and ids as valid input for users
* Because mod commands allow IDs as input, `>>hackban` is now just an alias of `>>ban`
* Several settings commands were added or updated

### AutoMod Changes
* All automod actions now utilize the new strikes system, so punishments are now centralized
  * Enabling/disabling features controls whether or how many strikes will be given for each action, and punishments are set separately through the `>>setstrikes` command
* Invite link detection improved
* Duplicate message detection improved
* Auto anti-raid mode threshold is now configurable

### Settings Changes
* Configurable prefix (default prefix will always work and cannot be removed)
* Added server activity logs, message edit/delete logs, and moderation logs
* Customizable log timezone
* Customizable 'Moderator Role' which can use all Moderation commands regardless of the role's native permissions

### Backwards Compatibility
This is a bit tricky, because the setup is vastly different from the previous version of Vortex. It hasn't been decided how to treat settings at this point. The current most-likely scenario is: If a server is using the Beta version, their settings will be transferred from that. Otherwise, if they are currently using Vortex, they will be automatically set up with a comparable set of settings.