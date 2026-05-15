# Strength Pareto Evolutionary Algorithm 2 (SPEA2)

*   **Introduction to SPEA2** [*]
    *   Definition and Background (Enhancement of SPEA)
    *   Applications in Multi-objective Optimization Problems (MOPs)
*   **SPEA2 Algorithm Workflow** [*]
    *   Initialization
        *   Generate initial population ($P_0$)
        *   Create empty external archive ($P'_0$)
    *   Fitness Evaluation
    *   Iteration Loop (Generations $t=0$ to $M-1$)
        *   Fitness Assignment Procedure [*]
        *   Archiving (Copying non-dominated solutions) [*]
        *   Archive Truncation (Reducing archive size if necessary) [*]
        *   Selection (Binary tournament selection)
        *   Genetic Operators (Crossover and Mutation)
        *   Population Update ($P_{t+1}$)
    *   Final Ranking and Pareto-front ($F_1$) Return
*   **Fitness Assignment Mechanics** [*]
    *   Strength Value $S(i)$ [*]
        *   Definition (Number of solutions dominated by $i$)
        *   Relationship between strength and dominance
    *   Raw Fitness $R(i)$ [*]
        *   Formula (Sum of strength values of dominators)
        *   Interpretation (Lower values/Zero as non-dominated)
*   **Diversity Preservation** [*]
    *   Density Estimation [*]
        *   k-th nearest neighbor method
        *   Fitness refinement formula ($R + 1 / (2 + D_k)$)
        *   Calculation of $k$ ($k = \sqrt{popsize + archivesize}$)
    *   Archive Truncation [*]
        *   Incremental removal approach
        *   Tie-breaking rules for identical distances
*   **Practical Exercise: Solving a Bi-objective Minimization Problem** [*]
    *   Problem Setup (Population size $N=3$, Archive size $N=3$)
    *   Process Step 1: Determining Dominance and Calculating Strength $S(i)$ [*]
    *   Process Step 2: Calculating Raw Fitness $R(i)$ based on dominators [*]
    *   Process Step 3: Selection of Individuals for the Archive [*]
    *   Process Step 4: Density Estimation for Archive Expansion (Case where $N=4$) [*]
        *   Euclidean Distance Matrix Calculation [*]
        *   Calculating $k$ value (Square root of population + archive size)
        *   Sorting Distances (Excluding self-comparison)
        *   Final Solution Selection based on Density [*]