# Lab2 - TSP

### Introduction
The goal of this laboratory is to solve the Traveling Salesman Problem (TSP); it is a classic optimization problem where a salesman needs to visit a set of cities exactly once and return to the starting city, minimizing the total travel distance.

### Approaches Used
I tried three different approaches to solve the TSP:

1. **Greedy Algorithm**; this approach starts from the first city of the set and iteratively visits the nearest unvisited city until all cities are covered; finally, it returns to the starting city to complete the tour;
2. **Evolutionary Algorithm - Version 1**; this approach aims to find a shorter path using a segment crossover and the Swap mutation;
3. **Evolutionary Algorithm - Version 2 (Inver-Over and Inversion mutation)**; this approach is similar to the previous one; however, in this case, the algorithm uses the Inver-Over crossover and the Inversion mutation.

At the end of each algorithm, the cities, the best path and their costs were displayed in 2D plots. In addition, the same best paths found were used to create several HTML files that illustrate the routes on a world map.

### Results
The results for each approach across different datasets are summarized in the table below:

|                  | Italy     | Vanuatu   | Russia     | US         | China      |
|------------------|-----------|-----------|------------|------------|------------|
| Greedy Algorithm | 4436.032  | 1475.528  | 42334.165  | 48050.026  | 63962.918  |
| EA Version 1     | 5643.244  | 1345.545  | 67685.216  | 167020.429 | 362677.202 |
| EA Version 2     | 4445.693  | 1345.545  | 41752.091  | 175554.411 | 438353.812 |

The results indicate that the Greedy Algorithm achieves lower costs almost across all countries compared to both versions of the Evolutionary Algorithm. However, a more detailed analysis shows that both the Evolutionary Algorithms can find the optimal solution for small datasets such as Vanuatu; in addition, EA version 2 performs competitively against the Greedy approach in medium datasets such as Italy and Russia; finally, the tested versions of Evolutionary Algorithms are not as effective as the Greedy solution for larger datasets such as US and China.