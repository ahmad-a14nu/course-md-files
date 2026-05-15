# Evolutionary Strategy (ES)

*   **1. Introduction to Evolutionary Strategy (ES)**
    *   Definition and Principles
    *   Focus on real-valued parameter vectors
    *   Iterative improvement process

*   **2. Population of Solutions**
    *   Representation as real-valued vectors
    *   Evolution over generations

*   **3. Operations**
    *   **Mutation [*]**
        *   Primary variation operator
        *   Small, random changes via Gaussian distribution
    *   **Recombination (Optional)**
        *   Parent combination to produce offspring
        *   Global recombination (all parents)
        *   Local recombination (subset of parents)

*   **4. Selection Mechanisms [*]**
    *   **($\mu + \lambda$) Selection [*]** (Survival from both parents and offspring)
    *   **($\mu, \lambda$) Selection [*]** (Survival from offspring only)

*   **5. Fitness Function**
    *   Quality evaluation
    *   Search guidance for optimal solutions

*   **6. Strategy Parameters [*]**
    *   Definition (control evolution and mutation)
    *   **Mutation Example: Process and Calculation [*]**
        *   Objective: Minimize function $f(x) = x^2$
        *   Formula: $x' = x + \sigma \times N(0,1)$
        *   Role of $\sigma$ (Sigma/Step size)
        *   Impact of large vs. small $\sigma$ values

*   **7. Adaptation of Strategy Parameters [*]**
    *   Fixed Strategy Parameters
    *   Dynamic Strategy Parameters (predefined rules/time-based)
    *   **Self-Adaptation [*]**
        *   Encoding parameters into the individual's genome
        *   Individual representation: $(x, \sigma)$ [*]

*   **8. Variants of ES [*]**
    *   **(1 + 1)-ES [*]** (Single parent/offspring mutation and survival)
    *   **($\mu + \lambda$)-ES [*]** (Population competition between parents and offspring)
    *   **($\mu, \lambda$)-ES [*]** (Population competition among offspring only)

*   **9. Applications**
    *   Optimization of complex, real-valued functions
    *   Robotics and Engineering design
    *   Machine Learning (Hyperparameter tuning)

*   **10. Advantages**
    *   Handling noisy, non-linear, and multi-modal problems
    *   Robustness against local optima (stochastic variation)

*   **11. Limitations**
    *   Computational expense (large populations/high dimensions)
    *   Requirement for parameter tuning (population size, mutation rates)