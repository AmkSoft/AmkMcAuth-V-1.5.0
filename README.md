# AmkMcAuth-V-1.5.0
Easy to use (offline-mode) login authentication plugin

Bug-Fix: 

Thanks to bukkit.org member: "mdfm28", MySQL support is now optimized. mdfm28 rewrote the MySQL-update code as it was not optimal (and sometime AmkMcAuth did not update the Password resulting null values in the players table password column). Now every Password-Change that occurs wil instantly be written to the MySQL table. 
Mdfm28, thank you for your support and contrubution to this project to make it better.
New functionality: 

Added "Capcha" on Server join, The player has to click a random block in a temporary inventory when they enter/join the server. This can be enabled (default is disabled). Is the player clicks the wrong block he will be kicked with a message saying: "Failed to click Capcha? Kicked because you are not Human!"
Added a replacement for Password. Players can now use a minecraft block as a password. If they use this, AmkMcAuth will display an temporary inventory containing several minecraft blocks. The player has to click the block he want two use or set as his password. A player can use this if he types in the word 'menu' in place of the normal password he uses.
Typing in: "t\login menu"  wil display the inventory having minecraft blocks. The word 'menu' acts as a password replacement so AmkMcAuth knows the player wants to use the temporary  inventory to select his password-block.  This works for every command: register, login and changepass.
There is a new setting: "AutoMenu" that controles this behaviour. If the setting: "AutoMenu" is set to true, the "menu: become the auto-selected option, so the player does nog have to type it in, so if the player types: "t\l", "t\Login", "t\register" (no/blank password) AmkMcAuth assumes the "menu" option by default and shows the temporary inventory when there has to be a password-block selected.
