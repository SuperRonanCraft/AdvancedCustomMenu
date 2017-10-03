# Menus #
The fudamental reason you have this plugin installed!
***
### Summary ###
  - [Title](#title)
  - [Frame-Delay]
  - [Rows]
  - [Commands]
  - [Items]

### Title - *Required*
***
Info: The title of the menu when it's openned  
Value Type: String List  
Extra:  
 \- Animateable if multiple lines are applied  
 \- Supports Placeholders!

### Frame-Delay ###
***
Info: The amount of ticks between each frame  
Value Type: Integer  
Default Value: 20

### Rows - *Required*
***
Info: The amount of rows a menu should display  
Value Type: Integer  
Extra: Any value above 6 will give a bugged texture!

### Commands ###
***
Info: An alias to open the menu with a quick command  
Value Type: String  
Extra: Use ';' to specify mutliple commands  
Example:
```yaml
Commands: 'command1; command2'
```

### Items ###
***
Info: The fundamental reason to have an menu, create items without allowing players to take them!
Value Type: Section of Keys
Extra: View the [Items](items.md) page to view how to create an item
