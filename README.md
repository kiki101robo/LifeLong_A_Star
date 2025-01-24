# Lifelong A* Algorithm Implementation

## Files Overview

### `Lifelong_A_Star.py`
- **Purpose**: Implements the Lifelong A* (LPA*) pathfinding algorithm with dynamic obstacle handling in a grid environment.
- **Key Functions**:
  - `__init__(self, s_start, s_goal, heuristic_type)`: Initialize the algorithm with start and goal points, heuristic type, and environment settings.
  - `run()`: Manages the visualization and user interaction loop.
  - `on_press(event)`: Handles mouse click events to modify obstacles and re-compute paths.
  - `ComputeShortestPath()`: Executes the core LPA* algorithm logic to determine the shortest path.
  - `UpdateVertex(s)`: Updates the priority queue based on heuristic and path cost changes.
  - `plot_path(path)`: Displays the path from start to goal on the grid.
  - `plot_visited(visited)`: Shows all nodes visited during the path computation.

### `env.py`
- **Purpose**: Defines the grid environment for the pathfinding algorithm including obstacles, boundaries, and motion possibilities.
- **Data Structures**:
  - `obs`: A set containing tuples of obstacle coordinates.
  - `motion`: A list defining possible movements from each cell.

### `plotting.py`
- **Purpose**: Handles graphical representation of the pathfinding process on a grid layout.
- **Functions**:
  - `plot_grid(name)`: Draws the grid and labels it.
  - `plot_path(path)`: Visualizes the computed path on the grid.
  - `update_obs(obs)`: Refreshes the grid with new or removed obstacles.

## Setup and Execution
- **Requirements**: Python 3.x, `matplotlib`, `numpy`
- **Run Command**:

Lifelong_A_Star.py
Launch the script to view the grid environment. Click on the grid to add or remove obstacles and observe real-time path re-computation.

## Features
- **Interactive Pathfinding**: Adjust the grid dynamically by adding or removing obstacles and watch the algorithm respond in real time.
- **Visualization**: Provides clear visualization of the pathfinding process, including start and goal points, obstacles, and the computed path.

## Additional Notes
- This implementation is tailored for educational and demonstration purposes, illustrating dynamic pathfinding in a controlled setting.
- System performance may vary based on grid complexity and the placement and number of obstacles.
