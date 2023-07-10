# Linear Algebra Library for Matrices by @Keobkeig (Richie X.)
This is a JavaScript library for performing linear algebra operations on matrices. It provides a **Matrix** class with various methods to perform operations such as finding the trace, augmenting matrices into Gaussian elimination, performing matrix operations (addition, subtraction, multiplication), finding the inverse of matrices, checking for transpose and symmetry, and calculating areas of triangles and quadrilaterals.

# Matrix Class
## Properties
- **rows**: The number of rows in the matrix.
- **cols**: The number of columns in the matrix.
- **matrix**: The 2D array representing the matrix elements.
  
## Methods:
- populate(object): Populates the matrix with either zeros or values from the given object.
- toString(): Converts the matrix to a string representation.
- transpose(): Returns the transpose of the matrix.
- determinant(): Calculates the determinant of the matrix.
- trace(): Calculates the trace of the matrix (only for square matrices).
- add(matrix): Performs matrix addition with the given matrix.
- subtract(matrix): Performs matrix subtraction with the given matrix.
- multiply(matrix): Performs matrix multiplication with the given matrix.
- isSymmetric(): Checks if the matrix is symmetric.
- triangleArea(): Calculates the area of a triangle represented by the matrix.
- quadArea(): Calculates the area of a quadrilateral represented by the matrix.
- gaussElim(): Performs Gaussian elimination on the matrix.
- inverse(): Calculates the inverse of the matrix if it exists.
  
## Usage:
To use the library, create an instance of the Matrix class and pass the necessary parameters to initialize the matrix. Then, you can call the available methods to perform operations on the matrix.

Example usage:
```javascript
Copy code
// Create a 2x2 matrix
const matrix = new Matrix([[1, 2], [3, 4]]);

// Calculate the determinant
const determinant = matrix.determinant();
console.log("Determinant:", determinant);

// Calculate the trace
const trace = matrix.trace();
console.log("Trace:", trace);

// Add two matrices
const matrix2 = new Matrix([[5, 6], [7, 8]]);
const sum = matrix.add(matrix2);
console.log("Sum:", sum.toString());

// Calculate the area of a triangle
const triangle = new Matrix([[1, 2, 3], [4, 5, 6]]);
const area = triangle.triangleArea();
console.log("Triangle Area:", area);

// Calculate the area of a quadrilateral
const quad = new Matrix([[2, 1], [2, 3], [-2, 2], [-1, 0]]);
const quadArea = quad.quadArea();
console.log("Quadrilateral Area:", quadArea);
```

Please note that this library assumes valid inputs and may not handle all possible edge cases.
