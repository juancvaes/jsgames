# jsgames
A repository of javascript games. Purpose: Etudiar

#### How movement is created in a video game?
It is created by drawing the screen repeatedly over time, a couple of dozen times 
per second, so that the sequence of images shown in quick sucession create the idea 
of movement.

To animate the game and create movement you will need to perform two actions in sequence 
and repeatedly:
1. Update the entities of the game.
2. Draw the canvas based on the current information about the entities of the game.