# Sudoku_Solver

Q: How do we use constraint propagation to solve the naked twins problem?  
A: Naked twins involves two boxes that can fit exactly the same values of length 2. If that is the case then it must be that each one must have one of the digits among their peers. That also means that any of their other peers cannot have those two digits. Therefore, we iterate through their peers and eliminate those two digits from each box that are not the twins.

Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: We simply add the new diagonal constraints to the unitlist. Our program was able to solve the sudoku with the unitlist before so adding it would simply make the program go through the diagonal units in addition to what we previously had and solve the sudoku puzzle.

* `solver.py` - Sudoku Solver.
* `PySudoku.py` - This is code for visualizing the solution.
* `visualize.py` - This is code for visualizing the solution.
