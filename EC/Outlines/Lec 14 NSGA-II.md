# NSGA-II (Non-dominated Sorting Genetic Algorithm II)

- **Introduction to NSGA-II**
    - Introduced by Deb (2001)
    - Evolutionary Multi-objective Optimization (EMO)
    - $(\mu + \lambda)$ Evolutionary Algorithm principles [*]
    - Efficiency, simplicity, and diversity maintenance

- **Basic $(\mu + \lambda)$- Algorithm**
    - Algorithm Pseudocode/Flow [*]
    - Parent ($\mu$) and Offspring ($\lambda$) populations

- **Core Concepts of NSGA-II**
    - Dominance [*]
    - Crowding Distance [*]
    - A-Posteriori methods (Pareto Optimization)
        - Coverage and Convergence to the Pareto front

- **NSGA-II Algorithm Outline (Evolution Loop)**
    1. **Initialization**
        - Population $P_0$ and fitness evaluation
    2. **Evolution Loop** [*]
        - Offspring Generation ($O_t$)
        - Evaluation
        - Population Merging ($U_t = P_t \cup O_t$) [*]
        - Non-dominated Sorting [*]
        - Selection of top $N$ solutions [*]
    3. **Termination**
        - Identification of first Pareto front ($F_1$)

- **Non-dominated Sorting Procedure** [*]
    - First Pareto Front ($F_1$) identification (Rank 1)
    - Second Pareto Front ($F_2$) identification (Rank 2)
    - Iterative Repetition and Exclusivity
    - Completion/Ranking of all solutions in $U_t$
    - Visual Representation of Pareto Fronts

- **Selection of N Candidate Solutions for the Next Generation ($P_{t+1}$)** [*]
    - Front-wise Addition process
    - Case 1: Complete Front Fits
    - Case 2: Partial Front Fits (Crowding Distance usage) [*]

- **Crowding Distance Calculation Steps** [*]
    1. **Sorting**: Ascending order based on objective values
    2. **Boundary Assignment**: Setting boundary solutions to Infinity [*]
    3. **Distance Calculation**: 
        - Absolute difference between adjacent solutions
        - Mathematical Formula for $d_i$ [*]
        - Normalization across different objectives
    4. **Crowding Distance Assignment Algorithm (Pseudocode)** [*]
    5. **Strategy Impact**: Preference for higher distances/less crowded regions

- **Example – Class Activity (Problem Solving)** [*]
    - **Problem Setup**:
        - Minimization of $f_1(x)$ and $f_2(x)$ [*]
        - Defined Constraints and Subject-to conditions
    - **Numerical Data Processing**:
        - Fitness Evaluation for Parents and Offspring [*]
        - Resulting Pareto Front Sets ($F_1, F_2, F_3, F_4$) [*]

- **Fast Non-dominated Sort Algorithm** [*]
    - Domination Set ($S_p$) identification
    - Domination Counter ($n_p$) calculation
    - **Procedural Example**: 
        - Building the table for $S_i$ and $n$ for specific chromosomes [*]
        - Identifying the final $F_1$ set based on the counter $n=0$ [*]