# Dijkstra & Floyd–Warshall Assignment

## Project Description

This project implements shortest path algorithms for weighted directed graphs using C++.

The implemented algorithms are:

- Dijkstra Algorithm (Single Source Shortest Path)
- Repeated Dijkstra Algorithm (All-Pairs Shortest Path)
- Floyd–Warshall Algorithm (Dynamic Programming APSP)

The graph is loaded from a text file and tested using Google Test.

---

## Implemented Functions

### 1. `dijkstra(int src)`

Computes the shortest paths from a source node to all other nodes using a priority queue (min-heap).

### 2. `repeatedDijkstra()`

Runs Dijkstra from every node in the graph to generate the All-Pairs Shortest Path matrix.

### 3. `floydWarshall()`

Uses dynamic programming to compute shortest paths between all pairs of nodes.

---

## Project Structure

```text
Code_library/
    dijkstra_floyd.cpp
    graph.cpp
    graph.h
    dijkstra.h
    floyd.h
    graph.txt

Googletests/
    Testcases.cpp
```

---

## How to Build and Run

### Requirements

- C++17 compiler
- Google Test framework
- VS Code or any C++ IDE
- MinGW g++ compiler (Windows)

---

## Compile the Project

Open terminal in the project folder and run:

```bash
g++ Code_library/*.cpp Googletests/Testcases.cpp -std=c++17 -lgtest -lgtest_main -pthread
```

---

## Run the Program

After compiling, run:

```bash
a.exe
```

---

## How to Run Tests

The project uses Google Test.

The following tests are included:

- Graph loading test
- Dijkstra shortest path test
- Dijkstra vs Floyd–Warshall comparison test

Run tests using:

```bash
a.exe
```

If all tests pass, the output should show:

```text
[  PASSED  ] 3 tests.
```

---

## Assumptions and Notes

- The graph is directed and weighted.
- Dijkstra algorithm assumes non-negative edge weights.
- Infinity is represented using `1e9`.
- Function signatures and project structure were not modified.
- The adjacency list is used for Dijkstra.
- The adjacency matrix is used for Floyd–Warshall.

---

## Author

Name: Mark Kyrollos
Student ID: 900211436
