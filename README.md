# hw2-assignment

## short explaination 
Use the turn variable to track the turn, when it's equal to 1 meaning it's player 1's turn (AI's turn). 
When player remove stick in the correct way (1 or 2 sticks only) then the turn variable change to 2 meaning that player 2 will plays next turn.

To make computer smart, it needs to understand logic of this game. It's found that 1, 4, 7, 10,... is the losing position which meaning that
if you get those numbers into your turn, you'll definitely lose (if the oppenent play it correctly).
So the idea is to remove sticks to those numbers into the oppenent's turn, and there is a pattern that can be written as:
  Sticks in the pile % 3 = 0 : remove 2 sticks
  Sticks in the pile % 3 = 1 : remove 1 or 2 does matter (You definitely lose if the opponent play it right)
  Sticks in the pile % 3 = 2 : remove 1 sticks
As long as the computer does start the game in the losing position (1, 4, 7, 10, 13,... or n % 3 = 1) the computer will always win.
