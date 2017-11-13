# Items #
Create a beautiful and interactive item, displaying useful information!  
View a menu with an example of all sections on the [Example.yml](files/Example.yml) file
```yaml
Items:
  <UNIQUEID>:
    Slot: 1
    Frame-Delay: 20 #Optional
    Frames: # Required
      <UNIQUEID>
        Name: '&aName of item'
        Item: 'wool'
        Lore:
        - '&aLine #1'
    Click-Handlers: #Optional
      <UNIQUEID>:
        - <Handlers>
    View-Handlers: #Optional
      - <Handlers>
```
***
### Summary ###
 - [Slot](#slot---required)
 - [Frame-Delay](#frame-delay)
 - [Frames](#frames---required)
 - [Click-Handlers](#click-handlers)
 - [View-Handlers](#view-handlers)
***
- #### Slot - *Required* ####
***
Info: The slot in which an item should be placed  
Value Type: Integer or Valid String   
Extra:   
 - The lastest item will override any previously placed items if two or more items have the same slot  
 - A slot must be within the total slots menu slots
Placeholders:

***
- #### Frame-Delay ####
***
Info: The amount of delay in ticks to change a frame  
Value Type: Integer  
Default Value: 20
***
- #### Frames - *Required* ####
***
Info: Each frame can have it's own item, name and lore!  
Value Type: Section of key-section pairs  
Extra: Go to the [Frame](frames.md) page to learn how to make a valid frame!
***
- #### Click-Handlers ####
***
Info: Whats an item without it doing comehting when you click it!  
Value Type: Section of key-section pairs  
Extra: Learn how to create a [click-handler](click-handlers.md)
***
- #### View-Handlers ####
*Added in 1.4.0*
***
Info: Want to make an admin menu? Make items invisible to certain players!  
Value Type: Section of keys  
Extra: Learn how to use [view-handlers](view-handlers.md)
