### What is Raid Mode?
* When Raid Mode is activated, it sets the server to the tableflip verification level.
* While Raid Mode is active, any member that joins the server will be sent a DM explaining that the server is under lockdown, and then kicked. This prevents any new members from joining the server.
* When Raid Mode ends, Vortex will provide a list of all members that were kicked if a modlog channel has been set.
* Bots do not affect Raid Mode, and bots can still be added to the server while Raid Mode is active.

### How to start and stop Raid Mode?
* Using the command `>>raidmode on` will enter Raid Mode.
* Using the command `>>raidmode off` will leave Raid Mode.
* Using the command `>>autoraidmode on` will set Vortex to watch for a raid, and automatically enable Raid Mode if it detects a raid (too many users joining in a very short time-span). Vortex will automatically end Raid Mode when it detects that the raid is over, or it can be ended at any time with `>>raidmode off`
* Using the command `>>autoraidmode off` will set Vortex to not automatically take action.