# Java-Command-Stacker
A simple command stacker for 1.17 and up. 

Building:

1) Download the project.
2) Run "gradlew shadowJar" inside the root of the project.
3) The completed jarfile will appear in "app/build/libs".

Credit to https://github.com/etiennestuder/java-ordered-properties for a simple way of making the properties in the config file ordered.

![file menu image](https://github.com/thecolonel63/Java-Command-Stacker/raw/main/command_stacker_pics/file_menu.png?raw=true)

To start, this can read .mcfunction files to add multiple commands at a time. You can access this via File -> Open .mcfunction file

This contains a few configuration options:

![options menu image](https://github.com/thecolonel63/Java-Command-Stacker/raw/main/command_stacker_pics/options_menu.png?raw=true)

"Disable wrapping /summon command inside spawn egg" - Disables the built in wrapping of the /summon command for a more generalized use.

"Keep stack on completion instead of removing" - Stops the command tower from clearing itself away - Useful if you use setblock commands on the tower blocks themselves, i.e for use of setting the tower blocks to a repeating - chain command block tower.

"Hide warning about command being longer than 256 characters" - Hides the warning message that shows up when the command is too long for the chat. 

"Hide warning about command being longer than max packet size in Multiplayer" - Hides the warning of an item that if given directly could inventory ban the player.

The toolbar also has "Item Details" where you can configure the generated item:

![item details menu image](https://github.com/thecolonel63/Java-Command-Stacker/raw/main/command_stacker_pics/item_details_menu.png?raw=true)

"Item Name" - Changes the Item Name of the spawn egg.

"Item Type" - Changes the type of spawn egg to be generated.

"Item Lore" - Changes the lore of the item generated.

Note that Item Name, Type, and Lore can all contain color codes, and properly handle " and ' characters. 

The Item Lore has been programmed to automatically convert \n into the proper format as well, although color codes must be repeated for every new line.

![summon details menu image](https://github.com/thecolonel63/Java-Command-Stacker/blob/main/command_stacker_pics/summon_details_menu.png?raw=true)

The "Summon Command Details" allow you to change the position of the stack when "Disable wrapping /summon command inside spawn egg" is checked.

Every configurable change previously mentioned is automatically saved to "command_stacker.properties" once the program is closed, and reloaded once the program is opened again.

![example command list image](https://github.com/thecolonel63/Java-Command-Stacker/blob/main/command_stacker_pics/example_command_list.png?raw=true)

The bottom bar contains an input for commands, as well as buttons to either copy the generated command or clear the whole list.

Once a command is added to the list, it can be moved up or down, copied, removed, or edited.

Command edit popout:
![command edit popout image](https://github.com/thecolonel63/Java-Command-Stacker/blob/main/command_stacker_pics/command_edit_popup.png?raw=true)

Once you are done modifying the list, you can save it by clicking the "Copy to Clipboard" button:
![command copied to clipboard image](https://github.com/thecolonel63/Java-Command-Stacker/blob/main/command_stacker_pics/command_copied_to_clipboard.png?raw=true)

Warning for /give command longer than 256 characters:
![command longer than 256 characters image](https://github.com/thecolonel63/Java-Command-Stacker/blob/main/command_stacker_pics/256_length_warning.png?raw=true)

Warning for /give command longer than maximum packet size:
![command longer than max packet size image](https://github.com/thecolonel63/Java-Command-Stacker/blob/main/command_stacker_pics/long_packet_warning.png?raw=true)
