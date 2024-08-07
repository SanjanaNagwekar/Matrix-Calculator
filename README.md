# Matrix Calculators

## Project Overview

This repository contains three advanced matrix operation projects implemented in C, focusing on demonstrating various programming techniques such as parallel processing, multithreading, and mathematical computations like matrix multiplication and cosine distance calculation. The projects highlight robust error handling, efficient memory management with malloc, and utilize the exec family of system calls for process execution. Each program is designed to handle matrix operations efficiently.

### Projects Included:

1. **Matrix Calculator Using Parallelization**: Utilizes child processes for matrix multiplication with input from standard files.
2. **Matrix Multiplication Using Threads**: Employs POSIX threads to perform matrix multiplication safely and efficiently.
3. **Matrix Cosine Distance Calculation**: Combines matrix operations and calculates the cosine distance between vectors.

Each project is tailored to provide practical examples of handling complex matrix operations in a concurrent computing environment.

## Compilation and Execution

### Matrix Calculator Using Parallelization

- **Compilation**:
  ```bash
  gcc -o matrixmult_multiwa matrixmult_multiwa.c -Wall -Werror
  gcc -o matrixmult_parallel matrixmult_parallel.c -Wall -Werror
  ```
- **Running**: 
  ```bash
  ./matrixmult_multiwa A1.txt W1.txt W2.txt W3.txt
  ```

### Matrix Multiplication Using Threads

- **Compilation**:
  ```bash
  gcc -D_REENTRANT -pthread -o matrixmult_threaded matrixmult_threaded.c -Wall -Werror
  ```
- **Running**:
  ```bash
  ./matrixmult_threaded path_to_matrix_A_file path_to_matrix_W_file
  ```

### Matrix Cosine Distance Calculation

- **Compilation**:
  ```bash
  gcc -o matrixmult matrixmult.c -lm
  ```
- **Running**:
  ```bash
  ./matrixmult <matrix_A_file> <matrix_W_file> <matrix_B_file> <correct_vector_file>
  ```

## General Usage Notes

- Ensure the executables are in the same directory or adjust paths accordingly.
- Input files should follow specified formats, with elements separated by spaces and rows by new lines.
- Test files are provided in respective directories to verify functionality and performance.

## Testing and Output

Each project comes with its specific testing instructions. Generally, test by running the provided executable with sample input files and check outputs against expected results. Output files or console outputs will include results from computations or relevant error messages.

## Contributions and Issues

Contributions to the projects are welcome. Please follow standard procedures for submitting issues or pull requests on GitHub.

## Additional Information

Each project is designed for Linux/Unix environments and might require modifications for other operating systems. For detailed information about project structure and functionalities, refer to the inline comments in the source code files.
