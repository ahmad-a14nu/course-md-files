# Genetic Algorithms: Course Outline

## 1. Introduction to Evolutionary Computation (EC)
### 1.1 Overview and Definition
*   Relationship between AI and EC
*   Inspiration from Biological Evolution
*   The Concept of Natural Selection (Darwinism) [*]
### 1.2 Evolutionary Hierarchy
*   EC within Computational Intelligence
*   Related Nature-inspired Algorithms (Genetic Programming, Differential Evolution, etc.)
### 1.3 Real-world Analogies
*   Evolution of Racehorse Bloodlines

## 2. Fundamental Concepts & Terminology [*]
### 2.1 The GA Vocabulary
*   **Gene:** Basic unit/feature (Allele as the value)
*   **Chromosome:** Sequence of genes (Candidate solution)
*   **Population:** Group of chromosomes in a generation
### 2.2 Representation Types
*   Binary Encoding [*]
*   Real-Valued Encoding
*   Permutation Encoding (e.g., 8 Queens) [*]
### 2.3 Mapping Concepts
*   Genotype vs. Phenotype [*]
*   Importance of representation for efficiency

## 3. The General Evolutionary Scheme [*]
### 3.1 Basic Flowchart of GA [*]
1.  Initialization
2.  Fitness Evaluation
3.  Selection
4.  Recombination (Crossover)
5.  Mutation
6.  Survivor Selection
7.  Termination

## 4. Population and Initialization
### 4.1 Population Generation
*   Standard (Random) Method
*   Heuristic Initialization (Risk of local optimum)
### 4.2 Impact of Population Size
*   Small Population (Faster, but less exploration)
*   Large Population (Slower, but covers more search space)
*   Mutation to compensate for small populations [*]

## 5. Selection Operators [*]
### 5.1 Selection Pressure
*   High vs. Low Selection Pressure
*   Risk of premature convergence
### 5.2 Selection Schemes [*]
*   **Tournament Selection:** (Adjusting size to change pressure) [*]
*   **Roulette Wheel / Proportionate Selection:** (Fitness-based probability) [*]
*   **Rank-based Selection:** (Addressing excessive pressure from raw fitness) [*]
*   **Random Selection:** (Equal chance for all)
*   **Steady State Selection:** (Replacing bad chromosomes with new ones)

## 6. Advanced Parameters and Selection Policies
### 6.1 Generation Gap (GP) [*]
*   Calculation of population fraction replaced
### 6.2 Elitism [*]
*   Preserving the $k$ best individuals
*   **Exercise:** Calculation of GP and Elitism values from a scenario [*]
### 6.3 Duplicate Management
*   Eliminating duplicates to prevent premature convergence

## 7. Recombination and Variation Operators [*]
### 7.1 Crossover Operators [*]
*   Single-Point Crossover
*   Two-Point Crossover
*   Uniform Crossover (Random Binary Mask) [*]
*   Position-based Crossover (For permutations)
*   Order-based Crossover (For permutations)
### 7.2 Mutation Operators [*]
*   Bit Flip (Binary)
*   Random Resetting (Integers)
*   Swap / Scramble / Inversion (Permutations) [*]
*   Boundary-Replaces (Real-valued)

## 8. Step-by-Step Problem Solving Examples (Process-Driven) [*]

### 8.1 The 8 Queens Problem (Permutation-based) [*]
*   **Step 1:** Representation (Index = Column, Value = Row)
*   **Step 2:** Random Initialization
*   **Step 3:** Fitness Function (Number of non-attacking pairs)
*   **Step 4:** Parent Selection
*   **Step 5:** Crossover Implementation
*   **Step 6:** Mutation for diversity
*   **Step 7:** Reaching the Goal (Fitness = 28)

### 8.2 The Knapsack Problem (Optimization-based) [*]
*   **Constraints:** Weight Capacity (e.g., 12kg)
*   **Objective:** Maximize Value
*   **Process:** Binary string representation, Weight/Value calculation, and Roulette Wheel Selection application. [*]

## 9. Analysis and Types of GAs
### 9.1 Classification
*   Generational GA (Standard)
*   Incremental / Steady State GA
### 9.2 Performance Measures
*   Accuracy (Objective Value vs. Optimality Gap)
*   Convergence (Rate and Final state) [*]
*   Computational Efficiency (Execution Time vs. Iterations)
*   Robustness (Consistency and Sensitivity)
*   Exploration vs. Exploitation [*]
*   Scalability (Problem Size)

## 10. Practical Issues & Applications
### 10.1 Implementation Challenges
*   Choosing representation and operator parameters
### 10.2 Application Domains
*   Control, Scheduling, Robotics, and Machine Learning.
*   Specifics: DNA Analysis, Traveling Salesman (TSP), and VLSI Design. [*]