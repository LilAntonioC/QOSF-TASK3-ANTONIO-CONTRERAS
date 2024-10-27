# Bin Packing Problem (BPP) Optimization with Quantum Computing

## Overview

This project focuses on solving the Bin Packing Problem (BPP) using various optimization techniques, including classical brute force methods and quantum algorithms like Quantum Annealing, Quantum Approximate Optimization Algorithm (QAOA), and Variational Quantum Circuits. The BPP involves efficiently packing a set of objects into containers while minimizing the number of containers used.

## Objectives

- Implement classical brute force algorithms to solve small instances of the BPP.
- Explore quantum methods, including quantum annealing and variational approaches, to solve the BPP.
- Compare the performance of classical and quantum methods across varying problem sizes.

## Problem Formulation

The BPP can be formulated as a binary quadratic optimization problem. Key components include:

- **Objective Function**: Minimize the number of containers used.
- **Constraints**:
  - Each object must be assigned to exactly one container.
  - The total size of objects in each container must not exceed the container's capacity.

## Implementation

### Brute Force Solver

A brute force solver is implemented to find the optimal solution by evaluating all possible combinations of object assignments.

### Quantum Approaches

1. **Quantum Annealing**: Utilizes D-Wave's quantum hardware to explore the solution space efficiently.
2. **QAOA**: A hybrid quantum-classical approach using parameterized quantum circuits to approximate the solution.
3. **Variational Quantum Circuits**: Employs quantum circuits with adjustable parameters for solving the optimization problem.

## Findings

- **Brute Force**: Effective for small instances (up to 14 objects), solving them in less than 30 seconds. Infeasible for larger problems (beyond 36 binary variables).
- **Quantum Annealing**: Demonstrated faster performance, solving small instances in 0.9 seconds and medium instances in around 2 seconds. Occasionally produced solutions violating constraints.
- **Variational Approaches**: Encountered challenges in optimization, particularly with gradient calculations, often resulting in prolonged computation times without achieving optimal solutions.


## Conclusion

This project highlights the potential of quantum computing in solving combinatorial optimization problems like the Bin Packing Problem, while also illustrating the current limitations of classical versus quantum methods.
