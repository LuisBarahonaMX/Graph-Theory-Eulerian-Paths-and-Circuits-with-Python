# Graph Theory | Eulerian Paths, Walks, and Circuits with Python

### Graph Traversal, Network Visualization, and Discrete Mathematics Using NetworkX

**Project Type:** Educational Graph Theory Project  
**Field:** Discrete Mathematics | Graph Theory | Algorithms | Network Analysis  
**Programming Language:** Python  
**Environment:** Google Colab | Jupyter Notebook  
**Author:** Data Engineer Luis Barahona

---

## 1. Project Overview

This project explores fundamental graph theory concepts through practical examples and interactive visualizations developed with Python and NetworkX.

The notebook focuses on graph traversal, demonstrating how vertices and edges can be connected to form walks, simple paths, closed walks, and circuits.

It also introduces Eulerian path problems, which involve determining whether it is possible to traverse every edge of a graph exactly once.

The main objective is to connect mathematical graph concepts with their computational representations, providing a foundation for studying network algorithms and route optimization.

---

## 2. Project Objectives

- Understand the basic structure of graphs.
- Represent vertices and edges using NetworkX.
- Explore different types of graph traversal.
- Distinguish between walks, simple paths, and circuits.
- Visualize traversal sequences using Python.
- Identify closed walks and edge-simple circuits.
- Introduce Eulerian path problems.
- Analyze graph connectivity and vertex degrees.
- Explore practical applications in transportation, logistics, and communication networks.

---

## 3. Fundamental Graph Concepts

### 3.1 Graph Representation

A graph is a mathematical structure composed of:

- **Vertices (nodes):** Entities represented in a network.
- **Edges:** Connections between vertices.

The notebook uses NetworkX to construct undirected graphs and visualize their relationships.

### 3.2 Walks

A walk is a sequence of adjacent vertices connected by edges.

Walks may revisit vertices and edges.

The notebook illustrates different walks by highlighting selected connections in red.

### 3.3 Simple Paths

A simple path is a traversal in which vertices are not repeated.

The notebook demonstrates simple paths connecting different pairs of vertices.

### 3.4 Closed Walks

A closed walk starts and ends at the same vertex.

Vertices and edges may be repeated during the traversal.

### 3.5 Circuits

In this notebook, a circuit is treated as a closed walk that does not repeat edges.

Vertices may be revisited, provided that edges are not repeated.

---

## 4. Eulerian Paths

An Eulerian path is a traversal that visits every edge of a graph exactly once.

For a connected undirected graph, the existence of an Eulerian path depends on the number of vertices with odd degree.

### Eulerian Path Conditions

| Odd-Degree Vertices | Result |
|:---|:---|
| 0 | Eulerian circuit exists |
| 2 | Eulerian path exists, but no Eulerian circuit |
| More than 2 | No Eulerian path exists |

These conditions apply when all vertices with nonzero degree belong to the same connected component.

An Eulerian path is different from a Hamiltonian path:

- Eulerian paths focus on traversing edges.
- Hamiltonian paths focus on visiting vertices.

---

## 5. Notebook Methodology

### Step 1 — Library Imports

The notebook imports NetworkX and Matplotlib.

These libraries are used for graph construction and visualization.

### Step 2 — Initial Graph Construction

A reference graph containing six vertices is created.

The graph includes multiple connections and a self-loop.

NetworkX is used to define the graph structure, while Matplotlib displays its nodes and edges.

### Step 3 — Walk Visualization

Different vertex sequences are highlighted on the reference graph.

These visualizations demonstrate how walks can connect vertices and revisit previously traversed connections.

### Step 4 — Simple Path Examples

The notebook introduces paths without repeated vertices.

Examples illustrate how different valid paths can connect the same or different vertices.

### Step 5 — Closed Walk Examples

Closed walks are constructed to demonstrate traversal sequences that return to the starting vertex.

### Step 6 — Circuit Visualization

The notebook explores closed traversals that do not repeat edges.

### Step 7 — Eulerian Path Exercises

Two final graph examples are introduced to investigate whether all edges can be traversed exactly once.

These exercises provide opportunities to apply Eulerian path conditions.

---

## 6. Eulerian Path Exercises

### Exercise 1 — Graph with an Eulerian Path

The first graph contains six vertices:

A, B, C, D, E, and F.

Its edges are:

```python
edges = [
    ("A", "B"),
    ("A", "C"),
    ("B", "C"),
    ("B", "D"),
    ("B", "E"),
    ("C", "E"),
    ("D", "E"),
    ("E", "F")
]
```

The graph contains exactly two odd-degree vertices:

- C
- F

Therefore, an Eulerian path exists.

One valid Eulerian path is:

```text
C → A → B → C → E → B → D → E → F
```

This traversal uses each of the eight edges exactly once.

### Exercise 2 — Graph Without an Eulerian Path

The second graph contains the following edges:

```python
edges = [
    ("A", "B"),
    ("A", "C"),
    ("B", "C"),
    ("B", "D"),
    ("C", "E"),
    ("D", "E"),
    ("E", "F")
]
```

This graph has four odd-degree vertices:

- B
- C
- E
- F

Therefore, an Eulerian path does not exist.

These examples demonstrate how vertex degrees determine whether a complete edge traversal is possible.

**Note:** The notebook presents these graphs as exercises. The mathematical solutions above are documented here for reference; automated verification is not yet implemented in the original notebook.

---

## 7. Technologies Used

| Technology | Purpose |
|:---|:---|
| Python | Programming language |
| NetworkX | Graph construction and network analysis |
| Matplotlib | Graph visualization |
| Jupyter Notebook | Interactive programming environment |
| Google Colab | Cloud notebook execution |

---

## 8. How to Run

### Google Colab

Open the notebook using the link below:

[Open Graph Theory Notebook in Google Colab](https://colab.research.google.com/drive/1DuZTfi6PCufYezMHdY4il7eiw00hzNP6)

### Run Locally

Install the required libraries:

```bash
pip install networkx matplotlib notebook
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open the project notebook and execute the code cells sequentially.

The visualizations will display the different graph traversal examples.

---

## 9. Practical Applications

Graph traversal and Eulerian path analysis are relevant to several technical areas.

### Transportation and Logistics

- Route planning
- Street network traversal
- Delivery optimization
- Transportation network analysis

### Telecommunications

- Network connectivity
- Communication route analysis
- Network redundancy exploration

### Computer Science

- Algorithm design
- Network analysis
- Graph-based problem solving
- Discrete mathematics education

### Data Engineering

- Relationship modeling
- Graph data structures
- Connected data analysis
- Network representation

---

## 10. Limitations

This notebook is primarily an educational exploration of graph theory.

Current limitations include:

- Several exercise cells remain incomplete.
- Eulerian paths are not automatically computed.
- The examples emphasize visualization rather than algorithm benchmarking.
- Some highlighted traversals do not fully represent repeated edges because they are drawn as simple directed graphs.
- The project does not implement large-scale route optimization.
- Further validation is needed before adapting the examples to real transportation networks.

---

## 11. Future Improvements

Potential extensions include:

- Implementing automatic Eulerian path detection.
- Using NetworkX's `has_eulerian_path()`.
- Computing Eulerian traversals with `eulerian_path()`.
- Adding vertex-degree tables.
- Incorporating automated validation of traversal sequences.
- Comparing Eulerian and Hamiltonian problems.
- Visualizing traversal order and direction.
- Applying graph algorithms to real transportation networks.

---

## 12. Conclusion

This project provides a practical introduction to graph theory using Python and NetworkX.

Through graph construction and visualization, the notebook demonstrates the differences between walks, simple paths, closed walks, and circuits.

The Eulerian path exercises illustrate how vertex degrees influence the existence of complete edge traversals.

These concepts establish a mathematical foundation for more advanced studies in network analysis, route planning, graph algorithms, and computational optimization.

---

## 13. Project Resources

### Google Colab Notebook

[Explore the Notebook](https://colab.research.google.com/drive/1DuZTfi6PCufYezMHdY4il7eiw00hzNP6)

### NetworkX Documentation

[NetworkX — Graph Analysis Library](https://networkx.org/documentation/stable/)

---

## Author

**Data Engineer Luis Barahona**

Mexican Data Engineer and 2026 graduate of Universidad del Caribe, passionate about technology, Data Science, Artificial Intelligence, algorithms, and continuous learning.

---

## Contact

| Platform | Contact |
|:---|:---|
| Email | [190300395@ucaribe.edu.mx](mailto:190300395@ucaribe.edu.mx) |
| GitHub | [github.com/LuisBarahonaMX](https://github.com/LuisBarahonaMX) |
| LinkedIn | [linkedin.com/in/luis-barahona-mx](https://www.linkedin.com/in/luis-barahona-mx/) |
| Instagram | [@luisbarahonamx](https://www.instagram.com/luisbarahonamx/) |
| X | [@luisbarahonaMX](https://x.com/luisbarahonaMX) |
| Website | [SIKO AI Platform](https://sikoai.web.app/) |
