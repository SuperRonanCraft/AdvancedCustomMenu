# Menu-Item #
Create/Identify the item which to open the menu with  
***
### Summary ###
  - [Item](#item)
  - [Name](#name)
  - [Lore](#lore)
  - [Give-Join](#give-join)
  - [Give-Slot](#give-slot)
  - [Ignore-Amount](#rows)
  - [Ignore-Durability](#commands)
  - [Ignore-Meta](#items)
***
- ### Item ###
***
  Info: The item type of the item 
  Value Type: String  
  Format: '[itemType]:\<data\>:\<amount\>'
  Extra: Required for create a Menu-Item
***
- ### Name ###
***
  Info: The display name of the item  
  Value Type: String
***
- ### Lore ###
***
  Info: The lore of the item  
  Value Type: String List  
  Extra: Supports [Placeholders](frames.md#placeholders)!
***
- ### Give-Join ###
***
  Info: Give the menu item upon a player joining  
  Value Type: Boolean
***
- ### Give-Slot ###
***
  Info: The slot which to give the menu item on  
  Value Type: Integer
***
- ### Ignore-Amount ###
***
  Info: When checking if the player interacted with an item, should we ignore item *amount*?  
  Value Type: Boolean
***
- ### Ignore-Durability ###
***
  Info: When checking if the player interacted with an item, should we ignore item *durability*?  
  Value Type: Boolean
***
- ### Ignore-Meta ###
***
  Info: When checking if the player interacted with an item, should we ignore item *meta*?  
  Value Type: Boolean
