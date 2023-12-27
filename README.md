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
Developed by:VEERARAGAVAN V
RegisterNumber: 23004739
'''
def selection_sort(nums):
    # write your code here using selection sort
    for i in range(len(nums)):
        lowest_value_index=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[lowest_value_index]:
                lowest_value_index=j
        nums[i],nums[lowest_value_index]=nums[lowest_value_index],nums[i]    
list_of_nums = eval(input())
# use the selection sort function
# print the sorted list
selection_sort(list_of_nums)
print(list_of_nums)
```
ii)	#Insertion Sort
```
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: VEERARAGAVAN V
RegisterNumber: 23004739
'''
def insertion_sort(nums):
    # Write your code here to sort the elements in the list using Insertion sort algorithm
    for i in range(1,len(nums)):
        items=nums[i]
        j=i-1
        while j>=0 and nums[j]>items:
            nums[j+1]=nums[j]
            j-=1
        nums[j+1]=items
    
list_of_nums = eval(input())
# use the insertion sort function to get the sorted list
# print the sorted list
insertion_sort(list_of_nums)
print(list_of_nums)
```

## Output:
![Screenshot 2023-12-27 225039](https://github.com/veerargavanv27/Sorting-Algorithm/assets/138955645/e9a4a585-8d16-46c4-b1f0-62ff96820f39)
![Screenshot 2023-12-27 225058](https://github.com/veerargavanv27/Sorting-Algorithm/assets/138955645/2ddca984-ddff-430c-a663-a48581a21076)


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
