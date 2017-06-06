
# Lab 10 :Matrix Multiplication

[TOC]

## Problem statement 

  Write a Python Program to implement Matrix Multiplication

  Sample Input0    : [[1, 2], [1, 2]], [[1, 2], [1, 2]]
  Sample Output0   : [[3, 6], [3, 6]]

  Sample Input1    : [[1, 1], [1, 1]], [[1, 2, 1], [1, 2, 1]]
  Sample Output1   : [2, 4, 2], [2, 4, 2]

  Sample Input2    : [[1, 1], [1, 1]], [[1, 2], [1, 2], [1, 2]]
  Sample Output2   : Cannot multiply the matrices. Incorrect dimensions.	




## Solution Key

```python 

def matrixmulti(X, Y):
    result = [[0 for col in range(len(Y[0]))] for row in range(len(X))]

    if  len(X[0]) != len(Y):
        print ("Cannot multiply the matrices. Incorrect dimensions.")
        return

    for i in range(len(X)):
        for j in range(len(Y[0])):
            for k in range(len(Y)):
                result[i][j] += X[i][k] * Y[k][j]
    
    return result



```


## CloudCoder Exercise 




## Related material 





## Pre-Lab Questions 



## Post-lab Questions


## Bonus 1 

## Related Material 

### PPT Slides showing the Recursive Calls 

### Recursion vs Iteration

### CD Link : http://10.100.8.8/kata/edit/3A77017D5C?avatar=dolphin