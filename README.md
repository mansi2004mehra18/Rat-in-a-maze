# Rat-in-a-maze

By backtracking


Question 1 :
Rat in a Maze

You are given a starting position for a rat which is stuck in a maze at an initial point (0, 0) (the maze can be thought of as a 2-dimensional plane). The maze would be given in the form of a square matrix of order N * N where the cells with value 0 represent the maze’s blocked locations while value 1 is the open/available path that the rat can take to reach its destination. The rat’s destination is at (N - 1, N - 1).

Your task is to find all the possible paths that the rat can take to reach from source to destination in the maze.

The possible directions that it can take to move in the maze are 'U'(up) i.e. (x, y - 1), 'D'(down) i.e. (x, y + 1), 'L' (left) i.e. (x - 1, y), 'R' (right) i.e. (x + 1, y).

(This problem is similar to Grid ways.)

                   Algorithm -

1. Create a solution matrix, initially filled with 0’s.
2. Create a recursive function which takes the initial matrix, output matrix and position of rat(i,j).
3. If the positon output is out of the matrix or the position is not valid then return.
4. Mark the position output[i][j] as 1 and check of the current position is destination or not. If destination is reached print the output matrix and return.
5. Recursively call for position (i+1, j) and (i, j+1).
6. Unmark position(i,j), i.e output[i][j] = 0.