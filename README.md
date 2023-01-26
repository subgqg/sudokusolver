# sudokusolver
This code is a Python program that solves a sudoku puzzle using backtracking. The puzzle is represented by a 2-dimensional list called "board" and the solution is also stored in this list.

The main function is the "solve" function which takes a board as an input. It first calls the "find_empty" function to find the first empty cell in the puzzle. If no empty cells are found, it returns True indicating that the puzzle is solved. If an empty cell is found, it assigns the row and column values to "row" and "col" respectively.

The program then enters a for loop that iterates from 1 to 10. For each iteration, it calls the "valid" function to check if the current number can be placed in the current empty cell. If it can, the number is placed in the cell and the solve function is called recursively. If the function returns True, the function returns True. If the function returns False, the number is removed from the cell and the loop continues. If the loop completes and no valid numbers were found, the function returns False.

The "valid" function checks if a given number can be placed in a given cell by checking the row, column, and 3x3 box of the cell. If the number already exists in any of these, it returns False. Otherwise it returns True.

The "print_board" function prints the board in a human-readable format, with horizontal and vertical lines separating the 3x3 boxes.

The "find_empty" function iterates through the board and returns the coordinates of the first cell that contains the value 0. If no empty cells are found, it returns None.

The board is then printed before and after the solve function is called, so you can see the initial puzzle and the solution.
