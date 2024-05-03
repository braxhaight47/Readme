# Readme
# RRT Algorithms Simulation Project

## Overview
This project tests multiple Rapidly-exploring Random Trees (RRT) algorithms. It only produces output when all paths find a result. If the simulation does not find a solution within 15-30 seconds, please end the simulation and try again. We acknowledge this as a limitation and apologize for the inconvenience.

## Running the Simulation
### Initial Setup
- The simulation floor is divided into two zones for placing the start and goal nodes.
  - **Goal Node**: Place in the row in the positive y-direction immediately following the last obstacle.
  - **Start Node**: Place in the row in the negative y-direction opposite to the goal node.
- Grey boxes represent randomly generated obstacles, located between the starting and goal node zones.

### Algorithms Display
- **Purple**: Original RRT
- **Navy**: Post-RRT Modification
- **Teal**: Coin Flip RRT
- **Red**: A* Search

### Robot Path
The robot currently follows the path determined by the Post-RRT Modification. You can switch to another algorithm by changing the `Ppath` variable in the code to any of the paths created by the different algorithms.

## Output
- The program outputs the nodes along each path and a table of path distances, measuring the Euclidean distance between each node in a path.
- Paths are visualized on the map, and a green path shows the trajectory from node to node for deeper analysis.

## Issues and Contributions
This project has ongoing development needs, particularly in handling cases where not all paths find a result. If you encounter issues or have suggestions, please feel free to reach out.

## Contact
For any questions or further assistance, please contact us through this platform.

