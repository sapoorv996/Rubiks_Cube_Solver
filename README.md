# Rubik's Cube Solver
This project is based on using an algorithm in Python to solve a 3x3 randomized Rubik’s Cube. The algorithm is divided into six separate stages and each stage solves either a face or row of the cube before moving on to the next stage. 

The algorithm was then converted from Python to MATLAB to take advantage of the native Graphical User Interface in MATLAB. In this GUI, the user enters the colors for each piece of the cube and the algorithm solves the cube and gives the user the list of steps to solve the cube for themselves.

## Data Structures and Algorithms
There were several different data structures involved in our algorithm used for the cube in memory, the list of moves to replicate the steps, and a variety for the GUI.

The Rubik’s Cube algorithm is based on using a set of moves that are predefined based on the fact that there are only so many possible moves one can apply to the cube. Therefore, we defined these moves in which the columns or rows of the phases of the cube change. These moves then rearrange the respective contents of the 2D representation of our cube depending on which moves were performed.

We first created a two-dimensional array that stores the whole cube where each entry is the starting character of each color. This two-dimensional array is the foundation of our algorithm because this is the representation of the cube. After each move is applied to the cube while solving, the corresponding move is added to the list of moves in order to give the user the steps we used. Once the algorithm is finished, the entries of the array should contain a solved cube and the list will give the exact steps to solve the cube. In order to represent the cube in MATLAB, we implemented a cell data structure which is a matrix of strings used to color each piece of the cube in our GUI. Finally, each element of the GUI is stored as an object. We can then manipulate each object to store specific entries. For example, there is an object that stores the string of the next move, and we change that string after each move.

## Project Preview
**Rubik's Cube Solver - Input Page**
![enter image description here](https://lh3.googleusercontent.com/_m7-h-VODeAkTMeCK3MH5yrKaHG6aA1XLllVHMrwOzt0U6xYVZRRDBPpV56RnnbyuWW-9my902zoJw)

**Rubik's Cube Solver - Move List**
![enter image description here](https://lh3.googleusercontent.com/Sh8mwSmAKAoOG2slgqNgwSYqy2Hm17tyZzgAY-MWqteQIuPQYFT5R6TCEcsqBZCU4NR7In8eqpIB_g)

**Rubik's Cube Solver - Move Viewer**
![enter image description here](https://lh3.googleusercontent.com/LuPa666Q1MOlYto0Si7ae5HIoFonTkDYSJpEK4xzSfGB8NWq6v_nyZZy-p1OFRXnZ4AlHuHrTcqmTg)

## Built With
[Python3.4](https://docs.python.org/3/)