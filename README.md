Artificial Bee Colony
The Artificial Bee Colony (ABC) algorithm is a swarm-based search algorithm inspired by the foraging behavior of honey bees. Developed by Prof. Dr. Derviş Karaboğa, this algorithm is used to solve optimization problems by simulating the intelligent foraging behavior of bees.

Key Concepts
1-Initialization: Generate initial random solutions (food sources).

2-Employed Bees Phase: Each employed bee searches for new solutions near their current food source.

3-Onlooker Bees Phase: Onlooker bees choose food sources based on the quality of the food source and search for new solutions.

4-Scout Bees Phase: If a food source is abandoned, a scout bee searches for a new random food source.

5-Termination: Repeat the employed, onlooker, and scout phases until a stopping criterion is met.

The ArtificialBeeColony class initializes with the following input parameters:
G: A NetworkX graph that represents the TSP problem being solved

num_bees: The number of candidate solutions (i.e., bees) in the population

max_iterations: The maximum number of iterations before the algorithm stops

The class has the following methods:
evaluate_fitness: Computes the fitness value of a given path, which represents a candidate solution to the TSP problem.

apply_random_neighborhood_structure: Applies a neighborhood structure to a given path, which generates a new candidate solution.

sort_population_by_fitness: Sorts the population of candidate solutions based on their fitness values.

choose_solution_with_probability: Selects a candidate solution from the population based on the probability of the solution's fitness.

generate_possible_solution: Generates a new candidate solution by randomly generating a path in the graph.

run: Runs the ABC algorithm and returns the best solution and its fitness value.
