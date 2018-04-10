# Overview
## 🛡 What is Auto Moderation?
Auto Moderation is Vortex keeping your server clean so you don't have to. It also keeps watch even when you're sleeping or away, and isn't susceptible to content that could crash or lag your client.

## 🛡 Quick Setup
To quickly start using the recommended set of automod features, simply run `>>setup` and then select 'AutoMod.'

# Specific Features
## 🛡 Anti-Advertisement/Referral
The anti-invite feature makes Vortex automatically delete invite links to other Discord servers. To begin using this feature, use the `>>antiinvite <strikes>` command. Replace `<strikes>` with the number of strikes that Vortex should assign the user for posting invite links. You can also prevent referral (and other malicious) links with the anti-referral system. This uses the same format, `>>antireferral <strikes>`.<br>
**Recommended (Invites): `>>antiinvite 2`**<br>
**Recommended (Referral): `>>antireferral 3`**

## 🛡 Resolving Links (Redirect Links)
Users often try to get around invite and referral link filters using redirect sites such as goo.gl or bit.ly, or even customized domains. Vortex's link resolving protects against all kinds of redirect sites, including header/javascript redirects and redirect chaining.<br>
**Recommended: `>>resolvelinks ON`**<br>
🌟 Resolving Links is only available with [[Vortex Pro]]

## 🛡 Anti-Copypasta
This feature prevents users from sending "copypastas", or bits of copy-pastable (and often spammed) text. These range from annoying unicode like cooldog to false (fake) Discord-related PSAs.<br>
**Recommended: `>>anticopypasta 1`**

## 🛡 Anti-Duplicate
This feature prevents common spam by detecting duplicate messages. To set this feature, use `>>antiduplicate <strike threshold> [delete threshold] [strikes]`. Vortex will start deleting messages once the `[delete threshold]` duplicate is sent, and start assigning `[strikes]` strikes for each duplicate starting with the `<strike threshold>` duplicate.<br>
**Recommended: `>>antiduplicate 4 2 1`<br>**
(start deleting on the 2nd duplicate message, and assign 1 strike for every duplicate starting with the 4th)

## 🛡 Maximum Mentions
This feature stops mention spammers from performing mass-mentions of users (or roles). Any user mentioning more than the set maximum will have their message deleted and assigned a strike for every mention above the maximum. To set up the maximum mentions for user mentions, use `>>maxmentions <number>`. For roles, use `>>maxmentions role <number>`.<br>
**Recommended (user): `>>maxmentions 10`**<br>
**Recommended (role): `>>maxmentions role 4`**

## 🛡 Maximum Lines
Enabling this will set a maximum number of lines users' messages can be. Any messages with more lines than the maximum will be deleted, and users will receive 1 strike for every multiple of up-to the maximum number of lines (For example, setting the max to 10: 11-20 lines = 1 strike, 21-30 lines = 2 strikes, etc). To enable this, use `>>maxlines <number>`, where `<number>` is the maximum number of lines.<br>
**Recommended: `>>maxlines 10`**

## 🛡 Automatic Anti-Raid Mode
This feature has Vortex watch for potential raids and automatically enable Anti-Raid Mode if a raid is detected. To enable this, use `>>autoraidmode <joins>/<seconds>`, which will enabled Anti-Raid Mode if the number of joins per time exceeds the provided values (or `>>autoraidmode ON` to use 10 joins in 10 seconds).<br>
**Recommended: `>>autoraidmode 10/10`**

## 🛡 Automatic Dehoisting
This feature prevents users from setting their username or nickname to be listed higher in the user list. For example, users frequently prefix their username with `!` to be listed first. <br>
**Recommended: `>>autodehoist !`**