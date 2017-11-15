# Frames #
Create an item and make it animated too!  
Info: Each frame must be in it's own section under "Frames"
Example:
```yaml
Frames:
  <UNIQUEID>:
    Enchantments:
    - sharpness:1
    Hide-Flag: 63
    Name: '&aExample'
    Item: 'wool:1:64'
    Lore:
    - '&764 orange wool!'
  <UNIQUEID>:
    Name: '&aExample#2'
    Skull-Owner: '%player_name%'
    Item: 'wool:14:32'
    Lore:
    - '&732 red wool!'
```
***
### Summary ###
 - [Name](#name---required)
 - [Item](#item---required)
 - [Lore](#lore)
 - [Enchantments](#enchantments)
 - [Hide-Flag](#hide-flag)
 - [Skull-Owner](#skull-owner)
 - [Egg-Type](#egg-type)
 - [Color](#color)
 - [Banner-Pattern](#banner-pattern)
 - [Placeholders](#placeholders)
***
- #### Name - *Required* ####
***
Info: The name of the item in the specified frame  
Extra: Supports [Placeholders](#placeholders)!
***
- #### Item - *Required* ####
***
Info: The itemstack to display in the specified frame  
Type: String or Integer  
Format: \[itemType\]:\<data\>:\<amount\>  
Extra:  
 - Data and Amount are optional!  
 - Data changes the data type, such as orange wool being "wool:1"  
 - Amount can be added without altering the data with a "0" in place for data  
 - Find a list of item names [here](http://minecraft-ids.grahamedgecombe.com)  
***
- #### Lore ####
***
Info: The lore of the item   
Type: String list  
Extra: Supports [Placeholders](#placeholders)!
***
- #### Enchantments ####
*Added in 1.4.0*
***
Info: List of enchantments to give an item, more enchants [here](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/enchantments/Enchantment.html)   
Type: String list  
Format: \[enchantment\]:\<level\>   
***
- #### Hide-Flag ####
*Added in 1.4.0*
***
Info: The hide flags to apply to this item  
Type: Integer  
Extra: You can specify the sum of the flag id's u need, or just put **63** for all flags ;)  
Valid Entries:
 - **1** = Attributes
 - **2** = Destroys
 - **4** = Enchants
 - **8** = Placed-On
 - **16** = Potion-Effects
 - **32** = Unbreakable
***
- #### Skull-Owner ####
*Added in 1.4.1*
***
Info: The owners name of the head to show  
Extra:
 - Supports Placeholders  
 - Will replace current item with a skull (if invalid)  
Disclaimer: *This feature is highly experimental, only player names are supported as of now.*  
***
- #### Egg-Type ####
*Added in 1.4.3*
***
Info: The entity egg type, view valid entity types [here](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/entity/EntityType.html)
Extra: Will replace current item with a spawn egg (if invalid)
***
- #### Color ####
*Added in 1.4.3*
***
Info: The color to give leather armor, tipped arrows or potions, generate color codes [here](https://minecraftcommand.science/armor-generator)  
Extra: Will replace current item (if invalid) with a random valid item  
Disclaimer: There is *no* way of removing the color indicator, as it is client side!  
Valid Entries:
 - **\<red\>, \<green\>, \<blue\>** Each color ranges from 0 to 255
 - **\<raw rgb\>** The raw color value, such as '16711680' for red
 - **#RRGGBB** R, G and B range from 0-9 and A-F
***
- #### Placeholders ####
***
Info: Placeholders that can be used inside any text area within the plugin!  
List:
 - All [placeholders](https://www.spigotmc.org/wiki/placeholderapi-placeholders/) from [PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/), if installed
 - %player_name%: Replaces with the name of the player
 - {perm:\<NODE\>,\<NODE2\>}: If a player has all permission nodes, that line will be shown, opposite action if node begins with a '-'.
 - {cords: x1=\<x1\> x2=\<x2\>, y1=\<x1\> y2=\<x2\>, z1=\<x1\> z2=\<x2\>}: If a player is within every coordinate specified, such as "{cords: x1=100 x2=500}". There MUST be a pair of x's, y's or z's! (Error log if lines are incorrect)
