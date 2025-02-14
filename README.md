# AI Maze: Hunt for Treasures

## Overview

AI Maze: Hunt for Treasures is a Python-based game built with Pygame. The game generates a grid-based maze where the AI-controlled player navigates obstacles, collects gold, and avoids damage while optimizing the best path to gather all treasures. The AI uses the A\* search algorithm for pathfinding and heuristic calculations to determine the shortest route.

## Features

- **Randomly generated grid**: Each game starts with a unique maze containing obstacles, damage zones, gold, and treasures.
- **A**\* Search Algorithm\*\*: The AI utilizes the A\* algorithm to find the optimal path to a target location while avoiding obstacles.
- **Path Optimization**: The AI calculates the best order to collect multiple treasures using permutations, ensuring the shortest overall path.
- **Dynamic Gameplay**: The player loses HP when stepping on damage tiles and gains gold when collecting coins.
- **Interactive Start Menu**: Players can start the game or exit via a simple UI.

## How It Works

1. **Grid Generation**:

   - The grid is initialized with random obstacles (`O`), damage tiles (`D`), gold (`G`), and treasures (`T`).
   - The player starts at the top-left corner `(0,0)`.

2. **Heuristic Function and A**\* Algorithm\*\*:

   - The heuristic function calculates the Manhattan distance between two points, guiding the A\* algorithm.
   - The `a_star_search` function implements pathfinding logic, exploring the shortest path from the player’s position to a specified goal while avoiding obstacles.

3. **Path Optimization**:

   - The `find_best_path` function determines the optimal order to collect treasures by evaluating all possible sequences and selecting the shortest overall route.

4. **Game Execution**:

   - The AI follows the optimal path to collect treasures.
   - If the player's HP drops below 50, the game ends.
   - The game displays a message when all treasures are collected.

## Installation & Execution

### Requirements

Ensure you have Python and Pygame installed. You can install Pygame using:

```bash
ipip install pygame
```

### Running the Game

Execute the script by running:

```bash
python ai_maze.py
```

## Contributors

- I developed the "Path Optimization" logic, specifically the `find_best_path` function, optimizing the AI agent's movement for treasure collection. 

## License

This project is open-source and available for personal and educational use.

