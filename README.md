## DATE:
## EX NO 8: Selection sort and Insertion sort
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

i)	Selection Sort
```
#Developed by: MONISH N  
#RegisterNumber: 212223240097
def selection_sort(nums):
    for i in range(len(nums)):
        lowest = i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[lowest]:
                lowest = j
        nums[i],nums[lowest] = nums[lowest], nums[i]
    
list_of_nums = eval(input())
selection_sort(list_of_nums)
print(list_of_nums)
```
ii)	Insertion Sort

```
#Developed by: MONISH N 
#RegisterNumber: 212223240097
def insertion_sort(nums):
    for i in range(1,len(nums)):
        item = nums[i]
        j = i-1
        while j>=0 and nums[j]>item:
            nums[j+1]=nums[j]
            j -=1
        nums[j+1] = item
    
list_of_nums = eval(input())
insertion_sort(list_of_nums)
print(list_of_nums)
```

## Output:

### i)
![Screenshot 2024-10-16 092908](https://github.com/user-attachments/assets/90f7b7d2-687b-4b68-ad77-eb50bdd71566)

### ii)
![Screenshot 2024-10-16 093039](https://github.com/user-attachments/assets/1a632acb-5efd-42e5-8d35-1f87d32157cb)


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
