# ML Connect 3

A **machine learning powered Connect 3 game** built with **Python and Pygame**.  
This project allows humans to play Connect 3 while also enabling **AI agents to train against each other using reinforcement learning**.

The AI can learn strategies through repeated episodes and store its learned policy for later use.

---

## Features

- Connect 3 board game implementation (With expandability defined in constants.py)
- Reinforcement Learning AI players
- Multiple gameplay modes
- Headless AI training for fast learning
- Visual AI training to watch learning in real time
- Human vs AI gameplay using a trained policy
- Clean UI built with **Pygame**

---

## Game Modes

### Human vs Human
Two players take turns placing pieces on the board.

### Human vs AI
Play against a trained AI model that uses a saved policy.

### AI Training (Visual)
Two AI agents train against each other while the game is rendered on screen.

### Headless AI Training
Two AI agents train **without rendering graphics**, allowing thousands of games to run quickly.  
This is the **fastest training mode**.

---

## Requirements

- Python 3.10+
- Pygame

Install dependencies:

```bash
pip install pygame
```

### Running the Game

Run the main script:
```bash
python -m src.main
```

This will open the game menu where you can choose a mode.
---

### Training the AI

Training occurs automatically when selecting:

AI Training Visual

AI Headless Training

The AI plays multiple episodes defined in:

`constants.EPISODES`

After training finishes, the learned policy is saved and can be loaded for Human vs AI matches.

### Controls

Mouse only:

Click board cells to place pieces

Click buttons to navigate menus

Reset button appears after a game ends

Back button returns to the menu
---

### Technologies Used

Python

Pygame

Numpy

Reinforcement Learning
--- 
### Authors

Michael L.
Elijah F.
