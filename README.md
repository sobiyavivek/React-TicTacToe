1. Square Component (Square)

A simple button that represents each cell in the Tic-Tac-Toe board.
Receives value (either 'X', 'O', or null) and onSquareClick (function to handle clicks).
Renders the value inside a button.

2. Board Component (Board)

Manages the game logic for the Tic-Tac-Toe board.

Handles clicks:

If the clicked square is already filled or there's a winner, it prevents further actions.
Otherwise, updates the board with 'X' or 'O' based on xIsNext.

Determines the game status:

Calls calculateWinner(squares) to check if a player has won.
Displays "Next player: X/O" or "Winner: X/O".

Renders the board:

Uses three rows, each containing three Square components.

3. Game Component (Game)

Manages the game history and state.

Tracks game moves:

Uses useState to store a history of board states.
currentMove keeps track of the move number.

Handles game actions:

handlePlay(nextSquares): Updates the history and moves to the next state.

jumpTo(nextMove): Allows players to go back to a previous move.

Displays the game history:

Renders a list of buttons that let players jump to past moves.

4. Winner Calculation (calculateWinner)
   
Checks all possible winning combinations.
If three matching symbols ('X' or 'O') align in a row, column, or diagonal, it returns the winner.
Otherwise, it returns null, meaning the game is still ongoing.

5. Additional Features
   
Move History: Players can jump back to a previous game state.

Turn Indicator: Displays which player's turn it is.

Game Over Detection: Stops play when there's a winner.

To run the code :

Open the program using vs code.

Install Node Package Manager.

Run using 'npm start' command from terminal.




