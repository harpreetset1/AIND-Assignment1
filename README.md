# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: Naked Twins in the grid can be identified where a unit (row/ column/ 3x3 box) has 2 boxes with the same possibility of missing values. Either of the 2 values can be applied to either of the boxes. We can use the value of these twins as constraint and eliminate these 2 options from other missing values within a unit.        

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: All we need to do here is add another dimension in the unitlist object. This dimension is diagonals of the grid. While processing the grid we iterate through each unit type (row/ column/ 3x3 box) to see that a unit shouldnt have ant of the 1-9 values repeating. These unit types act as constraints for finding out the values. By adding diagonals as another unit type we can add that constraint and while finding out the values we end up getting non repeating values in 9 boxes of diagonal. 

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in function.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.
