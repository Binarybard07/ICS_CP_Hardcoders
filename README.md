# IC_PROJECT

We use two 2D arrays (maze and travelled). Maze is used to represent the maze and travelled keeps track on the cells visited.
The outer border of maze is set to walls(*).
The cells which have been visited are marked as 't' in the travelled Array.
The spaces (cells set to ' ') in the maze array represent open paths where the maze algorithm can create passages.

PRIMS ALGO:
From the current cell, it randomly selects a neighbouring cell(up, down, left, right) that has not been visited. If the randomly choosen neighbouring cell is already visited, we would again choose the neighbouring cell unless an unvisited cell is not obtained.
If the neighboring cell has not been visited, it creates a passage by updating the maze array and marking the corresponding cell as visited in the travelled array.
The function continues this process until all neighboring cells are visited.
