# Optimization of Molecular H₃ Molecule

Predicting the most stable arrangement of atoms in a molecule is a crucial task in quantum chemistry. This project focuses on the Trihydrogen cation (H₃⁺), aiming to determine its most stable bond length and the corresponding ground state energy, considering the molecule's symmetry in the form of an equilateral triangle. The Variational Quantum Eigensolver (VQE) algorithm is used for the same using the Pennylane library.

## Steps:

### Step 1: Initialize Atomic Coordinates
   - Intialize the Molecular coordinates and write the Hartee Fock Hailtonian.

### Step 2: Determine Qubit Requirements
   - Calculate the number of qubits needed.

### Step 3: Qubit State Initialization
   - Use Jordan-Wigner transformation to initialize the qubit state.
   -  This transformation is informed by the Hartree-Fock method, incorporating double excitation for two particles.

### Step 4: Compute the Cost Function
   - Utilize VQE to calculate the cost function i.e. expectation value of the Hamiltonian.

### Step 5: Gradient Descent Optimization
   - Apply gradient descent optimization techniques to the cost function.
   - By taking the gradient of the cost function, iteratively adjust the parameters to minimize the energy and arrive at the most stable configuration.
