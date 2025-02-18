# Route Finding Problem

## Overview
This project implements a **Route Finding Algorithm** to determine the optimal path between two points on a given map. The solution uses graph-based search algorithms such as **Dijkstra's Algorithm, A* Search, and BFS/DFS** to find the most efficient route.

## Features
- Implements multiple pathfinding algorithms:
  - **Dijkstra's Algorithm** (Shortest Path)
  - **A* Search** (Heuristic-based optimal path)
  - **Breadth-First Search (BFS)** (Unweighted optimal path)
  - **Depth-First Search (DFS)** (Exploratory search)
- Supports **weighted and unweighted graphs**
- Interactive **visualization of the route**
- Handles **real-world road networks** using OpenStreetMap data
- Allows for **custom map input** in JSON or adjacency list format

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/route-finding-problem.git
   cd route-finding-problem
   ```
2. Install required dependencies:
   ```sh
   pip install -r requirements.txt
   ```

## Usage
Run the script with:
```sh
python main.py --algorithm dijkstra --start A --end B
```

### Command Line Arguments
| Argument | Description |
|----------|-------------|
| `--algorithm` | Choose from `dijkstra`, `astar`, `bfs`, or `dfs` |
| `--start` | Starting node |
| `--end` | Destination node |
| `--map` | (Optional) Path to custom map file |

### Example
To find the shortest path between nodes **A** and **B** using A* Search:
```sh
python main.py --algorithm astar --start A --end B
```

## Visualization
The project includes a graphical visualization of the computed path. The path is displayed on a grid map, highlighting the **shortest route** from start to destination.

## File Structure
```
route-finding-problem/
│── data/               # Contains map data files
│── src/                # Implementation of pathfinding algorithms
│   │── dijkstra.py     # Dijkstra's Algorithm
│   │── astar.py        # A* Search
│   │── bfs.py          # Breadth-First Search
│   │── dfs.py          # Depth-First Search
│── visualization/      # Path visualization module
│── main.py             # Main execution script
│── README.md           # Project documentation
│── requirements.txt    # Required Python libraries
```
##Image

![Screenshot 2025-02-18 154622](https://github.com/user-attachments/assets/4dfaf9bf-04cc-4970-a7e9-7177eb4ff135)


## Technologies Used
- **Python**
- **NetworkX** (Graph manipulation)
- **Matplotlib** (Path visualization)
- **OpenStreetMap API** (Optional, for real-world maps)

## Future Enhancements
- Integrate **Google Maps API** for real-time road networks
- Implement **bidirectional search** for improved efficiency
- Add **GPS-based real-world routing**

## Contributors
- [Your Name](https://github.com/squadron-leader)

## License
This project is licensed under the **MIT License**.

