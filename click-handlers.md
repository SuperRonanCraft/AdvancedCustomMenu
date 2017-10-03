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
  Info: The click type a player must click an item to allow execution  
  Execution: Upon a player clicks the item  
  Values:  
    \- Types accepted are 'left', 'right' or 'middle' (can be combined with a comma "," seperating each)  
  Default Value: none
    
- #### Shift ####
  Info: Specifies whether the handler needs a shift click  
  Execution: After [Click-Type](#user-content-click-type) if passed successfully  
  Values:  
    \- 'true' or 'false'  
  Default Value: none

- #### Price ####
  Info: The amount of Vault money required for this handler  
  Execution: After [Shift](#user-content-shift) if passed successfully  
  Extra: Vault and an economy plugin need to be enabled! 

- #### Price-Message ####
  Info: The message to send when the player does not have [Price](#user-content-price)  
  Extra: Supports placeholders  
  Default Value: null

- #### Permission ####
  Info: The permission required to use this click handler  
  Execution: After [Price](#user-content-price)

- #### Permission-Message ####
  Info: The message to send when the player does not have [Permission](#user-content-permission)  
  Default value: Config files default "NoPermission" node  
  Extra: Supports placeholders
  
- #### Commands ####
  Info: List, supports placeholders  
  Execution: If the player has passed all the above click handlers  
  Extra: Supports placeholders

- #### Close ####
  Info: Closes the menu after a click handler  
  Values:  
    \- 'true' value will close the menu when [Commands](#user-content-commands) were successfully passed  
    \- 'false' will keep the menu open no matter what (default)  
  Default Value: 'false'
