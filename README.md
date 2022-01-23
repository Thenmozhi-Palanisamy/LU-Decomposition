# LU Decomposition without zero on the diagonal

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. calculate the elements of L and U
2. Print elements of L and u
3. find v by solving LV=b by forward substitution
4. find x by solving UX= v by a backward subsitution
5.print array X as the solution 

## Program:
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: THENMOZHI.P
RegisterNumber:21005219 
*/
```
...

import numpy as np
from scipy.linalg import lu
A=eval(input())
P,L,U=lu(A)
print(L)
print(U) 

import numpy as np
from scipy.linalg import lu_factor,lu_solve
A =eval(input())
B =eval(input())
lu,piv= lu_factor(A)
x= lu_solve((lu,piv),B)
print(x)

## Output:
![output](.//LU1.png)
![output](.//LU2.png)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

