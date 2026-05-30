# Genetic Algorithm Route Optimizer

A Python visualization project that uses a genetic algorithm to find a short route between multiple planets. The project is inspired by the Traveling Salesman Problem and includes an animated Pygame interface.

## Overview

The user can place planets on the screen using mouse clicks. After pressing Enter, the genetic algorithm starts generating and improving possible routes between the planets. The best route found is displayed visually, and every 100 generations the rocket animation follows the current best path.

## Features

- Interactive planet placement
- Genetic algorithm for route optimization
- Route visualization using Pygame
- Animated rocket movement
- Random route generation
- Crossover and mutation operations
- Continuous improvement over generations

## Technologies Used

- Python
- NumPy
- Pygame

## Project Structure

```text
.
├── environment.py
├── train.py
├── rocket.png
├── space.jpg
├── README.md
└── requirements.txt
```

## How It Works

The project uses a population of possible routes. Each route represents an order in which the rocket visits the planets.

For each generation:

1. Each route is evaluated based on the total distance traveled.
2. The best routes are selected.
3. New routes are created using crossover and mutation.
4. The shortest route is displayed on the screen.
5. Every 100 generations, the rocket animates along the best route.

## Running the Project

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the project:

```bash
python train.py
```

## Controls

- Left mouse click: add a planet
- Enter: start the genetic algorithm
- Close window: exit the program

## Notes

The project requires the following image assets to be present in the same folder:

- `rocket.png`
- `space.jpg`

## Author

Vlad Soporan
