# Learning-Agents-and-Searching-Strategies-in-AI

## Project Description

This project involves the development of an autonomous delivery robot designed to navigate through an urban environment, represented as a grid or graph, to deliver packages to designated locations. The environment includes obstacles such as buildings, houses, and vehicles on roads. The project features path planning using informed search algorithms, dynamic environment handling, real-time path execution and control, a user interface for interaction and visualization, and performance evaluation.

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

- The environment is represented as a 15x15 grid or graph.
- Information about buildings, houses, delivery points, and vehicles on roads is included.
- The robot has a fixed initial start location.
- Matplotlib is used to visualize the city area with obstacles and delivery points.

## Algorithm Implementation

- Informed search algorithms such as Best First Search and A* are implemented for robot motion planning.
- A heuristic function using Euclidean distance is developed, considering the distance to the goal and the presence of obstacles.
- The cost from one location to another is randomly generated between 1 to 20, and the cost from the current location to the goal is calculated by Euclidean distance.
- A comparison between the algorithms is made to choose the best one for the problem.

## Dynamic Environment Handling

- Dynamic changes in the environment are simulated, such as changing the start, goal state, and vehicle positions after delivering an item.
- The robot adapts its path planning in real-time to handle these changes efficiently.

## Path Execution and Control

- A path execution module is developed, allowing the robot to follow the planned path while avoiding collisions.
- Five different delivery locations are generated randomly within the grid.
- The robot starts waiting for delivery, and after each delivery, the previous delivery location becomes the new start point for the next delivery.

## User Interface and Visualization

- A user interface is created to interact with the simulation environment.
- The robot's path, obstacles, and delivery points are visualized in real-time.
- Libraries such as Matplotlib, Pygame, Tkinter, PyQt, or PySide can be used for GUI and animation.

## Performance Evaluation

- The performance of the motion planning algorithm is evaluated in terms of path optimality, execution time, and adaptability to dynamic changes.

## Project Deliverables

- Source code implementing the motion planning algorithm, dynamic environment handling, path execution, and simulation components.
- A user-friendly interface to interact with the environment, visualize the robot's movement, and control the simulation.
- The code can be provided in `.ipynb` or `.py` format.

## Bonus Task: Multi-Robot Coordination

- The project can be extended to handle multiple autonomous robots navigating in the same environment simultaneously.
- Coordination strategies are implemented to prevent collisions and optimize delivery routes.

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

2. Interact with the user interface to assign deliveries and visualize the robot's path.

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch: `git checkout -b my-feature-branch`.
3. Make your changes and commit them: `git commit -m 'Add some feature'`.
4. Push to the branch: `git push origin my-feature-branch`.
5. Submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to customize this README file according to your project's specific requirements and details.
