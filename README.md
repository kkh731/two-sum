
# UCS & A* algorithm

The following script is a modification of the original pymaze script to solve maze problems using the UCS (Uniform Cost Search) and A* (A-star) algorithms. Maze generation and the display of the generated maze remain identical to the original project.

## Dependencies / setup

The file was developed in a vscode IDE and used Python 3.7.0 and matplotlib 3.5.1. Below is a list of libraries output through the 'pip list' command.

    PS C:\Users\kihye\Documents\인지개\pymaze-master> pip list
    Package           Version 
    ----------------- -----------
    cycler            0.11.0
    fonttools         4.38.0
    kiwisolver        1.4.5
    matplotlib        3.5.1
    numpy             1.21.6
    packaging         24.0
    Pillow            9.5.0
    pip               10.0.1
    pyparsing         3.1.2
    python-dateutil   2.9.0.post0
    setuptools        39.0.1
    six               1.16.0
    typing-extensions 4.7.1

The first step is to install the dependancies by opening the terminal, navigating to
the MazeGenerator directory, and running. 

`pip install -r requirements.txt`

## Use Guide

This file operates through the code within the examples directory. There are a total of three executable scripts available.

**1. `quick_start.py`** 
The unchanged files from the original pymaze codebase, `quick_start.py`. By running quick_start.py scripts, you can generate random solvable mazes using the depth-first search and recursive backtracking algorithms. It uses the DFS algorithm to solve the maze.

**2. `solve_ucs.py`** 
Modification of the original pymaze codebase, `quick_start.py`. Like the original code, it generates a random solvable maze but uses the Uniform Cost Search algorithm to solve the maze.

**3. `solve_astar.py`**
Modification of the original pymaze codebase, `quick_start.py`. Like the original code, it generates a random solvable maze but uses the A* algorithm to solve the maze.


## Notes

You can run the code with the following command: 

    PS C:\Users\kihye\Documents\인지개\pymaze-master> python -m examples.solve_ucs

*Currently, the code for saving the result to an mp4 file is commented out in all three scripts due to an error encountered during the process. To save the output, please uncomment the following code:* 

    # If we want to save the maze & maze solution images along with their animations, we need to let the manager know
    # manager.set_filename("myFileName")



