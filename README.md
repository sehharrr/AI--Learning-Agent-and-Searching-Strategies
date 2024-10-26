# AI--Leraning-Agent-and-Searching-Strategies

## Project Description

This project focuses on developing an autonomous delivery robot designed to navigate an urban environment modeled as a grid or graph to deliver packages to specific locations. The environment includes obstacles such as buildings, houses, and vehicles on roads. Key features include path planning with informed search algorithms, dynamic environment handling, real-time path execution and control, an interactive user interface for visualization, and performance evaluation.

## Table of Contents
- [Environment Representation](#environment-representation)
- [Algorithm Implementation](#algorithm-implementation)
- [Dynamic Environment Handling](#dynamic-environment-handling)
- [Path Execution and Control](#path-execution-and-control)
- [User Interface and Visualization](#user-interface-and-visualization)
- [Performance Evaluation](#performance-evaluation)
- [Project Deliverables](#project-deliverables)
- [Bonus Task: Multi-Robot Coordination](#bonus-task-multi-robot-coordination)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Environment Representation

- The environment is modeled as a 15x15 grid or graph.
- It includes information about buildings, houses, delivery points, and vehicles on roads.
- The robot has a fixed initial start location.
- The **Matplotlib** library is used for visualizing the city, including obstacles and delivery points.

## Algorithm Implementation

- Informed search algorithms like **Best First Search** and **A\*** are used for motion planning.
- A heuristic based on Euclidean distance is developed to account for the distance to the goal and nearby obstacles.
- Movement costs between locations are randomly assigned between 1 and 20. The cost to the goal is calculated using Euclidean distance.
- A comparison of search algorithms is conducted to determine the most suitable one for this problem.

## Dynamic Environment Handling

- The environment can change dynamically, such as altering the start, goal states, or vehicle positions after a delivery is made.
- The robot adjusts its path planning in real time to accommodate these changes efficiently.

## Path Execution and Control

- A path execution module ensures the robot follows the planned path while avoiding collisions.
- Five random delivery locations are generated within the grid.
- The robot waits for a delivery, and after completing each one, the previous delivery point becomes the new start location for the next task.

## User Interface and Visualization

- A user interface enables interaction with the simulation environment.
- The robot’s path, obstacles, and delivery points are displayed in real time.
- Libraries such as **Matplotlib**, **Pygame**, **Tkinter**, **PyQt**, or **PySide** can be used for the graphical interface and animation.

## Performance Evaluation

- The performance of the motion planning algorithm is evaluated based on path optimality, execution time, and adaptability to dynamic changes.

## Project Deliverables

- Source code implementing the motion planning algorithm, dynamic environment handling, path execution, and simulation components.
- A user-friendly interface for interacting with the environment, visualizing the robot's movement, and controlling the simulation.
- The code can be provided in either **.ipynb** (Jupyter notebook) or **.py** (Python script) format.

## Bonus Task: Multi-Robot Coordination

- The project can be extended to handle multiple autonomous robots operating in the same environment.
- Coordination strategies are implemented to avoid collisions and optimize delivery routes for all robots.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/autonomous-delivery-robot.git
   cd autonomous-delivery-robot
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Run the main script:
   ```bash
   python main.py
   ```

2. Use the user interface to assign deliveries and visualize the robot's path in real time.

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b my-feature-branch
   ```
3. Make your changes and commit them:
   ```bash
   git commit -m 'Add a new feature'
   ```
4. Push to the branch:
   ```bash
   git push origin my-feature-branch
   ```
