# Genetic Programming

*   **GP Characteristics Summary**
    *   Representation (Tree structures)
    *   Recombination (Exchange of subtrees)
    *   Mutation (Random change in trees)
    *   Parent selection (Fitness proportional)
    *   Survivor selection (Generational replacement)
*   **Specialization of Genetic Algorithms (GAs)**
    *   Representation Scheme: GA vs. GP [*]
        *   Linear string vs. Tree-based representation
        *   Fixed size vs. Variable depth/width (Non-linear)
        *   Maximum depth constraints
*   **Fitness Function**
    *   Problem-Dependent Design
    *   Fitness Evaluation Process
        *   Testing on domain sample cases
        *   Average performance metrics
    *   Example: Program Fitness Evaluation [*]
        *   Input (variables and target values)
        *   Evaluation (compute output, calculate MSE)
        *   Fitness scoring based on average error
*   **Tree-Based Representation** [*]
    *   Arithmetic Formula Representation
    *   Logical Formula Representation
    *   Program Code Structure Representation (e.g., While loops)
*   **Chromosome Representation**
    *   Sets Definition [*]
        *   Terminal Set (Leaf nodes: variables, constants)
        *   Function Set (Non-leaf nodes: operations, functions)
    *   Example: Mathematical Equation Mapping to Tree [*]
    *   Program Space 
        *   Grammar Components
        *   Objective Search Space
*   **Algorithm Flow: GA Vs. GP** [*]
    *   GA Scheme (Sequential Crossover AND Mutation)
    *   GP Scheme (Probabilistic Crossover OR Mutation Flowchart)
*   **Initial Population Generation** [*]
    *   Random Generation Constraints
    *   Root Selection
    *   Branching Factor (Arity determination)
    *   Node Initialization Process
*   **Selection Process**
*   **Crossover Operator** [*]
    *   Two Offspring Creation Process (Swapping corresponding subtrees)
    *   One Offspring Creation Process (Replacing subtree from one parent)
    *   Purpose of Crossover
*   **Mutation Operators** [*]
    *   Function Node Mutation (Process and Purpose)
    *   Terminal Node Mutation (Process, Purpose, and Impact)
    *   Swap Mutation (Process, Purpose, and Impact)
    *   Grow Mutation (Process, Purpose, and Impact)
    *   Truncate Mutation (Process, Purpose, and Impact)
*   **Mutation Operator with Probabilities**
    *   Individual Selection for Mutation (Probability $p_m$)
    *   Node Mutation within the Tree (Probability $p_n$)
    *   Impact of Probabilities (Exploration vs. Exploitation)
*   **Fitness Evaluation (Step-by-Step Problem Solving Example)** [*]
    *   Target Program Approximation ($y = x^2 + x + 1$)
    *   Candidate Program ($y = x^2 + 2$)
    *   Error Computation Table (True Output vs. Predicted Output)
    *   Total Error Calculation
    *   Alternative Fitness Formula Formulation ($Fitness = 1 / (1 + Error)$)
*   **References**
    *   Engelbrecht (Chapter 10)
    *   A.E. Eiben and J.E. Smith (Chapter 6)