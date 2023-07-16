# Minesweeper AI

This project implements an AI player for the game of Minesweeper. The AI uses logical deduction and inference to make educated moves and avoid mines.

## Requirements

- Python 3.x
- Pygame library

## Usage

1. Run the `runner.py` file to start the Minesweeper game.
2. The game window will display the Minesweeper board.
3. Left-click on a cell to reveal it.
4. Right-click on a cell to mark it as a mine.
5. The AI Move button allows the AI player to make a move.
6. The Reset button resets the game.
7. The game ends when all mines have been correctly flagged or a mine is revealed.

## AI Algorithm

The AI player uses a knowledge-based approach to make moves. It maintains a knowledge base consisting of logical statements (sentences) about the game state. The AI updates its knowledge base based on the cells it has explored and the counts of neighboring mines.

The AI follows the following steps for each move:

1. Mark the chosen cell as a move that has been made.
2. Mark the chosen cell as safe.
3. Add a new sentence to the knowledge base based on the chosen cell and its count.
4. Mark any additional cells as safe or mines if it can be concluded based on the current knowledge.
5. Add any new sentences to the knowledge base if they can be inferred from existing knowledge.

The AI player uses this knowledge to make safe moves or flag mines. If no safe moves are available, it makes a random move.

## Files

- `minesweeper.py`: Contains the implementation of the Minesweeper game and the AI player.
- `runner.py`: Runs the Minesweeper game using the Pygame library.

## Acknowledgments

This project is based on the CS50 AI course from Harvard University.

Note: The code provided is a simplified version and may require additional modifications and error handling for a complete and robust implementation.
