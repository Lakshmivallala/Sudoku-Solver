# Sudoku-Solver

PROBLEM STATEMENT-

Using Backtracking algorithmic-technique, we recursively generate a digit from 1 to 9 and test if it can be placed in a particular
square. We cross check if the number can be placed there or not. If the number is placed incorrectly, we backtrack or remove the 
possibility of that particular number being placed in that square by eliminating it.

ALGORITHM:

1. Find a square that has no assigned number.
2. Return ‘True’ if all squares are assigned with a number.
3. Run a for loop for digits from 1 to 9
   a. We place the digit in the selected square if that digit does not repeat in the corresponding row and column. The digit should not 
repeat in the block as well.
   b. If the digit cannot be filled in the square, the option is eliminated and we move onto the next iteration of the loop.
   c. We similarly fill in the rest of the digits recursively.
4. Return ‘False’ if none of the digits can be placed in the block to activate backtracking.

