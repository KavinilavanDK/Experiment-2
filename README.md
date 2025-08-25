# Experiment-2
Write a program in Python language for Matrix multiplication fails. Introspect the causes for its failure and write down the possible reasons for its failure. 
## Aim
Write a python program for matrix multiplication and inspect for failures. 

## Algorithm
1.	Start the program.
2. Create empty list formatrix1, matrix2 and result.
3. Get the rows and columns count from the user.
4. Get the values of two matrix.
5. Perform matrix multiplication and store the answer in result.
6. Stop the program. 

## Program
Name: KAVI NILAVAN DK

Register number:212223230103
```
import numpy as np

r1 = int(input("Enter number of rows for Matrix A: "))
c1 = int(input("Enter number of columns for Matrix A: "))
print(f"Enter elements row by row ({r1}x{c1}):")
A = [list(map(int, input().split())) for _ in range(r1)]
A = np.array(A)

r2 = int(input("\nEnter number of rows for Matrix B: "))
c2 = int(input("Enter number of columns for Matrix B: "))
print(f"Enter elements row by row ({r2}x{c2}):")
B = [list(map(int, input().split())) for _ in range(r2)]
B = np.array(B)

if A.shape[1] != B.shape[0]:
    print("\nMatrix multiplication not possible!")
    print(f"Columns of A ({A.shape[1]}) != Rows of B ({B.shape[0]})")
else:
    result = np.matmul(A, B)
    print("\nResultant Matrix:")
    print(result)

```

## Output
<img width="1448" height="596" alt="image" src="https://github.com/user-attachments/assets/355cf89c-b078-4e4a-b06c-e61f42590e7f" />
<img width="864" height="504" alt="image" src="https://github.com/user-attachments/assets/f157f137-557e-455c-b1bb-33a2991be8e2" />


## Result
Thus the python program for Matrix multiplication is executed.
