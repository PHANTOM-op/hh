Vortex's automod features will ignore anyone with roles that it is ignoring. It will also ignore channels that are on its ignore list. You can see the list of ignored roles by running the `>>ignore` command with no arguments.

![ignore](http://i.imgur.com/SCpgqoy.png)

If a role has **[can't interact]** it means that it is above Vortex's highest role. If a role has **[elevated perms]** it means that it has a permission such as Ban Members, Manage Messages, Kick Members, Manage Server, or Administrator.

You can add roles (or channels) to this list by running the `>>ignore` command with the name of the role or a mention of the channel, and you can remove ignores that you added with the `>>unignore` command. *You can unignore any channels, but you cannot unignore roles that are ignored because of "can't interact" or "elevated perms".* **The easy fix for too many roles being ignored is to move the 'Vortex' role to the top of the role list!**

![setting](http://i.imgur.com/rFtXQxu.png)

Finally, you can disable anti-invite or anti-spam (and not the entirety of automod) in specific channels by adding `{invites}` and/or `{spam}` to the channel topic, respectively. This is useful if (for example) you want to allow a channel to have invites posted, but don't want automod to completely ignore the channel.