# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program and read the order of the square matrix.
2.Initialize the lower triangular matrix (L) as an identity matrix and upper triangular matrix (U) as a zero matrix.
3.Calculate the elements of L and U using the LU decomposition method.
4.Display the L and U matrices and stop the program. 

## Program:
(i) To find the L and U matrix
'''Program to find L and U matrix using LU decomposition.
Developed by: lavanya s
RegisterNumber: 26012000
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

(ii) To find the LU Decomposition of a matrix
'''Program to solve a matrix using LU decomposition.
Developed by: harithra s
RegisterNumber: 26012000
'''
# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,pivot=lu_factor(A)
x=lu_solve((lu,pivot),B)
print(x)

## Output:
<img width="683" height="680" alt="Screenshot 2026-11-23 093918" src="https://github.com/user-attachments/assets/341d032b-4876-40f2-bd6b-c714810a8117" />
<img width="967" height="403" alt="Screenshot 2026-11-23 093932" src="https://github.com/user-attachments/assets/e4bc5aa0-9536-489c-afd7-47b039d94dc5" />
<img width="1218" height="858" alt="Screenshot 2026-11-23 094042" src="https://github.com/user-attachments/assets/226f8dce-ee66-470e-a934-2c09c361d663" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

