# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: DHARSAN KUMAR R
RegisterNumber: 23014208
def selection_sort(array):
    for i in range(len(array)-1):
        current =i
        for j in range(i+1,len(array)):
            if(array[j]<array[current]):
                current=j
        array[i],array[current]=array[current],array[i]
    return array 
    
list_of_nums = eval(input())
x=selection_sort(list_of_nums)
print(x)

```
ii)	#Insertion Sort
```
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: DHARSAN KUMAR R
RegisterNumber: 23014208

def insertion_sort(array):
   for i in range (1,len(array)):
       j = i
       while array[j-1]>array[j] and j>0:
           array[j-1],array[j]=array[j],array[j-1]
           j-=1
           
   return array 
    
nums = eval(input()) 
print(insertion_sort(nums))

```

## Output:
![image](https://github.com/DHARSAN23014208/Sorting-Algorithm/assets/149365413/01453cf8-78a7-4a63-82d7-007110bcbdb6)
![image](https://github.com/DHARSAN23014208/Sorting-Algorithm/assets/149365413/45ae1b69-205f-4a81-9ade-5478acc55bac)


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
