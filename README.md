# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Doolittle (L diagonal = 1)
2.Crout (U diagonal = 1)
3.LUP (with pivoting, more stable)
4.Cholesky (special case for symmetric matrices)

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: vignesh s
RegisterNumber: 212225040489
*/
```
import os
os.environ["OPENBLAS_NUM_THREADS"] = "1"

import numpy as np
from scipy.linalg import lu

matrix = np.array(eval(input()))
P, L, U = lu(matrix)

print(L)
print(U)
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: vignesh s 
RegisterNumber: 212225040489
*/
```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
matrix= np.array(eval(input()))
constant= np.array(eval(input()))
piv,lu= lu_factor(matrix)
result= lu_solve((piv,lu),constant)
print(result)

## Output:

![alt text](<Screenshot 2026-05-30 140658.png>)
![alt text](<Screenshot 2026-05-30 140702.png>)
![alt text](<Screenshot 2026-05-30 140707.png>)
![alt text](<Screenshot 2026-05-30 140713.png>)
## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

