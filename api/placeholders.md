# Placeholders #
The AdvancedCustomItemAPI allows for placeholders in almost every text field!
### Summary ###
- [Local](#local)
- [PlaceholderAPI](#placeholderapi)
***
- #### Local ####
***
  Info: Placeholders that can be used inside any text area within the plugin!  
  Values:
  - **%player_name%**: Replaces with the name of the player
  - **%player_uuid%**: Replaces with the players UUID
  - \***{perm:\<NODE\>,\<NODE2\>}**: If a player has all permission nodes, that line will be shown, opposite action if node begins with a '-'.
  - \***{cords: x1=\<x1\> x2=\<x2\>, y1=\<x1\> y2=\<x2\>, z1=\<x1\> z2=\<x2\>}**: If a player is within every coordinate specified, such as "{cords: x1=100 x2=500}". There MUST be a pair of x's, y's or z's! (Error log if lines are incorrect)
***
- #### PlaceholderAPI ###
***
  Info: Any placeholder from the [PlaceholderAPI](https://www.spigotmc.org/wiki/placeholderapi-placeholders/) from [PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/) plugin, if installed

##### Legend: #####
   \* = *Warning!* If using these, lines that require a value such as the name of an item or such, this will remove the line, making the title nulled, only use this in an items Lore!
