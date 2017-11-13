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
    Item: 'wool:14:32'
    Lore:
    - '&732 red wool!'
```
***
### Summary ###
 - [Name](#name---required)
 - [Item](#item---required)
 - [Lore](#lore)
 - [Enchantments](#enchantments) *New*
 - [Hide-Flag](#hide---flag) *New*
 - [Placeholders](#placeholders)

#### Name - *Required* ####
***
Info: The name of the item in the specified frame  
Extra: Supports [Placeholders](#placeholders)!

#### Item - *Required* ####
***
Info: The itemstack to display in the specified frame  
Type: String or Integer  
Format: \[itemType\]:\<data\>:\<amount\>  
Extra:  
 - Data and Amount are optional!  
 - Data changes the data type, such as orange wool being "wool:1"  
 - Amount can be added without altering the data with a "0" in place for data  
 - Find a list of item names [here](http://minecraft-ids.grahamedgecombe.com)  

#### Lore ####
***
Info: The lore of the item   
Type: String list  
Extra: Supports [Placeholders](#placeholders)!

#### Enchantments ####
***
Info: List of enchantments to give an item   
Type: String list  
Format: \[enchantment\]:\<level\>  
Extra: View all enchantment types here  

#### Hide-Flag ####
***
Info: The hide flags to apply to this item  
Type: Integer  
Extra: You can specify the sum of the flag id's u need, or just put **63** for all flags ;)  
List:
 - **1** = Attributes
 - **2** = Destroys
 - **4** = Enchants
 - **8** = Placed-On
 - **16** = Potion-Effects
 - **32** = Unbreakable

#### Placeholders ####
***
Info: Placeholders that can be used inside any text area within the plugin!  
List:
 - All [placeholders](https://www.spigotmc.org/wiki/placeholderapi-placeholders/) from [PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/), if installed
 - %player_name%: Replaces with the name of the player
 - {perm:\<NODE\>,\<NODE2\>}: If a player has all permission nodes, that line will be shown, opposite action if node begins with a '-'.
 - {cords: x1=\<x1\> x2=\<x2\>, y1=\<x1\> y2=\<x2\>, z1=\<x1\> z2=\<x2\>}: If a player is within every coordinate specified, such as "{cords: x1=100 x2=500}". There MUST be a pair of x's, y's or z's! (Error log if lines are incorrect)
