# Performance Assessment in Multi-Objective Optimization

### 1. Introduction to Performance Assessment
* Effectiveness of Multi-objective Optimization Algorithms (MOA)
* Solving Multi-objective Problems (MOPs)
* Goals of a good algorithm: Well-distributed, diverse, and optimal solutions along the Pareto Front (PF) [*]
* Quality Indicators: Types and Statements
    * Independent of user preferences
    * Dependent on user preferences

### 2. Quality Measures (Indicators) [*]
* **Measuring Convergence** [*]
    * Epsilon
    * Generational Distance (GD)
* **Measuring Convergence and Diversity** [*]
    * Hypervolume (HV)
    * Inverted Generational Distance (IGD)
* **Measuring Diversity** [*]
    * Spread
    * Generalized Spread

### 3. Generational Distance (GD)
* Definition: Distance from obtained approximation to the true Pareto-optimal front
* Mathematical Formula and Variables ($n$, $d_i$)
* Interpretation of Values (GD = 0 signifies perfect convergence)
* **Step-by-Step Calculation Exercise (Computing GD for 2-objective space)** [*]
    * Step 1: Compute Euclidean Distances (Nearest point in $PF^*$ for each solution in $S$)
    * Step 2: Apply GD Formula (Root mean square of distances)
* Drawbacks of GD
    * Ignores Diversity [*]
    * Sensitivity to Outliers
    * Scaling Issues (Population size dependence)
    * Requirement of the True Pareto Front [*]

### 4. Inverted Generational Distance (IGD)
* Definition: Variant of GD measuring both Convergence and Diversity [*]
* Mathematical Formula and Variables ($|PF^*|$, $d_j$)
* Interpretation of Values (Lower IGD is better; IGD = 0 is perfect)
* **Step-by-Step Calculation Exercise (Computing IGD)** [*]
    * Computing Euclidean Distance for each point $p^*$ on the True Front to the closest point in the approximation set
    * Summation and averaging of minimum distances
* Drawbacks of IGD
    * Requirement of True Pareto Front
    * High Computational Cost ($O(m \times n)$ complexity) [*]
    * Effectiveness issues in Many-Objective Optimization (MaOPs)
    * Curse of Dimensionality (>3 objectives) [*]

### 5. HyperVolume (HV)
* Definition: Volume of objective space dominated by solutions relative to a reference point
* Interpretation of Values (Larger HV indicates better convergence and diversity) [*]
* Mechanism: Points and Reference Point normalization
* **Step-by-Step Calculation Exercise (Computing HV)** [*]
    * Step 1: Normalization of Objective Values (Formula: $x_{norm} = \frac{x - x_{min}}{x_{max} - x_{min}}$) [*]
    * Step 2: Identify Reference Point
    * Step 3: Calculate Area dominated by each solution
    * Step 4: Total Area calculation (Sum of HVA + HVB)
* Drawbacks of HV
    * Computational Complexity (Expensive as objectives increase) [*]
    * Sensitivity to Reference Point selection [*]
    * Difficulty of interpretation in High Dimensions

### 6. Spread ($\Delta$)
* Definition: Metric for even distribution and diversity along the Pareto Front
* Mathematical Formula components ($d_f$, $d_l$, $d_i$, $\bar{d}$)
* Interpretation of Values (Ideal value = 0 for perfect spacing) [*]
* **Step-by-Step Calculation Exercise (Computing Spread for 2-objective minimization)** [*]
    * Calculation of $d_f$ and $d_l$ (Distances to extreme points)
    * Calculation of consecutive distances ($d_i$)
    * Calculation of Mean ($\bar{d}$)
    * Calculation of Deviation from Mean
* Drawbacks of Spread
    * Sensitivity to Extreme Solutions [*]
    * Requirement of Ordered Solutions (Challenging in 3+ objectives)
    * Limitations in High Dimensions
    * Scale Sensitivity between different objective functions

### 7. Generalized Spread
* Extension for 2-objective Spread to higher dimensions
* Distance to nearest neighbor approach
* **Exercise: 3-objective minimization problem with extreme points** [*]

### 8. Coverage (C-metric)
* Definition: Fraction of solutions in one set weakly dominated by another set
* Mathematical Formula and Notation ($a \leq b$)
* Domination rules (Better in all objectives, strictly better in at least one) [*]
* Range of values (0 to 1)
* **Step-by-Step Calculation Exercise (Coverage for Maximization Problem)** [*]
    * Calculating $C(A,B)$ (Percentage of Set B dominated by A)
    * Calculating $C(B,A)$ (Percentage of Set A dominated by B)