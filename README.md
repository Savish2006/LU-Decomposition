# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### (i) To find the L and U matrix
### Step 1:
Import the necessary libraries: NumPy as np and lu from SciPy's linalg module.
### Step 2:
Take matrix input from the user, convert it into a NumPy array A using eval(input()).
### Step 3:
Perform LU decomposition on matrix A to obtain matrices P, L, and U using lu(A).
### Step 4:
Print the lower triangular matrix L and the upper triangular matrix U. 
### (ii) To find the LU Decomposition of a matrix.
### Step 1:
Import the required libraries: NumPy as np and lu_factor, lu_solve from SciPy's linalg module.
### Step 2:
Take matrix input A and vector input b from the user and convert them into NumPy arrays.
### Step 3:
Compute the LU decomposition of matrix A using lu_factor(A) and store the LU matrix and pivot indices.
### Step 4:
Solve the system of linear equations Ax = b using lu_solve((lu, piv), b) and print the solution vector X.




## Program:
```
(i) To find the L and U matrix
'''Program to find L and U matrix using LU decomposition.
Developed by: SAVISH R
RegisterNumber: 212224230257
'''
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
(ii) To find the LU Decomposition of a matrix
'''Program to solve a matrix using LU decomposition.
Developed by: SAVISH R
RegisterNumber: 212224230257
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),B)
print(X)
```
## Output:
(i) To find the L and U matrix
![image](https://github.com/user-attachments/assets/82f5e7f2-8dd8-4fb9-8d6d-5cd2639f6068)
(ii) To find the LU Decomposition of a matrix
![image](https://github.com/user-attachments/assets/7a1646d8-0ad7-417b-8fea-9ddfa271529c)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

