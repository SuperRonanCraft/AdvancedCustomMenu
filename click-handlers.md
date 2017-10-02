# Click Handlers #

### Summary ###
- [Click-Type](#user-content-click-type)
- [Shift](#user-content-shift)
- [Price](#user-content-price)
- [Price-Message](#user-content-price-message)
- [Permission](#user-content-permission)
- [Permission-Message](#user-content-permission-message)
- [Commands](#user-content-commands)
- [Close](#user-content-close)

- #### Click-Type ####
  Default value: none
  Info: The click type a player must click an item to allow execution
  Execution: Upon a player clicks the item
  \---
    Types accepted are 'left', 'right' or 'middle' (can be combined with a comma "," seperating each)
    
- #### Shift ####
  Default value: none
  Info: Specifies whether the handler needs a shift click
  Execution: After [Click-Type](#user-content-click-type) if passed successfully
  \--- 
    Types accepted are 'true' or 'false'

- #### Price ####
  Info: The amount of Vault money required for this handler  
  Execution: After [Shift](#user-content-shift) if passed successfully
  \---
    Vault and an economy handler (like Essentials) need to be installed of course  

- #### Price-Message ####
  Supports placeholders  
  Default value: '&cYou don't have enough money for that!'  
  \---
    The message to send when the player does not have [Price](#user-content-price)  

- #### Permission ####
  Info: The permission required to use this click handler
  \---
    Supports placeholders

- #### Permission-Message ####
  Info: The message to send when the player does not have [Permission](#user-content-permission)
  Default value: Config files default "NoPermission" node  
  \---
    Supports placeholders
  
- #### Commands ####
  Info: List, supports placeholders  
  Execution: If the player has passed all the above click handlers
  \---
    All commands will be made as the player

- #### Close ####
  Info: Closes the menu after a click handler
  Default value: 'false'
  \---
    - The 'true' value will close the menu when [Commands](#user-content-commands) were successfully passed
    - 'false' will keep the menu open no matter what (default)
