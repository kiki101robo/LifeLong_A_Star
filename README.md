# Lifelong A* Pathfinding Project
This project implements the Lifelong A* (LPA*) algorithm, an incremental pathfinding method used in dynamic environments where obstacles can appear or disappear, and a path needs to be efficiently recalculated. It includes Python scripts to handle the environment setup, path planning, and visualization.

File Descriptions
main.py: Contains the Lifelong_A_Star class that implements the LPA* algorithm. It initializes with start and goal positions, chooses a heuristic (Euclidean or Manhattan), and handles dynamic obstacle updates.
env.py: Defines the Env class that models the grid environment, including obstacles, grid dimensions, and allowed movements.
plotting.py: Contains the Plotting class responsible for visualizing the environment, the visited nodes, and the final path using matplotlib.
Setup and Requirements
Python Version:

Ensure Python 3.6 or higher is installed.
Dependencies:

Requires matplotlib for plotting. Install using pip:
bash
Copy
pip install matplotlib
Usage
Running the Lifelong A Algorithm*:

Set the start and goal positions directly in the main.py.
Specify the heuristic type (Euclidean or Manhattan) in the Lifelong_A_Star class instantiation.
Run the script to see the algorithm in action, with interactive obstacle addition and removal:
bash
Copy
python main.py
Dynamic Obstacle Update:

Click on the plot area to add or remove obstacles during the algorithm's execution.
The path and visualization will update in real time based on the new environment configuration.
Visualization Adjustments:

Modify the visualization settings in plotting.py, such as colors, pause durations, and other matplotlib settings, to customize the display.
