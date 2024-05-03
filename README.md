# Readme
# RRT Algorithms Simulation Project

## Overview
This project tests multiple Rapidly-exploring Random Trees (RRT) algorithms. It only produces output when all paths find a result. If the simulation does not find a solution within 15-30 seconds, please end the simulation and try again. I acknowledge this as a limitation and apologize for the inconvenience.

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
The robot currently follows the path determined by the Post-RRT Modification. You can switch to another algorithm by changing the `Ppath` variable in the code to any of the paths created by the different algorithms. The are labeled clearly within the code where `Ppath` is currently Post-RRT Modification, `path` is the Origianl RRT path, `pathCoin` is the Coin Flip RRT, and `astar_path` is the A* path.

## Output
- The program outputs the nodes along each path and a table of path distances, measuring the Euclidean distance between each node in a path.
- Paths are visualized on the map in accoradance to the Algorithms Display section, and a green path shows the trajectory from node to node for deeper analysis.

## Issues and Contributions
This project has ongoing development needs, particularly in handling cases where not all paths find a result given RRT limitations. If you encounter issues or have suggestions, please feel free to discuss. The current plan is to create a goal 'zone' as opposed to a goal node, where once any branch reaches the zone, a straigh line is made to the true goal node.

## Contact
For any questions or further assistance, please contact me at bhaight@uncc.edu

