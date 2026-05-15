# TLBO Presentation Outline

### 1. Metaheuristic Classification [*]
*   Evolution based Algorithms
*   Swarm based Algorithms
*   Physics based Algorithms
*   Human behavior based Algorithms [*]
    *   **Sports based algorithms**
        *   Ludo Game Based Metaheuristics
        *   Deer Hunting Optimization Algorithm
        *   Football Game Based Optimizer
        *   Tug of War Optimization
        *   Ring Toss Game Based
        *   Battle Royale Optimization Algorithm
        *   Puzzle Optimization Algorithm
        *   Football Team Training Algorithm
    *   **Social interaction algorithms** [*]
        *   Teaching Learning Based Optimization (TLBO) [*]
        *   A Simple Human Learning Optimization Algorithm
        *   Socio Evolution and Learning Optimization Algorithm
        *   Heap Based Optimizer
        *   Coronavirus Optimization
        *   Driving Training Based Optimization
        *   Brain Storm Optimization Algorithm
        *   Child Drawing Development Optimization Algorithm
        *   Criminal Search Optimization Algorithm
        *   Human Evolutionary Optimization Algorithm
        *   HLO with Bayesian Inference Learning
    *   **Colonization based algorithms**
        *   Cultural Evolution Algorithm
        *   Social Based Algorithm
        *   Anarchic Society Optimization Algorithm
        *   Human Urbanization Algorithm
    *   **Politics – based algorithms**
        *   Ideology Algorithm
        *   Chaotic Election Algorithm
        *   Political Optimizer
        *   Political Optimizer with Interpolation Strategy
        *   City Councils Evolution

### 2. Introduction to Teacher Learning Based Optimization (TLBO)
*   Definition and Inspiration (Classroom process)
*   Population-based method (Students as solutions)
*   Role of the Teacher (Best solution) [*]
*   Goal of TLBO (Optimal/near-optimal results)

### 3. TLBO Phases [*]
*   **Teacher phase** [*]
    *   Knowledge sharing
    *   Elevation of class average performance
*   **Learner phase** [*]
    *   Interaction and collaboration between students

### 4. Steps of TLBO [*]
*   **1) Initialization**
    *   Defining population size
    *   Defining solution dimensions
    *   Random generation of initial solutions
*   **2) Teacher Phase (Mathematical Formulation)** [*]
    *   Identification of the Teacher (Highest fitness value)
    *   Update Formula: $X_{new} = X_{old} + r \cdot (X_{teacher} – TF \cdot X_{Mean})$ [*]
    *   Parameters: Teaching Factor ($T_F$), Random number ($r$), Population Mean ($X_{Mean}$)
*   **3) Learner Phase (Mathematical Formulation)** [*]
    *   Comparison of knowledge with other students
    *   Conditional Update Formulas (based on fitness comparison) [*]
*   **4) Termination**
    *   Maximum iterations or convergence criteria
*   **TLBO Flowchart** [*]

### 5. Practical Exercise (Numerical Problem Solving) [*]
*   **Problem Statement:** Minimize the function $f(x, y) = x^2 + y^2$ [*]
*   **Initial Population and Fitness Values**
*   **Step-by-Step Execution:**
    *   Calculation of the Mean of the population [*]
    *   Execution of Teacher Phase for a specific solution ($X_2$) [*]
    *   Execution of Learner Phase for a specific solution ($X_2$) [*]
    *   Updating and accepting new solutions based on fitness

### 6. Limitations of TLBO
*   Slow convergence
*   Difficulty in exiting local optima
*   Imbalance between exploration and exploitation
*   Requirement for larger population
*   Global optimum location dependency

### 7. Literature Review and Variants
*   Historical variants of TLBO (2011–2021)
*   Main ideas of modifications (Elitist, Weighted, Dynamic Group, etc.)

### 8. References
*   Primary source: R. Rao, V. Savsani, and D. Vakharia (2011)