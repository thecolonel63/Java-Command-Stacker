# Java-Command-Stacker
A simple command stacker for 1.17 and up. 

Credit to https://github.com/etiennestuder/java-ordered-properties for a simple way of making the properties in the config file ordered.

![alt text](https://github.com/thecolonel63/Java-Command-Stacker/raw/main/command_stacker_pics/file_menu.png?raw=true)
To start, this can read .mcfunction files to add multiple commands at a time. You can access this via File -> Open .mcfunction file

This contains a few configuration options:

"Disable wrapping /summon command inside spawn egg" - Disables the built in wrapping of the /summon command for a more generalized use.
"Keep stack on completion instead of removing" - Stops the command tower from clearing itself away - Useful if you use setblock commands on the tower blocks themselves, i.e for use of setting the tower blocks to a repeating - chain command block tower.
"Hide warning about command being longer than 256 characters" - Hides the warning message that shows up when the command is too long for the chat. 
"Hide warning about command being longer than max packet size in Multiplayer" - Hides the warning of an item that if given directly could inventory ban the player.

The toolbar also has "Item Details" where you can configure the generated item:

"Item Name" - Changes the Item Name of the spawn egg.
"Item Type" - Changes the type of spawn egg to be generated.
"Item Lore" - Changes the lore of the item generated.

Note that Item Name, Type, and Lore can all contain color codes, and properly handle " and ' characters. 

The Item Lore has been programmed to automatically convert \n into the proper format as well, although color codes must be repeated for every new line.

The "Summon Command Details" allow you to change the position of the stack when "Disable wrapping /summon command inside spawn egg" is checked.

Every configurable change previously mentioned is automatically saved to "command_stacker.properties" once the program is closed, and reloaded once the program is opened again.

The bottom bar contains an input for commands, as well as buttons to either copy the generated command or clear the whole list.

Once a command is added to the list, it can be moved up or down, copied, removed, or edited.

