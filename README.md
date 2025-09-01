# Experiment-5
## AIM:  Write a python program for Binary Search and inspect for failures. 

## ALGORITHM
Start the program.
2. Get the list from the user
3. Get the element to be searched
4. Compare the mid element with the key, if same return the index
5. If key is greater, search it in the right side, else search it in the left side.
6. If not found return -1
7. Stop the program. 

## PROGRAM
#### NAME: SRIVATSAN G
#### REG NO: 212223230216
```
def binary_search(arr, x):  
    low = 0 
    high = len(arr) - 1 
    mid = 0 
    while low <= high: 
        mid = (high + low) // 2 
        if arr[mid] == x:
            return mid
        elif arr[mid] < x: 
            low = mid + 1 
        elif arr[mid] > x: 
            high = mid - 1 
        else: 
           return -1 
arr = [2,3,4,10,40] 
x = input("Enter the element to be searched: ");  
try: 
    x = int(x) 
    result = binary_search(arr, x)  
    if result != -1: 
          print("Element is present at index",str(result)) 
    else: 
          print("Element is not present in array") 
except: 
    print("Enter a valid input!")
```

## OUTPUT
<img width="684" height="262" alt="image" src="https://github.com/user-attachments/assets/a49dae4c-c67e-43dd-9990-7a242219d097" />

## RESULT
Thus, the python program of binary search is implemented and the output is verified 
successfully.
