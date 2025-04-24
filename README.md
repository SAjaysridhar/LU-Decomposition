# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
Step 1: <br>
Import library numpy and scipy.linalg.<br>
Step 2: <br>
Input the matrix/martices using eval(input()).<br>
Step 3:<br>
Perform LU decomposition using lu() or solve equations using lu_factor() and lu_solve().<br>
Step 4: <br>
Print the results L and U matrices or solution X matrix.<br>
## Program:

(i) To find the L and U matrix<br>

'''Program to find L and U matrix using LU decomposition.<br>
Developed by  : AJAY S <br>
RegisterNumber: 212224230010<br>
'''

import numpy as np<br>
from scipy.linalg import lu<br>
A = np.array(eval(input()))<br>
P,L,U=lu(A)<br>
print(L)<br>
print(U)<br>


(ii) To find the LU Decomposition of a matrix<br>


'''Program to solve a matrix using LU decomposition.<br>
Developed by  : AJAY S<br>
RegisterNumber: 212224230010<br>
'''

import numpy as np<br>
from scipy.linalg import lu_factor,lu_solve<br>
A=np.array(eval(input()))<br>
b=np.array(eval(input()))<br>
lu,piv=lu_factor(A)<br>
X=lu_solve((lu,piv),b)<br>
print(X)<br>


## Output:
(i) L and U matrix:
![Screenshot 2025-04-24 212221](https://github.com/user-attachments/assets/49c0d6fb-397f-458d-82cb-f961efc47f5d)

(ii) LU Decomposition of a matrix:
![Screenshot 2025-04-24 212237](https://github.com/user-attachments/assets/b94db798-d885-4c08-b3b8-1413bf7e5a60)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

