# Tic-Tac-Toe Game with AI

Welcome to the Tic-Tac-Toe game! This Python project allows you to play the classic Tic-Tac-Toe game either with an AI or with a friend. The AI opponent uses previous game data to predict the best move, making the game more interactive and engaging. You can also save game data to track outcomes.

## Features
- **Two Game Modes**:
  - **Play against AI**: Play as either "X" or "O" against a simple AI that learns from past games.
  - **Two-player mode**: Play with a friend, alternating turns to make moves.
  
- **Game Data Tracking**:
  - Save game outcomes (win, loss, tie) to a JSON file for later analysis.
  - AI uses past data to improve its move choices.

- **Board Display**:
  - A dynamic board is displayed after every move, updating the status in real-time.

## Requirements
- Python 3.x
- No additional libraries required, just standard Python modules.

## How to Play
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/Lord-Rahul/machine-learning.git
   ```
   Choose your game mode:

1: Play against AI.
2: Play with a friend.
Select your symbol:

Choose "X" or "O" to start playing.
Make your move by entering a number between 1 and 9 to place your mark on the board.

The game continues until there's a winner or a tie.

After the game ends, the board will display the result and the game data will be saved for future use.

AI Functionality
The AI opponent makes its moves based on past game data stored in game_data.json. The AI attempts to predict the most successful move based on previous outcomes. If there are no available game data, the AI selects a random available move.

How the AI Works:
The AI uses game data from a JSON file (game_data.json) to determine the success rate of each move.
It selects moves that have led to wins in past games, improving over time with more game data.
The AI is not perfect, but it learns from each game.
Save and Load Game Data
After each game, the board and outcome (win/loss/tie) are saved in game_data.json.
If a new game is played, the AI can use this data to make decisions.
Example Board
Here’s an example of how the board looks:
```
1 | 2 | 3
---------
4 | 5 | 6
---------
7 | 8 | 9
```
Each number corresponds to a spot on the board, where players can make their moves by choosing a number.
