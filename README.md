# A Sudoku Solver with no brute-force space exploration 
Academical sudoku solvers always force us to use recursive BFS or DFS algorithms to resolve the sudoku.
I am a great fan of the sudoku game and, through time, I gained a lot of experience resolving them fast.
I always want to write a code version that works as my mental algorithm of resolution.

# A "Human-on-paper" based algorithm
The logic behind is the same as a human who tries to resolve sudoku on paper. Instead, on a mathematical POV, there is a strong pruning to the solution tree.
In fact, we are trying to eliminate as many candidate numbers from the empty cells as we can using some logic and graphs theory.
I took inspiration from an article that gave useful information about some logical tricks to solve the sudoku on paper and an illuminated blog post that gave some ideas about the graph theory behind it.
**The PDF which I took inspiration from is attached to the zip file**

[Blog link on graph theory](https://rakhman.info/blog/solving-sudoku-with-graph-theory/#fn-1)

[Box-line intersection logic](https://www.puzzlemystery.com/Sudoku/SudokuTutorial/Algorithms/BoxLineReduction.aspx)

[Pointing-pairs Strategy for solving sudokus](https://www.sudoku.org.uk/SolvingTechniques/IntersectionRemoval.asp)

# Note!
The algorithm needs to be optimized both on the data structures side and on the efficiency of some operations. 
Due to the lack of time caused by the time-consuming pre-learning material, some steps are ugly and inefficient.

An expanded node in this case is every guess I make for a single cell (every number I try to resolve the sudoku)
