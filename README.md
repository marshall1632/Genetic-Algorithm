# Genetic-Algorithm
Practical on how Genetic algorithm works and also all built from the scratch

Genetic Algorithm

•	Evolutionary algorithms
	Computational models of natural evolution processes
	Simulation of species evolution
	Survival of the fittest
	Self-organisation, adaptive behaviour
	Genetic algorithms
	Branch of Evolutionary Algorithms
	Better and better solutions based on the evolution of the previous generation.

GENETIC ALGORITHMS STEPS:
	Create initial population 
	Evaluate population
	Stopping criterion
o	Select parents
o	Crossover
o	Mutation
o	Evaluate population
o	Define surviving population
	List best individuals


1.	Knapsack
The Knapsack problem is a fundamental problem in combinatorial optimization. It has various applications and can be stated in several forms, but the most classic version is the 0/1 Knapsack problem. Here’s a breakdown of the core concepts and approaches related to the Knapsack problem:
Core Concepts
1.	Problem Definition:
o	You have a set of items, each with a weight and a value.
o	You need to determine the most valuable combination of items that can fit into a knapsack of fixed capacity.
o	Each item can either be included (1) or excluded (0) from the knapsack, hence the name 0/1 Knapsack problem.
2.	Formulation:
o	Let nnn be the number of items.
o	Each item iii has a weight wiw_iwi and a value viv_ivi.
o	The knapsack has a maximum weight capacity WWW.
o	Define a binary variable xix_ixi for each item, where xi=1x_i = 1xi=1 if the item is included in the knapsack, and xi=0x_i = 0xi=0 otherwise.
o	The objective is to maximize the total value ∑i=1nvixi\sum_{i=1}^{n} v_i x_i∑i=1nvixi while ensuring the total weight ∑i=1nwixi≤W\sum_{i=1}^{n} w_i x_i \leq W∑i=1nwixi≤W.
3.	Types of Knapsack Problems:
o	0/1 Knapsack: Each item can be chosen only once.
o	Fractional Knapsack: Items can be divided, allowing for fractional quantities.
o	Unbounded Knapsack: Unlimited quantities of each item are available.
o	Multi-dimensional Knapsack: More than one constraint (e.g., weight, volume).
Approaches to Solve the Knapsack Problem
1.	Dynamic Programming:
o	Suitable for 0/1 Knapsack problems.
o	Constructs a table to store the maximum value achievable for each sub-capacity of the knapsack.
o	Time complexity is O(nW)O(nW)O(nW), where nnn is the number of items and WWW is the knapsack capacity.
o	Pseudocode for 0/1 Knapsack using dynamic programming
2.  Greedy Algorithm:
•	Effective for the Fractional Knapsack problem.
•	Sort items by value-to-weight ratio and add as much of each item as possible.
•	Time complexity is O(nlog⁡n)O(n \log n)O(nlogn) due to sorting.
3.  Backtracking:
•	Explores all possible combinations of items.
•	Prunes branches that exceed the knapsack capacity.
•	Suitable for smaller problems due to its exponential time complexity.
4.  Branch and Bound:
•	Uses a bounding function to prune the search space.
•	More efficient than backtracking for larger problems.
•	Constructs a tree structure where each node represents a partial solution.
5.  Heuristic and Metaheuristic Algorithms:
•	Useful for large-scale or complex variations.
•	Includes methods like Genetic Algorithms, Simulated Annealing, and Ant Colony Optimization.
•	Provides near-optimal solutions in a reasonable time frame.

Individuals represent solutions
A set of individuals make up a population
The chromosome represents a solution(the chromosome is the 0 and 1)


FITNESS FUNCTION
	Quality measurement to find out how chromosomes solve the problem 
	Whether it is an acceptable solution and can be used for evolution

