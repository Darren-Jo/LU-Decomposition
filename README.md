# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Read the given square matrix A of order n×n.
2. Initialize two matrices:

 - Lower triangular matrix L with diagonal elements as 1.
 - Upper triangular matrix U with all elements as 0
3. Compute the elements of U row-wise and the elements of L column-wise using LU decomposition formulas. 
4. Display the matrices L and U such that A=LU.

## Program:
(i) To find the L and U matrix
```
/*
Program to find L and U matrix using LU decomposition.
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
/*
Program to find the LU Decomposition of a matrix.
Developed by: K DARREN JOSEPH
RegisterNumber: 212225230039
*/
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
<img width="1090" height="394" alt="image" src="https://github.com/user-attachments/assets/69454855-0975-4200-9416-5527453fa21e" />
<img width="843" height="167" alt="image" src="https://github.com/user-attachments/assets/69302407-5985-4dad-9786-2d10aec6ac76" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

