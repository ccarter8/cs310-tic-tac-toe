# cs310-tic-tac-toe
For this project, I implemented a working two-player Tic-Tac-Toe game.
Two versions of this project were to be completeed. One tat runs in the command line, and one that has a fully integrated GUI.
We were provided with a robot framework for testing and confirming our results.
In the JPanel, the squares of the board are implemented as a two-dimensional array of JButton objects with a preferred size of 
64 x 64 pixels, and whose names are set to "SquareXY" (replacing X with the row and Y with the column).  
In addition, to display the winning player at the end of the game, a JLabel named "ResultLabel" is added to the bottom of the window.  
The reason these names are so important is that, during the acceptance tests, the Robot Framework will open the window, 
register "clicks" with the button elements, and check the results shown in the labels directly.
When the players click on the buttons, the Controller (as the event handler) should add the marks to the Model using its makeMark() method.  
The Controller should then invoke the View's updateButtons() method, which will update the View to reflect the new contents of the 
game board, using "X" or "O" to indicate the players' marks.
That is how the GUI is implemented.
