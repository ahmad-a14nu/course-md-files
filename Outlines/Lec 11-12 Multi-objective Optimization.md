# Multi-objective Optimization

*   **Core Concepts of MOO**
    *   Multiple Objectives
    *   Trade-offs
    *   Pareto Front [*]
*   **Application Examples**
    *   Car Buying
    *   Supply Chain Management
    *   Environmental Management
*   **Comparison of Optimization Types**
    *   Single objective optimization
    *   Multi-objective optimization (Objective functions $f_1, f_2, f_3$)
*   **Dominance Relationship [*]**
    *   Definition of Dominance (no worse in all, strictly better in one) [*]
    *   Dominance Comparison Examples (1 Vs 2, 1 Vs 5, 1 Vs 4) [*]
    *   Weak Dominance ($x \preceq y$)
    *   Non-dominated solution set [*]
    *   Dominance in 2D space (Dominating, Dominated, and Incomparable regions) [*]
*   **Pareto Optimality Concepts**
    *   Pareto Optimal Set
    *   Pareto Optimal Front [*]
    *   Front Variations (Min-min, Min-max, Max-min, Max-max) [*]
*   **Decision and Objective Spaces**
    *   Decision Space ($x_1, x_2, \dots, x_n$)
    *   Objective Space ($y_1, y_2, \dots, y_k$)
    *   Mapping from Search to Evaluation
*   **Algorithm Design Issues [*]**
    *   Optimization Goals
        *   Convergence (Finding the front) [*]
        *   Diversity (Finding a representative range) [*]
    *   Three Primary Design Components [*]
        1.  Fitness assignment
        2.  Diversity Preservation
        3.  Elitism (Environmental selection)
*   **1. Fitness Assignment Strategies [*]**
    *   **A) Aggregation-based (Scalarization-based) [*]**
        *   Aggregation Approach (Combining into a single function)
        *   Systematic Variation of parameters
        *   Weighted-Sum Aggregation formula ($w_1f_1 + w_2f_2 \dots$) [*]
        *   Advantages (Efficiency, Simple implementation)
        *   Disadvantages (Defining weights, Non-convex Pareto fronts) [*]
    *   **B) Criterion-based (Objective-based) [*]**
        *   Vector Evaluated Genetic Algorithm (VEGA) [*]
        *   Advantages and Disadvantages
        *   **Procedural Example: Designing aircraft component material (Solving conflicting objectives of Weight vs. Strength)** [*]
            *   Step 1: Initialization
            *   Step 2: Subpopulation Creation (splitting population for specific objectives) [*]
            *   Step 3: Selection Process (ranking by specific criteria per subpopulation) [*]
            *   Step 4: Crossover & Mutation
            *   Step 5: Iteration for Generations
    *   **C) Dominance-based [*]**
        *   Dominance Metrics [*]
            1.  Dominance Rank (DR): How many individuals dominate a solution? [*]
            2.  Dominance Count (DC): How many individuals does a solution dominate? [*]
            3.  Dominance Depth (DD): Which Pareto front layer is the solution in? [*]
        *   **Procedural Example: Calculating DR, DC, and DD for Population A, B, and C based on Cost vs. Quality** [*]
*   **2. Diversity Preservation [*]**
    *   Density-dependent selection probability
    *   Common Methods:
        1.  Crowding Distance (NSGA-II) [*]
        2.  Strength Pareto Ranking (SPEA2)
        3.  Reference-Point-Based Methods (MOEA/D)
*   **3. Elitism-Environmental Selection [*]**
    *   Implementation Variants (With Archive vs. Without Archive)
    *   Selection Criteria for Environmental Selection:
        1.  Dominance (Keeping non-dominated solutions) [*]
        2.  Density-Based Selection (Crowding Distance) [*]
        3.  Time-Based Selection (Steady-state algorithms)
        4.  Chance-Based Selection (Equal probability)
*   **Techniques to Solve Multi-objective Problems (MOP) [*]**
    *   **1) A Priori Methods [*]**
        *   Preferences set before optimization (e.g., Weighted Sum)
    *   **2) A Posteriori Methods [*]**
        *   Optimization first, selection later (e.g., NSGA-II, MOPSO)
    *   **3) Interactive Methods [*]**
        *   Preferences refined during optimization iterations
    *   **Comparison of Techniques (Aspects: Timing, Involvement, Flexibility, Computation Time)** [*]
*   **Evolutionary Computing (EC) for MOO**
    *   Benefits of EAs (Population-based, single run discovery of multiple solutions)
    *   Robustness against Pareto front shape and continuity [*]