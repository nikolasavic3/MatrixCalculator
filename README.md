# Matrix Calcualtor

## Description
This Python script performs matrix multiplication on sparse matrices. It reads matrix data from an input file, multiplies the matrices, and saves the result to an output file.

## Features
- Reads sparse matrix data from an input file
- Performs matrix multiplication
- Handles sparse matrices efficiently
- Saves the result to an output file
- Prints matrix information and multiplication results to console

## Requirements
- Python 3.x
- Standard Python libraries (no external dependencies required):
  - sys

## Installation
1. Clone this repository:
   ```
   git clone https://github.com/nikolasavic3/MatrixMultiplication.git
   ```
2. Navigate to the project directory:
   ```
   cd MatrixMultiplication
   ```

## Usage
Run the script using Python with command-line arguments:
```
python matrix_multiplication.py <input_file>.txt <output_file>.txt
```
For example:
```
python matrix_multiplication.py input_matrices.txt output_result.txt
```

## Input File Format
The input file should contain the data for two matrices in the following format:
```
num_rows_1 num_columns_1
row_1 column_1 value_1
row_2 column_2 value_2
...
num_rows_2 num_columns_2
row_1 column_1 value_1
row_2 column_2 value_2
...
```
Where:
- `num_rows` and `num_columns` specify the dimensions of each matrix
- Each subsequent line represents a non-zero element in the matrix with its row, column, and value

## Output
The script will:
1. Print the input matrices to the console
2. Print the result of the matrix multiplication to the console
3. Save the result matrix to the specified output file

## Limitations
- The script assumes that matrix multiplication is possible (i.e., the number of columns in the first matrix equals the number of rows in the second matrix)
- The script is designed for sparse matrices and may not be efficient for dense matrices

## Future Improvements
- Add error handling for invalid input files or matrix dimensions
- Implement more matrix operations (addition, subtraction, etc.)
- Optimize for large sparse matrices
- Add support for floating-point values in matrices

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## License
This project is licensed under the MIT License - see the LICENSE.md file for details.

## Disclaimer
This tool is for educational and computational purposes only. For large-scale or production use, consider using optimized linear algebra libraries.
