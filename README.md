# Hautus-Rosenbrock Controllability Test

This repository contains a Google Colab notebook for ECE 515 students interested in practicing or verifying a Hautus-Rosenbrock Controllability Test. 

## How to Use

1. Open the notebook in Google Colab: https://colab.research.google.com/drive/1BDLvw5ucTPo_IeVRMfiKFcWMu3EPZobK?usp=sharing 

2. Follow the instructions in the notebook to run the code.

### Information about the Test

The Hautus-Rosenbrock test is a criterion for determining the controllability of a linear time-invariant (LTI) system given by the state-space representation:

$\dot{x} = Ax + Bu$

A system is **controllable** if and only if for every eigenvalue $\lambda_i$ of the matrix $A$, the rank of the concatenated matrix $[\lambda_i I - A \mid B]$ is equal to the number of states, $n$.

That is, for each $\lambda_i \in \text{eigenvalues}(A)$:

$\text{rank}([\lambda_i I - A \mid B]) = n$

Where:
- $A$ is the state matrix ($n \times n$)
- $B$ is the input matrix ($n \times m$)
- $I$ is the identity matrix ($n \times n$)
- $\lambda_i$ is an eigenvalue of $A$
- $n$ is the dimension of the state vector (number of states)

This Colab Notebook performs the test on two user set matrices and reports if the system is controllable or not as well as controllable modes.
