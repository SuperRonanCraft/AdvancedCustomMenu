# Menus #
The fudamental reason you have this plugin installed!  
View a menu with an example of all sections on the [Example.yml](files/Example.yml) file
***
### Summary ###
  - [Title](#title---required)
  - [Menu-Item](#menu-item)
  - [Auto-Close](#auto-close)
  - [Frame-Delay](#frame-delay)
  - [Type](#type)
  - [Rows](#rows)
  - [Commands](#commands)
  - [Items](#items)
***
- ### Title - *Required*
***
  Info: The title of the menu when it's openned  
  Value Type: String List  
  Extra:  
  - Animateable if multiple lines are applied  
  - Supports Placeholders!
***
- ### Menu-Item ###
***
  Info: The item to open the menu with  
  Value Type: Section of Keys  
  Extra: Learn how to create a valid [menu-item](#menu-item.md) on the wiki
***
- ### Auto-Close ###
*Added in 1.2.1*
***
  Info: Amount of time in ticks to close a menu after it's been opened   
  Value Type: Integer  
  Default Value: 0  
  Extra:  
  - Set to '0' to disable
  - Does not reset if a player clicks an item
***
- ### Frame-Delay ###
***
  Info: The amount of ticks between each frame  
  Value Type: Integer  
  Default Value: 20
***
- ### Type ###
***
  Info: The kind of inventory type to display  
  Default Value: CHEST  
  Value Types:
  - **Chest** If the type is a chest, look at [rows](#rows)
  - **Dispenser** Create an dispenser inventory *(9 slots)*
  - **Dropper** Create an dropper inventory *(9 slots)*
  - **Hopper** Create an hopper inventory *(5 slots)*   
***
- ### Rows ###
***
  Info: The amount of rows a menu should display  
  Value Type: Integer  
  Extra: Any value above 6 will give a bugged texture!
***
- ### Commands ###
***
  Info: An alias to open the menu with a quick command  
  Value Type: String  
  Extra: Use ';' to specify mutliple commands  
  Example:
  ```yaml
  Commands: 'command1; command2'
  ```
***
- ### Items ###
***
  Info: The fundamental reason to have an menu, create items without allowing players to take them!  
  Value Type: Section of Keys  
  Extra: View the [Items](items.md) page to view how to create an item
