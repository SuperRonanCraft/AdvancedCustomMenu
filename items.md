# Items #
Create a beautiful and interactive item, displaying useful information!
***
### Summary ###
 - [Slot](#slot---required)
 - [Frame-Delay](#frame-delay)
 - [Frames](#frames---required)
 - [Click-Handlers](#click-handlers)

#### Slot - *Required* ####
***
Info: The slot in which an item should be placed  
Value Type: Integer   
Extra:   
 \- The lastest item will override any previously placed items if two or more items have the same slot  
 \- A slot must be less than the total slots shown in the menu to display

#### Frame-Delay ####
***
Info: The amount of delay in ticks to change a frame  
Value Type: Integer  
Default Value: 20

#### Frames - *Required* ####
***
Info: Each frame can have it's own item, name and lore!  
Value Type: Section of key-section pairs  
Extra: Go to the [Frame](frame.md) page to learn how to make a valid frame!

#### Click-Handlers ####
***
Info: Whats an item without it doing comehting when you click it!  
Value Type: Section of key-section pairs  
Extra: Learn how to create a [click-handler](click-handlers.md)
