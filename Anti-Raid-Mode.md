Raids can loosely be defined as a group of people (or a group of automated accounts) attempt to join a server en masse and cause disruption via spam messages, voice channel spam, or direct message attacks. Luckily, Vortex is adept at preventing this by allowing moderators to bar entry to the server and automatically cap how quickly users can join.

### What is Anti-Raid Mode?
* When Anti-Raid Mode is activated, it sets the server to the tableflip verification level (if not already there or higher)
* While Anti-Raid Mode is active, any member that joins the server will be sent a DM explaining that the server is under lockdown, and then kicked. This prevents any new members from joining the server.
* When Anti-Raid Mode is active, Vortex will provide a modlog entry for each kicked user if a modlog channel has been set.
* Bots do not affect Anti-Raid Mode, and bots can still be added to the server while Anti-Raid Mode is active.

### How to start and stop Anti-Raid Mode?
* Using the command `>>raidmode on` will enter Anti-Raid Mode.
* Using the command `>>raidmode off` will leave Anti-Raid Mode.

---

### What is Auto Anti-Raid Mode?
* Auto Anti-Raid Mode allows Vortex to automatically enable and disable Anti-Raid Mode when it detects the start and end of a raid.
* Vortex detects the start of a raid by a certain number of users joining within a certain time span.
* Vortex detects the end of a raid by no users attempting to join for several consecutive minutes.
* Bots do not affect Auto Anti-Raid Mode; Vortex will not consider (real, BOT-account) bots being added to a server when trying to detect a raid.

### How to enable and disable Auto Anti-Raid Mode?
* Using `>>autoraidmode <users>/<seconds>` will enable Auto Anti-Raid Mode to detect for raids of `<users>` number of users joining within `<seconds>` seconds. For example, `>>autoraidmode 15/5` will enable Anti-Raid Mode if 15 users join within a time span of 5 seconds.
* Using the command `>>autoraidmode on` will enable Auto Anti-Raid Mode at the default values of `10` users in `10` seconds (this is identical to running `>>autoraidmode 10/10`.
* Using the command `>>autoraidmode off` will set Vortex to not automatically take action.