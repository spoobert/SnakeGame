SNAKE by Daniel Thompson
CS-315 Lab5

Everything works as intended.
There is one quirk to the gameboard, however: If you make the game board the minimum size possible,
there isn't enough room to print the title and the score, so there's some overlapping.

Code is thoroughly commented.
To move, you can use the VIM hjkl movement, or standard WASD movement(this is done simply using an 'or' statement)

The "main" is recycled from the original main file, which was named "screep.cpp".
This is because the original code was used partially for testing, and the startup && teminate functions were left as is.
Also: getChar was ONLY altered to make the snake move slightly faster initially.



****Only other issue is the destructor. The MATRIX and FREEPOOL are successfully deleted.
	 I BELIEVE the snake is being deleting correctly, however I am unsure. Snake is used as a pointer in the gameboard,
	 and is only ever newed up IN matrix. But if I add a delete for snake in the TdArray class, it segfaults, so
	 a delete is attempted after gameover by doing "delete matrix->snake".**** 




After compiling, type "make run" to run.
