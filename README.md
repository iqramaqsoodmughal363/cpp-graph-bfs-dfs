# 🌐 Graph with BFS and DFS Traversal in C++

> A C++ program implementing an undirected **Graph** using adjacency lists with **Breadth-First Search (BFS)** and **Depth-First Search (DFS)** traversal algorithms.

---

## 📋 Overview

A **Graph** is a non-linear data structure consisting of vertices (nodes) and edges connecting them. This program represents an undirected graph using an **adjacency list** and demonstrates two fundamental traversal algorithms:

- **BFS (Breadth-First Search):** Explores level by level, uses a queue.
- **DFS (Depth-First Search):** Explores as deep as possible, uses recursion (stack).

---

## ✨ Features

- ✅ Graph implementation using adjacency list (`vector<vector<int>>`)
- ✅ Add edges (undirected)
- ✅ BFS traversal using `std::queue`
- ✅ DFS traversal using recursion
- ✅ Visited array to avoid revisiting nodes
- ✅ Clean and modular class-based implementation
- ✅ Beginner-friendly with proper comments

---

## ⏱️ Complexity Analysis

| Algorithm | Time Complexity | Space Complexity |
| :---: | :---: | :---: |
| **BFS (Adjacency List)** | O(V + E) | O(V) – Queue + Visited array. |
| **DFS (Adjacency List)** | O(V + E) | O(V) – Recursion stack + Visited array. |

*Where V = Number of vertices, E = Number of edges.*

---

## 💻 Sample Input / Output

**Graph Structure:**
0 — 1 — 3
| |
2 — 4

text

**Input:**
Edges: (0,1), (0,2), (1,3), (2,4)
Start Node: 0



**Output:**
BFS: 0 1 2 3 4
DFS: 0 1 3 2 4



*(Note: DFS output may vary based on adjacency list order.)*

---

## 🧮 Program Logic & Execution Flow

### 1. **BFS (Breadth-First Search)**
- Uses a `queue<int>` to store nodes to visit.
- Marks the start node as visited and pushes it to the queue.
- While the queue is not empty:
  - Pop the front node and print it.
  - For each unvisited neighbor, mark it visited and push it to the queue.

### 2. **DFS (Depth-First Search)**
- Uses recursion (implicit stack).
- Marks the current node as visited and prints it.
- For each unvisited neighbor, recursively calls `DFSUtil()`.

### 3. **Graph Class**
- `addEdge(u, v)`: Adds an edge between `u` and `v` (undirected).
- `BFS(start)`: Traverses the graph starting from `start`.
- `DFS(start)`: Traverses the graph starting from `start`.

---

## 🛠️ How to Compile and Run (Windows & Linux)

Follow the instructions below based on your operating system.

### 🪟 For Windows Users (Using MinGW/G++ or any C++ compiler)
| Step | Command |
| :---: | :--- |
| **1. Compile** | `g++ -std=c++11 graph_bfs_dfs.cpp -o graph_bfs_dfs.exe` |
| **2. Run** | `graph_bfs_dfs.exe` |

> **Note:** If `g++` is not recognized, make sure MinGW is installed and added to your System PATH.

---

### 🐧 For Linux / macOS Users (Terminal)
| Step | Command |
| :---: | :--- |
| **1. Compile** | `g++ -std=c++11 graph_bfs_dfs.cpp -o graph_bfs_dfs` |
| **2. Run** | `./graph_bfs_dfs` |

> **Prerequisite:** Ensure GCC/G++ is installed on your system. (On Linux: `sudo apt install g++` | On macOS: `xcode-select --install`)

---

## 📂 Project Structure
cpp-graph-bfs-dfs/
│
├── graph_bfs_dfs.cpp # Main source code file
└── README.md # Project documentation (this file)



---

## 🔍 Real-World Applications

- **Social Networks:** Finding friends, recommendations (BFS).
- **Web Crawling:** Google uses BFS/DFS to index web pages.
- **GPS Navigation:** Finding shortest paths in maps.
- **Network Topology:** Analyzing network connectivity.
- **AI & Search:** Solving puzzles, game trees (like chess).
- **Pathfinding:** Used in algorithms like Dijkstra, A*.

---

## 🧠 Key Learnings

- **BFS vs DFS:** BFS is good for shortest paths, DFS for exploring all paths.
- **Adjacency List:** Efficient representation for sparse graphs.
- **Queue vs Stack:** BFS uses queue (FIFO), DFS uses stack (LIFO/recursion).
- **Visited Array:** Prevents infinite loops and revisiting.
- **Graph Traversal:** All nodes are visited exactly once.

---

## 🔧 Potential Enhancements

- **Weighted Edges:** Add weights to edges.
- **Directed Graph:** Modify to support directed edges.
- **Shortest Path:** Implement Dijkstra's Algorithm.
- **Cycle Detection:** Add cycle detection for directed/undirected graphs.
- **Connected Components:** Count the number of connected components.
- **Iterative DFS:** Implement DFS without recursion (using explicit stack).
- **Generic Graph:** Use templates for different data types.

---

## 👩‍💻 Author

**Iqra Maqsood Mughal**  
*C++ Developer | Programming Enthusiast*

---

## 📅 Date

**August 6, 2026**

---

## 📄 License

This project is open-source and intended for educational purposes.
