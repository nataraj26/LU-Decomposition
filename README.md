# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
 1. Import the module numpy and scipy to use the build-in functions for calculation
 2. Prepare lists from each linear equations and assign as an array
 3. Preform scipy.linalg.lu() to find the pivot table, lower triangle and upper triangle matrix
 4. End the program

## Program:
(i) To find the L and U matrix
```python
/*
Program to find the L and U matrix.
Developed by: NATARAJ KUMARAN S
RegisterNumber: 23003973
*/
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```python
/*
Program to find the LU Decomposition of a matrix.
Developed by: NATARAJ KUMARAN S
RegisterNumber: 23003973
*/
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv = lu_factor(A)
x = lu_solve((lu,piv),b)
print(x)
````

## Output:
(i) To find the L and U matrix
![Screenshot 2023-12-28 201408](https://github.com/nataraj26/LU-Decomposition/assets/147514615/53468c4b-daf5-45fb-9f0a-517a0fa9a483)
(ii) To find the LU Decomposition of a matrix
![Screenshot 2023-12-28 201819](https://github.com/nataraj26/LU-Decomposition/assets/147514615/7a1ea04d-a688-4faf-89a7-666324d4dbde)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

