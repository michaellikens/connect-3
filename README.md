# 🧠 ML Connect 3

A **machine learning–powered Connect 3 game** built with **Python** and **Pygame**.  
This project combines classic gameplay with **reinforcement learning**, allowing AI agents to train, improve, and compete over time.
![image1](https://i.imgur.com/lWWvQ9L.png)


## 🚀 Overview

ML Connect 3 is both a playable game and an experimentation platform for AI training.  
Users can play manually, compete against trained models, or observe AI agents learning strategies through repeated simulations.



## ✨ Features

- 🎮 Fully functional **Connect 3 game engine** (configurable via `constants.py`)
- 🤖 **Reinforcement Learning AI agents**
- 🔁 Multiple gameplay and training modes
- ⚡ **Headless training** for high-speed simulations
- 👀 **Visual training mode** to see AI learning in real time
- 🧑‍💻 Human vs AI gameplay using saved policies
- 🖥️ Clean and interactive UI built with **Pygame**



## 🎯 Game Modes

### 👥 Human vs Human
Two players take turns placing pieces on the board.

### 🤖 Human vs AI
Play against a trained AI model using a saved policy. (configure policy in `constants.py`)

### 👁️ AI Training (Visual)
Watch two AI agents train against each other with real-time rendering.

### ⚡ Headless AI Training
Train AI agents without rendering graphics, enabling thousands of games to run quickly.  
> This is the **fastest and most efficient training mode**.

## 📸 Screenshots
![image2](https://i.imgur.com/o8LMzBN.png)
![image3](https://i.imgur.com/8F3bAcq.png)

## 📦 Requirements

- Python **3.10+**
- Pygame

### Install Dependencies

```bash
pip install pygame numpy pathlib
```

### ▶️ Running the Game
```bash
python -m src.main
```
This launches the main menu where you can then select a game mode.

### 🧠 Training the AI

Training begins automatically when selecting:

- AI Training (Visual)
- Headless AI Training

The number of training episodes is defined in:

**`constants.EPISODES`**

After training completes:

- The AI's learned policy is saved

- The policy can be reused in Human vs AI mode
## 🎮 Controls

**Mouse only:**

- Click on board cells to place pieces
- Use buttons to navigate menus
- Reset button appears after a game ends
- Back button returns to the main menu
## 🛠️ Technologies Used
- Python
- Pygame
- NumPy
- Reinforcement Learning
## 📁 Project Structure
```text
CONNECT3/
├── assets/
│ ├── images/
│ │ └── icon.png
│
├── policies/
│ ├── policy_player1_date-time.pkl
│ └── policy_player2_date-time.pkl
│
├── src/
│ ├── ai_player.py
│ ├── board.py
│ ├── constants.py
│ ├── game_manager.py
│ ├── human_player.py
│ ├── main.py
│ ├── player_base.py
│ └── utilities.py
```
## 👨‍💻 Authors
**Michael L.**

**Elijah F.**

## 📌 Notes

This project is designed to be **extendable**:

- Modify board size or rules via `constants.py`
- Experiment with different RL strategies
- Improve AI performance through hyperparameter tuning

## ⭐ Future Improvements
- Save/load multiple AI models
- Add difficulty levels
- Implement Minimax or hybrid AI strategies
- Enhance UI/UX and animations
