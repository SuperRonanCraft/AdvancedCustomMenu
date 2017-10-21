# View Handlers #
***
Info: View handlers help you be able to block players from even viewing an item before trying to display an item and its contents. This also allows for dynamic items, such as items that require to have a permission, and the other to not have that same permission. *All handlers must pass to show the item.*
```yaml
View-Handlers:
  Permission: 'example.savage'
  Balance: 50
```
### Summary ###
- [Permission](#permission)
- [Balance](#balance)

***
- #### Permission ####
***
  Info: The Permission the player must have to view an item    
  Default Value: none  
  Extra:
    - Use '-' to have a player NOT have the permission to view
  
***
- #### Balance ####
***
  Info: The amount of *money* a player must have in their account to view an item    
  Default Value: none   
