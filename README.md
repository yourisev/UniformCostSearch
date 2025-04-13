# 🚀 Uniform Cost Search (UCS) in Java

This project implements the **Uniform Cost Search algorithm** to find the **least-cost path** between two vertices in a weighted graph. The program takes input as an **adjacency matrix**, and returns both the **path** and the **minimum distance** from the source node to the destination.

---

## 📌 Why This is Useful

- ✅ UCS is a graph traversal algorithm ideal for finding the **shortest path in weighted graphs**.
- 💲 It expands the **least-cost node** first using a **priority queue**.
- 💡 The implementation includes path reconstruction and handles disconnected graphs gracefully.
- 🧪 Great for learning **priority queue operations**, **greedy strategies**, and **graph representation** in Java.

---

## 🧩 How It Works

1. **Input**:
   - Number of vertices
   - Weighted adjacency matrix
   - Source and destination vertices

2. **Processing**:
   - Uses a `PriorityQueue<Node>` to always expand the node with the least cumulative cost.
   - Uses a `HashSet` to keep track of visited nodes.
   - Updates distances and parent pointers to trace back the shortest path.

3. **Output**:
   - The shortest path (via backtracking with `parent[]`)
   - The total distance

---

## 🧠 Key Concepts Used

| Concept | Description |
|--------|-------------|
| `PriorityQueue<Node>` | Maintains the frontier with cost-based priority |
| `HashSet` | Tracks settled (visited) nodes |
| `LinkedList` | Reconstructs and prints the path from destination back to source |
| `adjacencyMatrix` | Represents the weighted graph; 0 means no edge unless it's a self-loop |
| `Node` class | Comparable wrapper for graph node and path cost |

---

## 🛠 How to Run

🖥️ Prerequisites
- Java JDK 8 or higher

🔧 Compile
 ```bash
 javac UniformCostSearch.java
 ```

▶️ Run
```bash
java UniformCostSearch
```

Follow the prompts in the console to input:
- The number of nodes
- Weighted adjacency matrix
- Source and destination vertices
