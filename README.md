# IC_PROJECT

We use two 2D arrays (maze and travelled). <br>
The maze array represents the structure of the maze, including walls, passages, and the starting ('S') and ending ('E') points. The outer boundary is initialized with walls ('*'), and all other cells are initialized as a wall or a path based on its position.<br>
The travelled array is used to keep track of which cells have been visited during the maze generation process. It uses the character 't' to represent the not visited cells.<br>
x_coordinate, y_coordinate are used to represent the current coordinates of cursor within the maze.<br>

PRIMS ALGO:<br>
A random number between 0 and 3 is generated. This number is used to determine the direction in which the algorithm will attempt to create the passage.<br>
A while loop contiinues untill all the neighbouring cell of the current cell are not visited. If all the neighbouring cells are visited, the loop breakes.<br>
Each random number represents a direction of motion. <br>
Eg) To move right, we check if the cell which is 2 cells away from the current cell in the right side(let us call it as taget cell) is visited or not. If the target cell is not visited, then a path is created from the cell adjacent to current cell and the target. The path is created by assigning the value of those cell in maze array as ' '.
If the target cell is already visited, we make the cell adjacent  to current cell as wall.<br>
