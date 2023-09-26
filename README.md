
[![Pathfinding-visualizer](./public/styling/logo.png)](https://pathfinding-visualizer-9474.web.app)
# Pathfinding Visualizer

Fascinated with DS and various pathfinding algorithms pertaining to graphs?!!

Well, welcome to the Pathfinding Visualizer! This application was created out of my fascination with various pathfinding algorithms and the desire to provide a dynamic visualization of their functionality. I hope you find as much enjoyment in exploring and interacting with this visualization tool as I did when developing it. To experience it firsthand, please access the Pathfinding Visualizer [here](https://pathfinding-visualizer-9474.web.app) (we recommend using Google Chrome for the best experience):

This web application provides a visual representation of various pathfinding algorithms, allowing users to observe how different algorithms work and understand their efficiency. The following algorithms are visualized in this application:

- Dijkstra's Algorithm (weighted): The pioneer of pathfinding algorithms, ensuring the shortest path.

- A Search* (weighted): Arguably the premier pathfinding algorithm, employing heuristics for significantly faster pathfinding compared to Dijkstra's Algorithm while still guaranteeing the shortest path.

- Greedy Best-first Search (weighted): A swifter, heuristic-centric variation of A*; it prioritizes speed over guaranteed shortest paths.

- Swarm Algorithm (weighted): Combining traits of both Dijkstra's Algorithm and A*, it offers versatility but doesn't guarantee the shortest path.

- Convergent Swarm Algorithm (weighted): A more agile and heuristic-driven iteration of the Swarm Algorithm, favoring speed over path length guarantees.

- Bidirectional Swarm Algorithm (weighted): Applying the Swarm approach from both directions, it seeks efficiency but doesn't promise the shortest path.

- Breath-first Search (unweighted): A commendable algorithm that ensures the shortest path when weights are absent.

- Depth-first Search (unweighted): An unsuitable choice for pathfinding, as it doesn't guarantee the shortest path and is generally ineffective.

More on the non-trivial Swarm Algorithm and its variations:
#### Swarm search:
The Swarm Algorithm can be thought of as a fusion of Dijkstra's Algorithm and A* Search. Specifically, while it strives to reach the target node akin to A*, it also explores a considerable number of adjacent nodes around the starting point, akin to Dijkstra's approach.

What sets this algorithm apart from A* is its utilization of heuristics. It constantly updates the distance of nodes from the starting point while considering their estimated distance from the target node. This dynamic approach effectively balances the total distance disparity between nodes near the starting point and those closer to the target node. As a result, the Swarm Algorithm exhibits a distinctive triangular pattern.

 This approach finds applications in various domains, including robotics, optimization, and data mining. Swarm search encompasses diverse algorithm types, such as bi-directional swarm search and convergent swarm search.
#### Bi-directional swarm search: 
It is a variant of swarm search that involves two distinct sub-swarms moving in opposing directions. One sub-swarm initiates its journey from the starting point and progresses toward the target destination, while the other sub-swarm commences from the destination and navigates back to the initial point. The underlying idea is to reduce the search area by converging at a midway point, facilitating the discovery of a shared path. This type of swarm search proves valuable for tackling problems with multiple solutions or those necessitating path planning. For instance, the human-swarm teaming (HST) framework exemplifies bi-directional swarm search by fostering effective communication and coordination between humans and swarms of robots.

#### Convergent swarm search:
It, on the other hand, centers around a single swarm moving toward a common focal point or region. Swarm agents in this scenario utilize local interactions and feedback mechanisms to adjust their positions and velocities based on specific criteria, such as minimizing a cost function or maximizing a fitness function. The primary aim is to identify an optimal or nearly optimal solution within the search space by harnessing the collective intelligence and self-organization of the swarm. Convergent swarm search proves beneficial for solving problems with either a solitary global solution or those demanding optimization. For instance, cooperative target search by a UAV swarm pursues wide-area exploration and target detection while adhering to communication constraints and information sharing. Another example lies in the Laplacian dynamics model, which characterizes both convergent and divergent swarm behaviors by considering the interplay of attraction and repulsion forces.


Besides these algorithms for pathfinding, we have also implemented multiple maze generation algorithms.
## Getting Started

To get started with the Pathfinding Visualizer, simply visit the [web page](https://pathfinding-visualizer-9474.web.app) hosted on Firebase.

### Prerequisites

You don't need to install anything to use the Pathfinding Visualizer. Ensure you have a modern web browser to access the application.

## Usage

1. Visit the [Pathfinding Visualizer](https://pathfinding-visualizer-9474.web.app) website.
2. Choose a pathfinding algorithm from the dropdown menu.
3. You may generate your own blocks or use the maze generator to create maze or both.
4. Also you may add bombs to give certain node more weights.
5. Replace the start node and the target node.
5. Click the "Visualize" button to start the visualization.
6. Watch the pathfinding algorithm in action, with color-coded animations.

## Deployment

This project is deployed using Firebase Hosting. You can deploy your own version by following the [Firebase Hosting documentation](https://firebase.google.com/docs/hosting).

## Acknowledgments

Special thanks to [Clément Mihailescu](https://www.youtube.com/@clem) for [this](https://www.youtube.com/watch?v=msttfIHHkak) amazing tutorial.

Feel free to contribute to this project, report issues, or suggest improvements. Happy pathfinding! 🚀
