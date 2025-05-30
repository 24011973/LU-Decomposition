LU Decomposition
AIM:
To write a program to find the LU Decomposition of a matrix.

Equipments Required:
Hardware – PCs
Anaconda – Python 3.7 Installation / Moodle-Code Runner
Algorithm
(1) To Find The L and u matrix
Import NumPy and lu from scipy.linalg.
Read matrix input from the user using input() and convert it into a NumPy array.
Perform LU decomposition using lu() function and store the result in P, L, U.
Print the lower triangular matrix L.
Print the upper triangular matrix U.
(2) To Find The L and u matrix
Import NumPy and the functions lu_factor and lu_solve from scipy.linalg.
Read matrix A (coefficient matrix) from the user and convert it into a NumPy array.
Read matrix or vector B (right-hand side of the equation Ax = B) from the user and convert it into a NumPy array.
Perform LU factorization of matrix A using lu_factor(A).This returns lu (combined LU decomposition) and piv (pivot indices).
Solve the linear system using lu_solve((piv, lu), B) and store the result.
Print the solution vector or matrix.
Program:
(i) To find the L and U matrix

/*
Program to find the L and U matrix.
Developed by: ethicvaran
RegisterNumber: 212224230072
*/
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
(ii) To find the LU Decomposition of a matrix

/*
Program to find the LU Decomposition of a matrix.
Developed by: ethicvaran
RegisterNumber: 212224230072
*/
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)
Output:
(i)to find L and U matrix using LU decomposition:
![Screenshot 2025-05-30 114520](https://github.com/user-attachments/assets/3107b04c-7dc1-4792-a15c-b1021edfb296)
(ii)to solve a matrix using LU decomposition.
![Screenshot 2025-05-30 114525](https://github.com/user-attachments/assets/b7cf5d70-f484-4871-87cb-b4b365cf2e0f)


Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.
