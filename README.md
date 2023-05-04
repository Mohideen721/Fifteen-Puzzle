Fifteen Puzzle Game
This program is a browser-based implementation of the Fifteen Puzzle game. The game is played by clicking and dragging the puzzle pieces around to arrange them in numerical order from 1 to 15. The puzzle pieces can only be moved if they are adjacent to the empty space on the board.

Features
In addition to the basic functionality of the game, this implementation includes the following features:

Puzzle piece highlighting: When the mouse hovers over a puzzle piece, it will be highlighted in red if it can be moved to the empty space.
Puzzle background image: The puzzle background is set to an image of colorful geometric shapes.
Shuffle button: The game can be reset to a random initial state by clicking the "Shuffle" button.
End-of-game notification: When the player completes the puzzle, a notification will appear on the screen informing them that they have won the game.
Code
The JavaScript code is organized as follows:

Global variables
The following variables are declared globally:

gamePiece: An array containing the puzzle pieces as DOM elements.
notify: A counter for the end-of-game notification.
timer: A timer for the end-of-game notification.
spaceY: The y-coordinate of the empty space on the board.
spaceX: The x-coordinate of the empty space on the board.
window.onload function
The window.onload function initializes the game board and sets up event listeners for the puzzle pieces and shuffle button.

Puzzle piece event listeners
The event listeners for the puzzle pieces are defined as follows:

onmouseover: When the mouse moves over a puzzle piece, it checks if the piece can be moved to the empty space and highlights the piece accordingly.
onmouseout: When the mouse moves off a puzzle piece, it reverts the highlighting to the default state.
onclick: When a puzzle piece is clicked, it checks if it can be moved to the empty space, and if so, moves it and checks if the puzzle is complete.
checkMove function
The checkMove function checks if a puzzle piece can be moved to the empty space.

Shuffle button event listener
The event listener for the shuffle button shuffles the puzzle pieces by randomly selecting a direction to move a random puzzle piece.

up, down, left, and right helper functions
These functions check if a puzzle piece can be moved in the corresponding direction from its current position.

swap function
The swap function swaps the position of a puzzle piece with the empty space.

finish function
The finish function checks if the puzzle is complete by comparing the current position of each puzzle piece with its correct position.

win function
The win function displays the end-of-game notification and starts the timer. The Notify function is called every second to update the notification and decrement the counter.




