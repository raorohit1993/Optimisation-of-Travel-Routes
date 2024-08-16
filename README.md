0.1 Introduction
The Traveling Salesman Problem (TSP) is a cornerstone problem in combina- torial optimization. The goal is to determine the shortest possible route that allows a salesman to visit a set of cities, visiting each city exactly once and returning to the starting point. This problem is NP-hard, meaning that as the number of cities increases, the complexity of finding an optimal solution grows exponentially.
0.2 Optimization Methods for the Traveling Salesman Problem
0.2.1 DFJ Formulation
The Dantzig-Fulkerson-Johnson (DFJ) formulation is a classical linear pro- gramming model for solving the TSP. Introduced in 1954, this formulation aims to minimize the total travel distance while ensuring that each city is visited exactly once and that no subtours exist. TSP, it is computationally intensive, especially for large instances due to the large
number of subtour elimination constraints. 
0.2.2 Simulated Annealing
Simulated Annealing (SA) is a probabilistic optimization algorithm inspired by the annealing process in metallurgy. Proposed by Kirkpatrick et al. in 1983, the algorithm seeks to find a good approximation to the global optimum of a given function. For the TSP, the algorithm works as follows:
• Initial Solution: Start with an arbitrary solution, which is usually a random permutation of cities.
• Neighborhood Exploration: Slightly modify the current solution to create a neighboring solution.
• Acceptance Criterion: Always accept better solutions. Accept worse solutions with a probability that decreases as the algorithm progresses, based on a temperature parameter.
• Cooling Schedule: Gradually decrease the temperature according to a pre-defined schedule, reducing the likelihood of accepting worse solutions.
The algorithm’s ability to escape local minima makes it particularly useful for large-scale instances of the TSP, though the quality of the final solution depends heavily on the cooling schedule and the number of iterations.
3

0.3 Conclusion
This report has provided an overview of two important methods for solving the Traveling Salesman Problem: the DFJ formulation and Simulated An- nealing. The DFJ formulation, though exact, is computationally demanding for large instances, whereas Simulated Annealing offers a practical approach for finding near-optimal solutions in a feasible timeframe.
