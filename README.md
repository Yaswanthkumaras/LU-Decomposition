![image](https://github.com/user-attachments/assets/672c9dd2-5ba0-485c-bc20-0d7d7040cafc)# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
(i)

 Step 1: Import the numpy module to use the built-in functions for calculation

Step 2: From the scipy module, import lu to use the built-in function lu for calculation

Step 3: Get the input list from the user

Step 4: Using the lu(), we get three results (first is pivot, second is l matrix and the third is the u matrix)

Step 5: End the program

(ii)

Step 1: Import the numpy module to use the built-in functions for calculation

Step 2: From the scipy module, import lu_factor and lu_solve to solve the matrix

Step 3: Get the input lists from the user

Step 4: Using the lu_factor(), we get two results (first is the lu matrix and second is the pivot)

Step 5: Using the lu_solve(), we find the solution for the given matrix using lu decomposition

Step 6: End the program

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by:yaswanth kumar 
RegisterNumber:24900588
*/
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: yaswanth kumar
RegisterNumber: 24900588
*/
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,piv=lu_factor(A)
x=lu_solve((lu,piv),B)
print(x)
```

## Output:
![Screenshot 2024-12-04 203709](https://github.com/user-attachments/assets/efe10032-0ead-4dfd-882a-a52bcdbf5dcc)
![Screenshot 2024-12-04 204445](https://github.com/user-attachments/assets/d6ddfa96-bb61-4b6f-a5e7-747719f59e91)




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

