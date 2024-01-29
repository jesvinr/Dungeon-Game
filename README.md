
**Dungeon Game**

**Description**
This Java program, named Dungeon game, is a simple text-based dungeon adventure game. 
The game involves an adventurer, a monster, gold, pits, and a trigger in a nxn dungeon. 
The objective is to find the minimum steps required for the adventurer to reach the gold while avoiding the monster and pits.

**How to Play**
_Adventurer Location:_ Enter the initial location of the adventurer in the dungeon when prompted.

_Monster Location:_ Specify the initial location of the monster in the dungeon.

_Gold Location:_ Provide the location of the gold in the dungeon.

_Pits:_ Enter the number of pits in the dungeon and their respective locations.

_Trigger Location:_ Define the location of the trigger in the dungeon.

The program will display the dungeon layout with 'A' representing the adventurer, 'M' for the monster, 'G' for gold, 'P' for pits, and 'T' for the trigger.

The program will then check if the monster can reach the adventurer. If so, it will terminate the game, indicating that the monster will catch and kill the adventurer.

Otherwise, the program will calculate and display the minimum steps required for the adventurer to reach the gold.

**Code Structure**
The code uses a recursive approach (_findStep()_ method) to explore possible paths in the dungeon until the adventurer reaches the gold or trigger.

The _isValidMove()_ method checks if a move is within the bounds of the dungeon and is a valid open path.

The _differenceBetweenMonsterAndAdventurer()_ method calculates the steps between the adventurer and gold, monster and gold, and trigger and adventurer/monster.

The _givingInput()_ method initializes the dungeon layout based on the user-provided locations of gold, monster, trigger, and pits.

**Example Input:**

Enter adventurer location in dungeon...
0 0
Enter Monster location in dungeon...
3 3
Enter Gold location in dungeon...
2 2
Enter number of pits..
2
1 1
3 1
Enter trigger location:
1 3
Example Output

A000
0000
00G0
0M0T

No possible solution
Monster will catch you and kill you!!!

**Notes**
The game may have multiple valid solutions, and the minimum steps displayed depend on the order in which paths are explored.

The program assumes valid user inputs and does not perform extensive error checking.

**Dependencies**
The program uses the Scanner class for user input.
**Author**
This program was written by Jesvin R.
