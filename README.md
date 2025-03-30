# Quantum-Machine-Learning
Research codebase using MNIST that demonstrates how classical machine learning models can compete with quantum models through a novel hybrid quantum-classical feature engineering approach

1. **Data Preparation**
   - Load and preprocess the MNIST dataset.
   - Filter the dataset to include only the digits 0 and 9.
   - Reduce image dimensions using Principal Component Analysis (PCA).

2. **Quantum Feature Encoding**
   - Use quantum circuits to re-label the dataset.
   - Compute Projected Quantum Kernel (PQK) features via parameterized quantum circuits.
   - Calculate kernel matrices and perform eigenvalue decomposition to generate new labels that maximize the geometric separation between quantum and classical kernels.

3. **Model Training and Comparison**
   - Train a quantum-enhanced classical neural network on the PQK feature dataset.
   - Train a classical neural network on the original PCA-reduced dataset.
   - Compare the performance of both models (achieving > 90% accuracy on training data).

## Installation

To install the required packages, run:

```bash
pip install tensorflow==2.3.1 tensorflow-quantum cirq sympy numpy matplotlib


