# AI Pathfinder - Uninformed Search Algorithms Visualization


An interactive visualization tool for comparing different uninformed search algorithms (BFS, DFS, UCS, DLS, IDDFS, and Bidirectional Search) on a grid-based pathfinding problem.


## 🔍 Overview

This project demonstrates the implementation and visualization of various uninformed search algorithms in the context of pathfinding on a grid with obstacles. Each algorithm explores the search space differently, and the visualization helps understand their behavior, strengths, and weaknesses.

The grid is 8×10 with:
- **Start (S)**: Position (6, 0) - bottom left
- **Target (T)**: Position (6, 7) - bottom right
- **Walls (-1)**: Obstacles that cannot be traversed
- **Free Space (0)**: Traversable cells
- **6-direction movement**: Up, Right, Bottom, Bottom-Right (Diagonal), Left, Top-Left (Diagonal)

## ✨ Features

- **6 Uninformed Search Algorithms**: BFS, DFS, UCS, DLS, IDDFS, Bidirectional Search
- **Real-time Animation**: Watch how each algorithm explores the grid
- **Step-by-step Visualization**: Color-coded cells show frontier, explored, and final path
- **Interactive Selection**: Choose which algorithm to run
- **Performance Metrics**: Steps taken and path found status
- **Jupyter Notebook Compatible**: Seamless integration with IPython

## 🧮 Algorithms Implemented

| Algorithm | Description                                                           | Time Complexity | Space Complexity | Complete | Optimal |
|-----------|-----------------------------------------------------------------------|-----------------|------------------|----------|---------|
| **BFS** | Breadth-First Search - explores all nodes at current depth first        | O(b^d)          | O(b^d)           | ✅       | ✅     |
| **DFS** | Depth-First Search - explores as deep as possible before backtracking   | O(b^m)          | O(bm)            | ✅       | ❌     |
| **UCS** | Uniform-Cost Search - expands lowest cost node first                    | O(b^(1+⌊C*/ε⌋)) | O(b^(1+⌊C*/ε⌋))   | ✅       |  ✅    |
| **DLS** | Depth-Limited Search - DFS with depth limit                             | O(b^l)         | O(bl)             | ❌       | ❌     |
| **IDDFS** | Iterative Deepening DFS - combines BFS completeness with DFS space    | O(b^d)         | O(bd)             | ✅       | ✅     |
| **Bidirectional** | Searches from start and target simultaneously                 | O(b^(d/2))     | O(b^(d/2))        | ✅       | ✅     |

*Where: b = branching factor, d = depth of solution, m = maximum depth, l = depth limit*

##  Installation

### Prerequisites
- Python 3.8 or higher
- pip package manager

### Steps

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/ai-pathfinder.git
cd ai-pathfinder

# Install required packages
pip install matplotlib numpy ipython


**Version 1.0 - Basic Grid Setup**
Initial grid with start, target, and walls
Simple static visualization

**Version 2.0 - BFS Implementation**
Added BFS algorithm
Path reconstruction
Basic search visualization

**Version 3.0 - Multiple Algorithms**
Implemented DFS,BFS
Added animation support
6-direction movement

**Final Version**
All 6 algorithms implemented
Interactive algorithm selection
Performance metrics
