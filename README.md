
# Snake Game 🐍

Welcome to the **Snake Game** — a fun, fast-paced, and nostalgic game where you control a snake that must navigate the screen, eat food to grow longer, and avoid hitting walls or itself. This version is created using Python and the Turtle graphics library, designed to challenge your reflexes and strategic thinking.

---

## Features

- **Classic Gameplay**: Navigate the snake using the arrow keys. Eat food to grow longer while avoiding collisions with walls and the snake’s own body.
- **Score Tracking**: Track your current score and high score. Every time you beat your high score, it is saved for the next session.
- **Dynamic Food**: The food (represented by a green turtle) spawns randomly within the screen, and each time the snake eats it, it grows longer.
- **Responsive Controls**: Use the arrow keys to move the snake in all directions (up, down, left, right).
- **Game Reset**: On collision with walls or the snake’s body, the game resets and your score is brought back to zero.
- **Smooth Animations**: The game uses smooth animations and real-time updates for an immersive experience.

---

## How to Play

### Gameplay:
- **Move the Snake**: Use the arrow keys to control the snake’s direction. Avoid running into walls or the snake’s body!
- **Eat the Food**: Each time the snake eats the food, it grows longer and the score increases.
- **Avoid Collisions**: If the snake hits a wall or its own tail, the game ends, and the score resets to 0.
  
### Controls:
- **Up**: Press the "Up" arrow to make the snake move upwards.
- **Down**: Press the "Down" arrow to make the snake move downwards.
- **Left**: Press the "Left" arrow to move the snake to the left.
- **Right**: Press the "Right" arrow to move the snake to the right.

### Scoring:
- **Score**: You score 1 point each time the snake eats the food.
- **High Score**: The game tracks your highest score across sessions. It is saved in a `data.txt` file.

---

## Setup and Installation

### Requirements:
- Python 
- Turtle graphics library (usually pre-installed with Python)

### Running the Game:
1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/Sanjula2005/Snake_Game.git
   cd Snake_Game
   ```

2. Run the game using the following command:
   ```bash
   python main.py
   ```

Once the game starts, control the snake using the arrow keys and enjoy!

---

## Code Structure

This project is divided into multiple files, each handling a specific functionality.

### `main.py`:
- The main script that handles game logic, screen setup, user inputs, snake movement, food generation, and score tracking.

### `snake.py`:
- Contains the `Snake` class that defines the behavior of the snake (movement, growth, and direction changes).

### `food.py`:
- Contains the `Food` class responsible for generating food at random locations on the screen.

### `scoreboard.py`:
- Contains the `Scoreboard` class that tracks and displays the current score and high score.

---

## Gameplay Walkthrough

- **Starting the Game**: Upon launching, the game opens a window with a black background and a white snake moving around. The snake is initially short, and the goal is to eat the green food that appears randomly on the screen.
  
- **Snake Movement**: You can control the snake's movement using the arrow keys. The snake will move in the direction of the arrow key you press (up, down, left, or right).

- **Eating the Food**: Every time the snake eats the food, its body grows longer, and your score increases by 1 point. The food then spawns at a new random location.

- **Collisions**:
  - **Wall Collision**: If the snake hits any of the walls, the game resets, and your score goes back to 0.
  - **Self Collision**: If the snake collides with any part of its body, the game resets, and the score is reset to 0.

- **Game Over**: When the game ends due to a collision, the current score resets, and the game starts from the beginning. If you achieved a new high score, it is saved.

---
