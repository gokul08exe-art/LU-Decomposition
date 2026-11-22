# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program
2. Import the necessary libraries(numpy,scipy.linalg)
3. Define the matrix using numpy
4. Use lu(),lu_solve(),lu_factor() to get the solutions
5. End the program

## Program:
(i) To find the L and U matrix
'''
Program to find the L and U matrix.
Developed by:GOKULRAJ S 
RegisterNumber: 26015881
''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
P,L,U=lu(a)
print(L)
print(U)

(ii) To find the LU Decomposition of a matrix
'''
Program to find the LU Decomposition of a matrix.
Developed by: GOKULRAJ S
RegisterNumber: 26015881
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
lu,pivot=lu_factor(a)
x=lu_solve((lu,pivot),b)
print(x)

## Output:
<img width="1262" height="842" alt="image" src="https://github.com/user-attachments/assets/06485cf6-65d6-4f0b-baae-b24ac487397d" />

<img width="1417" height="757" alt="image" src="https://github.com/user-attachments/assets/5b0121c1-4f8c-425e-92c0-9bc543bb8a3f" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

