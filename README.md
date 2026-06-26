# 🎮 Tic-Tac-Toe AI

An unbeatable Tic-Tac-Toe AI built in **Python** using the **Minimax Algorithm** as part of **Harvard CS50's Introduction to Artificial Intelligence with Python**.

The AI analyzes every possible future game state before making a move, ensuring it always chooses the optimal action. As a result, it can never lose when playing against a human.

---

## 🚀 Features

- Unbeatable AI opponent
- Minimax Algorithm implementation
- Recursive game tree search
- Optimal move selection
- Pygame graphical interface
- Clean and modular Python code

---

## 🛠️ Technologies Used

- Python 3
- Pygame
- Minimax Algorithm
- Recursion
- Game Tree Search

---

## 📁 Project Structure

```
tic-tac-toe/
│
├── runner.py          # Game interface (Pygame)
├── tictactoe.py       # Game logic and AI
├── requirements.txt
└── README.md
```

---

## 🧠 How the AI Works

The AI uses the **Minimax Algorithm**, a classic adversarial search algorithm used in game-playing artificial intelligence.

The algorithm works as follows:

1. Generate all possible legal moves.
2. Simulate every possible future game.
3. Continue recursively until reaching a terminal state.
4. Evaluate terminal states using a utility function:
   - **+1** → X wins
   - **0** → Draw
   - **-1** → O wins
5. Propagate these values back through the game tree.
6. Choose the move that guarantees the best possible outcome.

Since Tic-Tac-Toe has a relatively small search space, the AI explores every possible game before making a decision, making it impossible to defeat.

---

## 📚 Functions Implemented

### `player(board)`
Determines which player's turn it is.

### `actions(board)`
Returns all legal moves available on the current board.

### `result(board, action)`
Returns a new board after applying a move without modifying the original board.

### `winner(board)`
Checks whether X or O has won the game.

### `terminal(board)`
Determines whether the game has ended.

### `utility(board)`
Returns the utility value of a terminal board.

### `minimax(board)`
Returns the optimal move using the Minimax algorithm.

---

## ▶️ Installation

Clone the repository:

```bash
git clone https://github.com/OsamaSobhy2006/tic-tac-toe.git
```

Navigate into the project:

```bash
cd tic-tac-toe
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the game:

```bash
python runner.py
```