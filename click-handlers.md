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
***
- #### Click-Type ####
***
  Info: The click type a player must click an item to allow execution  
  Execution: Upon a player clicks the item  
  Default Value: none
  ---------------
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
  ---------------
  The available nodes are listed below
  - **true** player must click the item while shifting
  - **false** player must click the item without shifting
***
- #### Price ####
***
  Info: The amount of Vault money required for the handler to execute commands  
  Execution: After [Shift](#user-content-shift) if passed successfully  
  Extra: Vault and an economy plugin need to be enabled! 
***
- #### Price-Message ####
***
  Info: The message to send when the player does not have enough [Price](#user-content-price)  
  Extra: Supports placeholders *(Unique "%price%" placeholder to display the price automatically)*  
  Default Value: null  
  ```yaml
  Price: 'donator.epic'
  Price-Message: '&cSorry %player_name%! &7You must have atleast $%price% to buy this!'
  ```
***
- #### Permission ####
***
  Info: The permission required to use this click handler  
  Execution: After [Price](#user-content-price)
***
- #### Permission-Message ####
***
  Info: The message to send when the player does not have [Permission](#user-content-permission)  
  Default value: Default "NoPermission" message  
  Extra: Supports placeholders
  ---------------
  Example:
  ```yaml
  Permission: 'donator.epic'
  Permission-Message: '&cSorry %player_name%! &7You must be an &eEpic&7 donator to do this!'
  ```
***  
- #### Commands ####
***
  Info: List, supports placeholders  
  Execution: If the player has passed all the above click handlers  
  Extra: Supports placeholders  
  ---------------
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
  ---------------
  Available nodes are listed below
  - **true** will close the menu after the player clicks
  - **false** will not close the menu
  - **onsuccess** will close if all click-handlers were successfully passed
