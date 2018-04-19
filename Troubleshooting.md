Oh no! Something isn't working!! Follow this handy guide for solving common issues!

# General Troubleshooting
### ⚠ Check Vortex's Permissions
Does Vortex have the necessary permissions to perform the action you want it to? Try giving Vortex the Administrator permission and moving the 'Vortex' role to the top (or near the top) of the role list. If this fixes your issue, Vortex didn't have sufficient permissions.

> ![RoleOrder](https://i.imgur.com/kJMIG8o.gif)

### ⚠ Check Discord's Status
It's possible that Discord may be having connectivity or latency issues. You can check Discord's status on [their status page](https://status.discordapp.com/) or on the [unofficial status server](https://discord.gg/jn7TAP8).

### ⚠ Check for Recent Updates
If there are any outages or other changes, check the `#announcements` channel on the [Support Server](https://discord.gg/0p9LSGoRLu6Pet0k)!


# Specific Troubleshooting
### ⚠ Vortex isn't deleting messages that it should be deleting!
1. Check that Vortex has sufficient permissions as described above.
2. Check which roles are being ignored with `>>ignored`. Take a look at the [[Ignoring Roles and Channels]] page for more information about ignored roles.
3. Check that you have the automod feature enabled with the `>>settings` command.

### ⚠ Muting isn't working!
1. Make sure that the Muted role exists and is configured properly for each channel. The easy way to configure it is to use the `>>setup muterole` command.
2. Make sure that there aren't any roles with a ✅ Send Messages override in your text channel settings; if a user has a role with a ✅ Send Messages override in a channel, they will be able to talk through the Muted role.


# Getting Further Support
### ⚠ Read the rest of the Wiki
Please make sure to read through this guide as well as the rest of the wiki before getting further support. You can find the main topics in the sidebar as well as the [[Homepage|Home]]

### ⚠ Join the Support Server
Feel free to join the [support server](https://discord.gg/0p9LSGoRLu6Pet0k) and ask questions in the `#support` channel. Please make sure to include the following:
1. The exact issue you are having
2. Your server's ID
3. A screenshot of your server's `>>settings`

### ⚠ Open an Issue
If you believe you have found a bug, you can [open an issue](https://github.com/jagrosh/Vortex/issues). Please do not use the issue page for questions or confusions; for those, join the [support server](https://discord.gg/0p9LSGoRLu6Pet0k).