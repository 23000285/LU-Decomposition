# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
## (1) To find the L and U matrix 
1. Import numpy library and import lu from scipy.linalg 
2. Obtain input and perform LU decomposition 
3. Print the lower triangular matrix L 
4. Print the upper triangular matrix U

## (2)To find the LU Decomposition of a matrix 
1.Import numpy library and import lu from scipy.linalg 
2.Obtain input and factorize 
3.Get right-hand side vector 
4.Solve the system and print the solution

## Program:
## (i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: VENKATANATHAN P R
RegisterNumber: 23000285
'''
#To print L and U matrix
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
## (ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: VENKATANATHAN P R
RegisterNumber: 23000285
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(a)
x=lu_solve((lu,piv),b)
print(x)

```

## Output:
![image](https://github.com/23000285/LU-Decomposition/assets/138970859/d094cc7c-0a9a-4f20-984a-d52ba8c44ef6)

![image](https://github.com/23000285/LU-Decomposition/assets/138970859/d5583014-7c06-468f-ad11-ababf6931b72)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

