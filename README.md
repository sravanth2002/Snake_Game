# Snake Game using Tkinter

This is a simple Snake game implemented in Python using Tkinter for the GUI.

## Game Details

- **Game Dimensions:**
  - Width: 1000 pixels
  - Height: 700 pixels

- **Speed:** 
  - Snake movement speed: 80 milliseconds per move

- **Game Elements:**
  - **Space Size:** Each segment of the snake and the food occupies a 25x25 pixel space
  - **Snake Color:** Green (`#00FF00`)
  - **Food Color:** Red (`#FF0000`)
  - **Background Color:** Black (`#000000`)

## Classes

### Snake Class

- **Attributes:**
  - `body_size`: Number of segments in the snake
  - `coordinates`: List of coordinates representing the snake's body
  - `squares`: List of Tkinter rectangles representing each segment of the snake

- **Methods:**
  - `__init__()`: Initializes the snake with initial coordinates and creates the snake's segments on the canvas

### Food Class

- **Attributes:**
  - `coordinates`: List representing the coordinates of the food on the canvas

- **Methods:**
  - `__init__()`: Initializes the food at a random position on the canvas

## Functions

- **`next_turn(snake, food)`**: Moves the snake to the next position, checks for collisions with the food or walls, updates the score, and schedules the next move
- **`change_direction(new_direction)`**: Changes the direction of the snake's movement based on user input
- **`check_collisions(snake)`**: Checks for collisions with the walls or the snake's own body
- **`game_over()`**: Displays "GAME OVER" text on the canvas when the game ends

## Setup and Usage

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/snake-game.git
   cd snake-game
