# Exploding Kittens

## by CDT Tamar DeWilde section K2

# Game Rules
#
### Exploding Kittens is a simulation of a four-player card game.


## Equipment: 
-----
### Exploding Kittens is played with a 49 card deck. 

#### The deck contains:
- #### 4 **Exploding Kitten cards**
- #### 6 **Defuse cards**
- #### 5 **Nope cards**
- #### 4 **Skip cards**
- #### 15 **Mitten Pair Steal cards**
- #### 15 **Kitten Pair Steal cards**
### Each player will start with 7 playing cards. Before distributing the cards remove all of the **Exploding Kitten** and **Difuse cards** from the deck. Distribute 6 cards from the deck to each player in addition to 1 **Difuse card**. Distribute the cards in the starting order of game play: Mark, Daniel, Ronak, Nadia. Place the remaining **Diffuse cards** and 3 **Exploding Kitten cards** back into the deck. It is important to only place 3 **Exploding Kitten** cards back into the deck to ensure that eventually 1 player will avoid exploding. Each player's status will be recorded to the side to indicate if a player is still Surviving or has been Exploded. 

## Game Play:
-----
### Before begining gameplay it is important to understand what the cards do. The **Exploding Kitten card** results in a player's Explosion. A **Diffuse card** defuses the **Exploding Kitten card**. The goal is to get as many **Defuse cards** as possible. A player who draws an **Exploding Kitten card**, but plays a **Diffuse card** will place the **Exploding Kitten card** back into the deck. The **Skip card** can be used by any player to skip the next players turn. The **Nope card** can be by any player following a **Skip**. When the **Nope card** is played the effects of the **Skip** will reverse and it will become the previous players turn. The **Mitten Pair Steal card** and the **Kitten Pair Steal card function** the same way. If a player has at least 2 of the card, then the player will recieve 1 card from the next players hand. It is important to note that the **Mitten Pair Steal** and the **Kitten Pair Steal cards** can not be mixed and matched. For each turn each player will select a card from their hand to play, carry out the actions associated with that card, and then draw a card from the top of the deck. 

### There will also be 4 _strategies_ that each player could use:
1. *Default*
2. *Aggressive*
3. *Defensive*
4. *Evasive*


## Objective:
-----
### If you explode you lose. The last surviving player wins the game!

## Open Design
### In our design, we had made it so that classes would need to have specific functions calling for vital vriables rather than giving every class access to all the variables. 

### Example: To display the pile on the GUI, the view would call controller, which would call model wich was made up from the Menu. Then the Menu would have a function that would return the Card value from the Board.
______________

## Fail-Safe Defaults
### With limiting access between classes for when it comes to variables, classes would not have access to them unless explicitly stated.

### Example: View does not have the acess to the functional files so view has to go through controller and then model to do what it needs to do. 

______________

## Economy of Mechanisms
### Rather than having complicated functions and classes, we decided to make our's simple and few. This prevented issues of having redundant functions that would possibly do something slightly different.

### Example: Rather than making a whole other system for placing the cards on the view, we used the player order from the model (through the controller) to be able to effectively place the cards on the view. 

