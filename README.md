# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Use LU decomposition to factorize the coefficient matrix A into two matrices L(lower triangular) and U (Upper Triangular)
   
2. Solve for Y in LY=B

3.Solve for X in UX=Y

4. The solution matrix X contains the values of the variables that satisfies the system of linear equations.

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: D.B.V.SAI GANESH
RegisterNumber: 23009248
'''
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: D.B.V.SAI GANESH
RegisterNumber: 23009248
'''
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
import numpy as np
arr=eval(input())
constant=eval(input())
A=np.array(arr)
B=np.array(constant)
result=lu_factor(A)
solution=lu_solve(result,B)
print(solution)
```

## Output:
(i)
![Screenshot 2023-12-01 184010](https://github.com/saiganesh2006/LU-Decomposition/assets/145742342/c18f96f0-f1c6-45ed-9370-f5db4f918a4d)

(ii)
![Screenshot 2023-12-01 183930](https://github.com/saiganesh2006/LU-Decomposition/assets/145742342/a83d3b54-a16d-4fe7-bf71-38d260e2d95b)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

