# jsgames
A repository of javascript games. Purpose: Etudiar

### Concepts

#### Reflow and Repaint
- Reflow is the process of browser re-calculating the layout and position of the elements.
- Repaint is the process of browser re-drawing elements on the page.

*Browser Rendering Process*
1. _Generate the Render Tree_: The browser parses HTML to DOM and CSS to CSSOM creating the render tree.
   Which contains the structure of DOM and the style of each node.
2. _Generate the Layout Tree_: The browser needs to calculate the size and the position of each node on the screen.
3. _Painting_: The broser determines the order of painting the elements in the browser.

*When does Reflow or Repaint is triggered?* 
When we do something to change the layout or style.

*When does Reflow happen?*
It might happen when we update the size of a node. For example: a change in _width_, _height_, _font-size_.

*When does Repaint happen?*
When an element on the page needs to change color or other properties that do not affect the layout. For example:
_color_, _background-color_.


#### How movement is created in a video game?
It is created by drawing the screen repeatedly over time, a couple of dozen times 
per second, so that the sequence of images shown in quick sucession create the idea 
of movement.

To animate the game and create movement you will need to perform two actions in sequence 
and repeatedly:
1. Update the entities of the game.
2. Draw the canvas based on the current information about the entities of the game.