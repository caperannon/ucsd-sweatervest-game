# Introduction #
The following are ideas for how we should construct the game. We need to have a good grasp on what objects need to interact with what, as well as how.

Try and be detailed!!!

# Classes: #

## Entity ##

---

**Description**

This is a basic entity that can be drawn to screen. It should have some sort of texture/image associated with it. The entity should have a position on screen representing where to draw it, as well as any other **BASIC** info needed by the draw method.


---

**Methods**

draw() - Draws the entity on screen at the entities position


---


## Moving Entity ##


---

**Description**

This is an entity that can move. Inherits everything an entity is, with the addition of being able to change the position. Now that it is moving we would want to keep track of the direction that it is moving, and possibly a destination. Should have some variable that sets the speed of the entity.


---

**Methods**

move() - Moves the entity to the given tile/point/whatever. Will also do checking to make sure that it only moves a max amount of its speed per call. If it cannot move the whole distance, set its destination and move there next time.