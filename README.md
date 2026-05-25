# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the NumPy module to use built-in linear algebra functions.
2. Create the matrix using np.array() and store it in a variable A.
3. Using the np.linalg.eig(), we get two results (first is eigenvalue and second is eigenvector) of the given matrix.
4. Print the eigenvalues and eigenvectors to display the result.

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: K DARREN JOSEPH
RegisterNumber: 212225230039
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
matrix = np.array(eval(input()))
P,L,U=lu(matrix)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: K DARREN JOSEPH
RegisterNumber: 212225230039
'''

# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
matrix= np.array(eval(input()))
constant= np.array(eval(input()))
piv,lu= lu_factor(matrix)
result= lu_solve((piv,lu),constant)
print(result)
```

## Output:
<img width="1123" height="404" alt="image" src="https://github.com/user-attachments/assets/502ffacd-ec84-4aec-9d7e-c9470cf2dd0d" />
<img width="820" height="169" alt="image" src="https://github.com/user-attachments/assets/32d08888-da43-4717-8255-b37e3e43acaf" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

