# Humble Chess Bot

Welcome to Humble Chess Bot, a friendly chess opponent built using Python, NumPy, Matplotlib and Google Colab.

You play as **White** against the Beginner Tutorial Bot, which plays as Black. The chessboard is displayed using Matplotlib, while moves are entered through a Google Colab form.

## How to play

### Step 1: Set up the game (run once)

Open this notebook in Google Colab and connect to a runtime.

Run the following code cells **once, in order**, starting from the top:

1. **Install the libraries** (Cell 3): Installs the required Python packages and chess engine.
2. **Initialize the board** (Cell 5): Creates a new chess game and resets the move history.
3. **Board visualization** (Cell 6): Loads the chessboard drawing function and displays the starting position.
4. **Chess engine imports** (Cell 8): Imports the engine-related libraries.
5. **Beginner Bot configuration** (Cell 9): Starts the computer opponent and configures its difficulty.

Once these cells have executed successfully, you're ready to play!

### Step 2: Play chess (repeat every turn)

Find the cell titled **Chess Move Controller** (Cell 11).

This is your main input interface.

1. Enter your move into the `move_text` form field.
2. Press the **Run** button beside the cell.
3. The computer will calculate its response.
4. The updated chessboard will appear below the cell.
5. Enter your next move and run the same cell again.

You can enter moves in standard chess notation, including:

- `e4` to advance the king's pawn.
- `Nf3` to move a knight.
- `e2e4` to specify the starting and destination squares.
- `O-O` to castle kingside when legal.

The program checks whether your move is legal before accepting it.

**Important:** During a game, keep using the Chess Move Controller. Running the board initialization cell again resets your game and erases the current move history.

### Step 3: Finish the game and export your PGN

When the game ends in checkmate, stalemate or another recognized conclusion, the controller displays **Game over!** and the final result.

To save your game history:

1. Scroll down to the **PGN Export** section.
2. Run the PGN imports cell (Cell 13).
3. Run the PGN Exporter cell (Cell 14).
4. Your complete game history will appear in Portable Game Notation (PGN).
5. The program will save a `.pgn` file to Colab's `/content` directory.

To download your PGN, open the **Files** panel on the left side of Colab, locate the generated `chess_game_...pgn` file, and select Download.

The PGN records the sequence of moves, players, date and final result. You can import it into a chess analysis website such as [Lichess](https://lichess.org/paste).

### Step 4: Play again

To begin a new game, rerun the **Initialize the board** cells (Cells 5 and 6). This clears the old chess position and move history.

You can continue using the existing Stockfish engine and Chess Move Controller.

**Remember to download your PGN before starting a new game.** Colab's runtime memory and temporary files can disappear when the runtime disconnects or resets.

---

*Humble Chess Bot wishes you an enjoyable learning experience. Difficulty: Beginner Tutorial Bot :)*
