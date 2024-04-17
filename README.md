# Linear Search and Binary search
## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Linear Search:
1.	Start from the leftmost element of array[] and compare k with each element of array[] one by one.
2.	If k matches with an element in array[] , return the index.
3.	If k doesn’t match with any of elements in array[], return -1 or element not found.
## Binary Search:
1.	Set two pointers low and high at the lowest and the highest positions respectively.
2.	Find the middle element mid of the array ie. arr[(low + high)/2]
3.	If x == mid, then return mid.Else, compare the element to be searched with m.
4.	If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.
5.	Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.
6.	Repeat steps 2 to 5 until low meets high
## Program:
i)	#Use a linear search method to match the item in a list.
```
#Program to find the match by linear search method
#Developed by: Mahalakshmi R
#Register Number: 212223230116
def linearsearch(a,b,array):
    for i in range(0,b):
        if array[i]==a:
            return i
    return -1
array=eval(input())
a=int(input())
b=len(array)
array.sort()
result=linearsearch(a,b,array)
if(result==-1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)
```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```
#Program to find the element in a list using Binary Search(Iterative Method).
#Developed by: Mahalakshmi R
#Register Number: 212223230116
def binarySearchIter(array, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
array = eval(input())
array.sort()
k = eval(input()) 
print(array)
res=binarySearchIter(array,k,0,len(array)-1)
if res==-1:
    print("Element not found")
else:
    print("Element found at index: ",res)
```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
#Program to find the element in a list using Binary Search (recursive Method).
#Developed by: Mahalakshmi R
#Register Number: 212223230116
def binarySearchIter(array, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
array = eval(input())
array.sort()
k = eval(input()) 
print(array)
res=binarySearchIter(array,k,0,len(array)-1)
if res==-1:
    print("Element not found")
else:
    print("Element found at index: ",res)
```
## Sample Input and Output
![image](https://github.com/Mahalakshmi230/Search-Algorithms/assets/149365324/dce3d10b-dfb9-4926-973a-b2510d746d2a)
![image](https://github.com/Mahalakshmi230/Search-Algorithms/assets/149365324/09418816-405d-41c5-8e71-cfca0a128888)
![image](https://github.com/Mahalakshmi230/Search-Algorithms/assets/149365324/4a323ba3-d2b8-44aa-8215-b21e1a778bb0)

## Result
Thus the linear search and binary search algorithm is implemented using python programming.
