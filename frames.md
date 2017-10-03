# Frames #
Create an item and make it animated too!
Info: Each frame must be in it's own section under "Frames"
Example:
```yaml
Frames:
  <UNIQUEID>:
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

#### Name - *Required* ####
***
Info: The name of the item in the specified frame  
Extra: Supports Placeholders!

#### Item - *Required* ####
***
Info: The itemstack to display in the specified frame  
Value Format: \[itemName\]:\<data\>:\<amount\>  
Extra:  
 - Data and Amount are optional!  
 - Data changes the data type, such as orange wool being "wool:1"  
 - Amount can be added without altering the data with a "0" in place for data  
 - Find a list of item names [here](http://minecraft-ids.grahamedgecombe.com)  
