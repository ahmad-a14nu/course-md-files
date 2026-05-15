# Swarm Intelligence

*   **Introduction to Swarm Intelligence**
    *   Definition and Characteristics (Decentralized, self-organized, collective goals)
    *   Inspirations from Natural Systems
        *   Bird flocks 
        *   Fish schools
        *   Ant colonies
    *   Simple Agents and Interaction Rules
        *   Attraction
        *   Repulsion
        *   Alignment
    *   Examples of Natural Swarm Intelligence (Bees, Fireflies, Termites)
*   **Swarm Optimization Algorithms** `[*]`
    *   Particle Swarm Optimization (PSO) `[*]`
    *   Ant Colony Optimization (ACO)
    *   Other Algorithms (Artificial Bee Colony, Bat Algorithm, Firefly Algorithm, Glowworm Swarm, Grey Wolf, Cuckoo Search, Dragonfly Algorithm)

# Particle Swarm Optimization (PSO) `[*]`

*   **Overview and Characteristics**
    *   Inspiration (Social behavior of bird flocking/fish schooling)
    *   Vector addition vs. Biological evolution (No crossover)
*   **Attributes of a Particle**
    *   Current Position
    *   Velocity
    *   Fitness Value
*   **Movement Influencers** `[*]`
    *   Personal best position (pbest)
    *   Global best position (gbest)
*   **PSO Algorithm Steps** `[*]`
    *   Step 1: Initialization
        *   Random generation of Position
        *   Random generation of Velocity
    *   Step 2: Particle Movement and Tracking Best Fitness
        *   Recording personal best (local best)
        *   Recording swarm's global best
    *   Step 3: Update Velocity `[*]`
        *   Velocity Equation 
        *   Velocity components (weighted current velocity, cognitive/deviation from self best, social/deviation from global best)
    *   Step 4: Update Position `[*]`
        *   Position Equation
    *   Step 5: Iteration and Termination
        *   Balancing Exploration and Exploitation
*   **PSO Parameters**
    *   1. Swarm Size (Population Size, N)
    *   2. Dimension of Particles
    *   3. Range of Particles
    *   4. Inertia Weight (w) and its Adaptive Formula
    *   5. Cognitive Component (c1)
    *   6. Social Component (c2)
    *   7. Random Coefficients (r1, r2)
    *   8. Maximum Velocity (Vmax)
    *   9. Stopping Condition
*   **Advantages of PSO (Why PSO?)**
*   **Limitations of PSO** `[*]`
    *   Premature Convergence
    *   Loss of Diversity
    *   Sensitive to Parameters
    *   Poor Performance in High Dimensions

# PSO Problem-Solving Exercise `[*]`
*(Problem: Minimizing the quadratic mathematical function $f(x) = x^2 + 3x + 5$ over the range [-10, 10])*

*   **Defining Problem Parameters** 
    *   Number of particles, iterations, velocity limits, inertia weight, cognitive/social coefficients
*   **Swarm Initialization Phase** 
    *   Initializing random positions and velocities
    *   Setting initial personal bests (pbest)
    *   Evaluating fitness to find the initial global best (gbest)
*   **Iteration #1 Execution** `[*]`
    *   Calculating updated velocity for each particle using the velocity equation
    *   Calculating updated position for each particle using the position equation
    *   Evaluating the new function value $f(x)$ for updated positions
    *   Determining the new Global Best from the updated values
*   **Iteration #2 Setup** 

# References
*   Engelbrecht (Chapter 16)
*   A.E. Eiben and J.E. Smith (Chapter 6.7)