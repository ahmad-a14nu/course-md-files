# Evolutionary Programming (EP) Course Outline

### 1. Introduction to Evolutionary Programming (EP)
*   Focus on Behavioral Models (Phenotypic evolution) **[*]**
*   Derived from Adaptive Behavior
*   Fitness Function (Behavioral error relative to environment)
*   Comparison with GA/GP: No Crossover **[*]**
*   Mutation-Only Mechanism **[*]**

### 2. Evolving a Finite-State Machine (FSM) with EP **[*]**
*   Origin of EP (Initially designed for FSMs)
*   Objective: Predicting the next symbol in a sequence
*   Mechanism in FSM
    *   Action dependence on current state
    *   Next action determined by input
*   Formal Definition of FSM
    *   $S$: Finite set of machine states
    *   $I$: Finite set of input symbols
    *   $O$: Finite set of output symbols (alphabet)
    *   $\rho$: Next state function
    *   $\phi$: Next output function

### 3. FSM Problem-Solving Example (Process & Execution) **[*]**
*   **Problem Statement:** Develop a state machine to output $\alpha$ upon encountering the pattern 0111, otherwise output $\beta$.
*   Input alphabet: $\Sigma = \{0, 1\}$
*   Output symbols: $\{\alpha, \beta, \gamma\}$
*   FSM Components and Transitions
    *   States: {A, B, C}
    *   Transition mapping based on input character
*   Execution Trace Example **[*]**
    *   Start state assignment
    *   Input symbol sequence processing (e.g., 0 1 1 1 0 0)
    *   Present state vs. Next state mapping
    *   Output symbol generation

### 4. FSM Representation and Encoding (Data Structure) **[*]**
*   FSM Structure (3-state machine)
*   Bit-String Representation (30 bits total)
*   **Details of 10-Bit Representation for Each State [*]**
    *   1st Bit: Initial state indicator (1/0)
    *   2nd Bit: Active status (1/0)
    *   3rd & 4th Bits: Next state for 1st input symbol
    *   5th & 6th Bits: Output symbol for 1st input symbol
    *   7th & 8th Bits: Next state for 2nd input symbol
    *   9th & 10th Bits: Output symbol for 2nd input symbol
*   Mapping Values
    *   State binary codes (A=00, B=01, C=10) **[*]**
    *   Output symbol codes ($\gamma=00, \beta=01, \alpha=10$) **[*]**

### 5. Advanced FSM Management
*   Handling Unknown Optimal Number of States
    *   Implementation of maximum number of states
    *   Dynamic state management

### 6. EP vs. Genetic Algorithms (GA) **[*]**
*   Key Difference: Absence of Crossover
*   Mutation Characteristics
    *   Probability ($p_m$)
    *   Operator variation based on application

### 7. Fitness Function
*   Evaluation based on prediction accuracy
*   Selection of the most fit individual

### 8. Mutation Mechanism and Procedure **[*]**
*   Mutation Probability ($p_m$)
*   Types of Mutation Changes **[*]**
    *   Changing initial state designation
    *   Altering activation status (Adding/Removing states)
    *   Modifying state transitions
    *   Changing output symbols
*   **Mutation Procedure Steps [*]**
    1. Random number generation (0 to 1)
    2. Application of flat probability
    3. Rejection of infeasible state transitions
    4. Post-mutation fitness evaluation
*   Adjusting probability ranges (Adding/Deleting states)

### 9. Population Dynamics in EP
*   Number of children
*   Population Size Management Steps
    1. Mutation process
    2. Fitness evaluation
    3. Selection
    4. Maintenance of constant population size

### 10. References
*   Engelbrecht Chapter 10
*   A.E. Eiben and J.E. Smith Chapter 6