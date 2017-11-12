# Click Handlers #
***
```yaml
Click-Handlers:
  <UNIQUE-ID>:
    Click-Type: 'left, right, middle'
    Shift: false
    Commands:
    - 'me I am awesome!'
    Price: 10
    Price-Message: '%prefix% &7Seems like you are not rich enough to be awesome'
    Permission: 'example.savage'
    Permission-Message: '%prefix% &cLooks like you are not savage enough to use this command!'
    Close: true
    Delay: 10
    Delay-Message:
    - '%prefix% Too fast! You must wait {secondsleft} secs to use this again!'
```
### Summary ###
- [Click-Type](#user-content-click-type)
- [Shift](#user-content-shift)
- [Price](#user-content-price)
- [Price-Message](#user-content-price-message)
- [Permission](#user-content-permission)
- [Permission-Message](#user-content-permission-message)
- [Commands](#user-content-commands)
- [Close](#user-content-close)
- [Delay](#delay)
- [Delay-Message](#delay-message)
- [Sounds](#sounds)\*
***
- #### Click-Type ####
***
  Info: The click type a player must click an item to allow execution  
  Execution: Upon a player clicks the item  
  Default Value: none  
  Value Type: String Array  
  ~~------~~  
  The available nodes are listed below
  These can all be combined using commas *(ex: 'left, right, middle')*
  - **left** player must left click
  - **right** player must right click
  - **middle** player must middle click
  
***
- #### Shift ####
***
  Info: Specifies whether the handler needs a shift click  
  Execution: After [Click-Type](#user-content-click-type) if passed successfully   
  Default Value: none  
  Value Type: String  
  ~~------~~  
  The available nodes are listed below
  - **true** player must click the item while shifting
  - **false** player must click the item without shifting
***
- #### Price ####
***
  Info: The amount of Vault money required for the handler to execute commands  
  Execution: After [Shift](#user-content-shift) if passed successfully  
  Extra: Vault and an economy plugin need to be enabled!  
  Value Type: Integer  
***
- #### Price-Message ####
***
  Info: The message to send when the player does not have enough [Price](#user-content-price)  
  Extra: Supports placeholders *(Unique "%price%" placeholder to display the price automatically)*  
  Default Value: null  
  Value Type: String List  
  ```yaml
  Price: 'donator.epic'
  Price-Message:
  - '&cSorry %player_name%! &7You must have atleast $%price% to buy this!'
  ```
***
- #### Permission ####
***
  Info: The permission required to use this click handler  
  Execution: After [Price](#user-content-price)
  Extra: Use a '-' to not require the permission
  Value Type: String
***
- #### Permission-Message ####
***
  Info: The message to send when the player does not have [Permission](#user-content-permission)  
  Default value: Default "NoPermission" message  
  Extra: Supports placeholders  
  Value Type: String List  
  ~~------~~  
  Example:
  ```yaml
  Permission: 'donator.epic'
  Permission-Message:
  - '&cSorry %player_name%! &7You must be an &eEpic&7 donator to do this!'
  ```
***  
- #### Commands ####
***
  Info: List, supports placeholders  
  Execution: If the player has passed all the above click handlers  
  Extra: Supports placeholders   
  Value Type: List String  
  ~~------~~  
  You can start off a command with any of the following to execute a special event to a player
  - **server:** connect a player to a specific bungeecord server
  - **player:** execute the command as the player *(Default)*
  - **console:** execute the command as console
  - **chat:** make the player send a chat message
  - **message:** send a message to the player
  - **broadcast:** send a message to every player online
  - **give:** give a player an item *(same syntax as a frames [item](frames.md#item---required))*
  - **op:** execute a command as an operator
***
- #### Close ####
***
  Info: Closes the menu after a click handler  
  Default Value: 'false'  
  Value Type: String  
  ~~------~~  
  Available nodes are listed below
  - **true** will close the menu after the player clicks
  - **false** will not close the menu
  - **onsuccess** will close if all click-handlers were successfully passed
***
- #### Delay ####
***
  Info: Delay in seconds that a player must wait to click an item again  
  Default Value: null  
  Value Type: Integer
***
- #### Delay-Message ####
***
  Info: The message to send to a player when a delay is active  
  Default Value: null  
  Value Type: String List  
  ~~----------~~  
  Special Placeholders:  
  - **{hoursleft}**: get the amount of hours left
  - **{minutesleft}**: get the amount of minutes left in the hour
  - **{secondsleft}** get the amount of seconds left in the minute
  ***
- #### Sounds ####
***
  Extra: More sounds can be found here(https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Sound.html)!
  Info: The message to send to a player when a delay is active  
  Default Value: null  
  Value Type: Key List  
  ~~----------~~  
  Types:  
  - **Basic**: Executed everytime the item is clicked
  - **Success**: Played if the click-handlers were successful
  - **Failed**: Played if the click-handlers did not pass
  Example:
  ```yaml
  Sounds:
    Basic: 'ITEM_ARMOR_EQUIP_GENERIC'
    Success: 'ITEM_TOTEM_USE'
    Failed: 'ENTITY_GHAST_DEATH'
  ```
