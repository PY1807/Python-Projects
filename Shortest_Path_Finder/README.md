# Explanation

In this problem, we have a grid consisting of '#','O','' and 'X'.
'#' denotes that it is a blocked path.
'O' denotes that it is the starting point.
''denotes blank cell which can be included in the path.
'X' denotes that it is the ending point where we have to reach.

What we have to do is that is we have to find the shortest path from starting point to the ending point.

I am using the 'curses' module in Python's library to create the visualization of the grid and all the paths 
that are possible while finding out the best path.

ALgorithm used:Breadth First Search

I have used the queue data structure that will help me traverse through all possible paths and then finds out 
the best path.

Functions used:

main : It initializes the id of the colors that will later be used and then calls the find_path method.

print_maze: It helps us visualize the possible paths by showing us the grid and helps us visualize every path
that is encountered during find_path function where the queue data structure is used.

find_start: This finds the index of the starting point and then returns it.

find_path: This is the main part of our program which contains the algorithm for finding out the best path usong
queue data structure . Here the print_maze mathod is called everytime when a new path is encountered. 

find_neighbours: This finds out all the possible neighbours in the 4 directions(North,South,East,West) and then
checks if they are present in the maze and then returns the possible neighbours for every position.
