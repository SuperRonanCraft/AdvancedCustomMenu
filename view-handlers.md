# View Handlers #
***
Info: View handlers help you be able to block players from even viewing an item before trying to display an item and its contents. This also allows for dynamic items, such as items that require to have a permission, and the other to not have that same permission. *All handlers must pass to show the item.*
```yaml
View-Handlers:
  Permission: 'example.savage'
  Price: 50
  Points: 25
```
### Summary ###
- [Permission](#permission)
- [Price](#price)
- [Points](#points)

***
- #### Permission ####
***
  Info: The Permission the player must have to view an item    
  Default Value: none  
  Extra:
    - Use '-' to have a player NOT have the permission to view
***
- #### Price ####
***
  Info: The amount of *money* a player must have in their account to view an item  
  Extra: [Vault](https://www.spigotmc.org/resources/vault.41918/) and an economy plugin like [Essentials](https://hub.spigotmc.org/jenkins/job/spigot-essentials/) needed to be enabled!  
  Default Value: 0 
***
- #### Points ####
*Added in 2.1.2*
***
  Info: The amount of points a player must have in their account to view an item  
  Extra: [PlayerPoints](https://dev.bukkit.org/projects/playerpoints) need to be enabled!  
  Default Value: 0 
