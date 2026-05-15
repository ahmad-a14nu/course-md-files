### Evolutionary Computation Family
*   Genetic Algorithm
*   Differential Evolution (DE) [*]
*   Genetic programming
*   Evolutionary Programming
*   Evolutionary Strategy

### Differential Evolution (DE) Basics
*   Introduction
*   Origin (1995 by Storn and Price)
*   Purpose (Optimizing continuous space functions)
*   Distinguishing Feature: Differential mutation [*]
*   Applications

### DE Pseudocode / Algorithm Steps [*]
*   1. Initialization
    *   Population Setup (Candidate solutions $N_p$, Dimensionality $d$)
    *   Parameters setup (Mutation factor $F$, Crossover rate $CR$)
*   2. Mutation [*]
    *   Mutant vector creation process
    *   Mutation Equation: $V_i = X_{r0} + F \cdot (X_{r1} - X_{r2})$ [*]
*   3. Crossover [*]
    *   Trial vector ($U_i$) formulation
    *   Crossover Condition based on $CR$ and $j_{rand}$
*   4. Selection [*]
    *   Objective function comparison between Trial ($U_i$) and Target ($X_i$) vectors
*   5. Test for Convergence

### Step-by-Step Problem Example: Optimizing the Sphere Function [*]
*   Objective Function Definition & Global Minimum Identification
*   Step 1: Initialization execution 
*   Step 2: Mutation execution (Calculating new vectors based on random inputs and factor $F$) [*]
*   Step 3: Crossover execution (Combining Target vectors $X$ and Mutant vectors $V$ to create Trial vectors $U$) [*]
*   Step 4: Selection execution (Calculating and comparing objective function results to determine the next generation) [*]
*   Iterative Process (Repeating for multiple generations/threshold)

### Advantages of DE [*]
*   Simplicity and few parameters
*   Performance on complex/multi-modal problems
*   Parallelizability 

### References
*   Engelbrecht Chapter 13
*   A.E. Eiben and J.E. Smith Chapter 6