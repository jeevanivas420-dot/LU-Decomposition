# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program.
2. Import required libraries (numpy, scipy.linalg).
3. Read the input matrix A from the user.
4. Apply LU decomposition using the lu() or lu_factor() function.
5. Separate the matrices into L (Lower triangular) and U (Upper triangular).
6. If solving AX = B:
Read matrix/vector B.
Use lu_solve() to find solution X.
7. Display the matrices L, U (and solution X, if required).
8. Stop the program.

## Program:
(i) To find the L and U matrix

**Program to find the L and U matrix.**
**Developed by: JEEVA NIVAS M**
**RegisterNumber: 212225040148**
```
import numpy as np
from scipy.linalg import lu


A = np.array(eval(input()), dtype=float)

P, L, U = lu(A)

print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix

**Program to find the LU Decomposition of a matrix.**
**Developed by: JEEVA NIVAS M**
**RegisterNumber: 212225040148**
```
import numpy as np
from scipy.linalg import lu_factor, lu_solve

A = np.array(eval(input()), dtype=float)
B = np.array(eval(input()), dtype=float)

lu, piv = lu_factor(A)


X = lu_solve((lu, piv), B)

print(X)
```

## Output:
<img width="1218" height="559" alt="image" src="https://github.com/user-attachments/assets/d0158ef3-ff0f-4dc3-b396-6fb1e17d406a" />
<img width="1231" height="308" alt="image" src="https://github.com/user-attachments/assets/055e2ec6-4f7f-434d-a842-decdf6db3f0e" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

