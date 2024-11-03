# Lab2 - TSP

### Introduction
The goal of this laboratory is to solve the Traveling Salesman Problem (TSP); it is a classic optimization problem where a salesman needs to visit a set of cities exactly once and return to the starting city, minimizing the total travel distance.

Travelling Salesman Problem (TSP) Solver
This project is a Python-based implementation for solving the Travelling Salesman Problem (TSP) using various algorithms, including a Minimum Spanning Tree (MST)-based approximation. The code is designed to load city data for various countries, calculate distances between cities, and find an approximate solution to the TSP using a greedy algorithm. The solution is presented with detailed outputs and visualizations.

Algorithms Implemented
Minimum Spanning Tree (MST) Approximation
The TSP tour is approximated using an MST-based approach:

Graph Creation: Cities are represented as nodes, with distances as edge weights.
MST Generation: A Minimum Spanning Tree is created to cover all nodes with the minimum total edge weight.
DFS Preorder Traversal: Nodes in the MST are visited in a Depth-First Search (DFS) preorder manner to form the approximate TSP path.
Features
Automatic Distance Calculation: Calculates geodesic distances (in km) between city coordinates.
MST-based Approximation: Provides a greedy solution that is computationally efficient.
Detailed Output: Prints each tour step with city names and step distances.
Visualization: Plots the distance evolution over generations (if using optimization across generations).