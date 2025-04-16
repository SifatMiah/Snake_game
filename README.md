# 🐍 Snake Game - Snake Class

This project contains a `Snake` class written in Python using the `turtle` module, which can be used as part of a classic Snake game.

## 🚀 Features

- Initializes a 3-segment snake on screen.
- Handles snake movement in all four directions.
- Prevents reverse movement (i.e., snake can't directly move backward).
- Allows the snake to grow by adding new segments.

## 🧠 How It Works

- The snake is made up of multiple `Turtle` objects (segments).
- The head segment leads the movement, and each segment follows the one in front.
- New segments are added to the tail using the `extend()` method.

## 🧩 Class Overview

### `Snake`

| Method | Description |
|--------|-------------|
| `__init__()` | Initializes the snake and sets the head. |
| `create_snake()` | Builds the initial 3-segment snake. |
| `add_segment(position)` | Adds a new segment to the snake at the specified position. |
| `extend()` | Adds a new segment to the end of the snake (used when eating food). |
| `move()` | Moves the snake forward by making each segment follow the one in front. |
| `up()` | Changes direction to up (unless going down). |
| `down()` | Changes direction to down (unless going up). |
| `left()` | Changes direction to left (unless going right). |
| `right()` | Changes direction to right (unless going left). |

## 🧱 Constants

- `STARTING_POSITIONS`: Coordinates to place the initial snake segments.
- `MOVE_DISTANCE`: How far each movement goes.
- `UP`, `DOWN`, `LEFT`, `RIGHT`: Constants for direction in degrees.


## 🕹 Usage

You can integrate this `Snake` class into a full Snake game by:

1. Creating a game loop to handle movement.
2. Detecting collisions with walls, food, or the snake itself.
3. Growing the snake and updating the score when food is eaten.
