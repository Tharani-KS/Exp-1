# Experiment 1: Exploring NumPy and Pandas

## Aim

To understand the use of NumPy and Pandas for performing basic data
manipulation and analysis in Python.

## Algorithm

1.  Import the NumPy library for matrix and numerical operations.
2.  Define a two-dimensional square matrix `A` and a vector `b`.
3.  Compute the transpose of matrix `A` to interchange rows and columns.
4.  Calculate the inverse of matrix `A` using `np.linalg.inv(A)` (ensure
    `A` is non-singular).
5.  Solve the linear equation `A × x = b` using `np.linalg.solve(A, b)`.
6.  Perform eigen decomposition to find eigenvalues and eigenvectors
    using `np.linalg.eig(A)`.
7.  Display the results for the matrix, transpose, inverse, solution
    vector, and eigenvalues.
8.  End the program.

## Formulas / Theory

-   **Transpose:** `Aᵀ` --- interchange rows and columns.
-   **Inverse:** `A⁻¹ = adj(A) / |A|`, provided `det(A) ≠ 0`.
-   **Linear system:** `A × x = b  ⇒  x = A⁻¹b`.
-   **Eigen decomposition:** `A v = λ v`, where `λ` is an eigenvalue and
    `v` is an eigenvector.

## Coding

# Step 1: Import the required libraries
import numpy as np
import pandas as pd

# Step 2: Define a matrix and vector
A = np.array([[4, 2], [3, 1]])
b = np.array([10, 7])

# Step 3: Find the transpose of the matrix
transpose = np.transpose(A)

# Step 4: Find the inverse of the matrix
inverse = np.linalg.inv(A)

# Step 5: Solve the linear equations
solution = np.linalg.solve(A, b)

# Step 6: Find eigenvalues and eigenvectors
eigenvalues, eigenvectors = np.linalg.eig(A)

# Step 7: Display the results
print("Original Matrix:")
print(A)

print("\nTranspose of Matrix:")
print(transpose)

print("\nInverse of Matrix:")
print(inverse)

print("\nSolution of Linear Equations:")
print(solution)

print("\nEigenvalues:")
print(eigenvalues)

print("\nEigenvectors:")
print(eigenvectors)

## Output

<img width="365" height="462" alt="image" src="https://github.com/user-attachments/assets/fabf3118-93b8-486e-bf61-f9bb4407e87c" />


## Result

Thus, the NumPy and Pandas libraries were explored using Python. Matrix operations such as transpose, inverse, solving linear equations, and eigenvalue and eigenvector calculation were successfully performed using NumPy.
