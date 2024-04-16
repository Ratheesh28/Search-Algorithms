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
a=eval(input())
b=int(input())
a.sort()
print(a)
def linsc(a,b):
    k=0
    for i in a:
        if(b==i):
           return 1,k
        else:
           k+=1
    return -1,k
d,k=linsc(a,b)
if(d==1):
    print("Element found at index: ",k)
else:
    print("Element not found")
```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```
lst=eval(input())
n=int(input())
lst.sort()
low=0
high=len(lst)-1
print(lst)
def binsc(lst,n,low,high):
    while(low<=high):
        mid=low+(high-low)//2
        if(lst[mid]==n):
            return 1,mid
        elif(n>lst[mid]):
            low=mid+1
        else:
            high=mid-1
    return -1,mid
d,mid=binsc(lst,n,low,high)
if(d==1):
    print("Element found at index: ",mid)
else:
    print("Element not found")
```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
a=eval(input())
b=int(input())
a.sort()
print(a)
def linsc(a,b):
    k=0
    for i in a:
        if(b==i):
           return 1,k
        else:
           k+=1
    return -1,k
d,k=linsc(a,b)
if(d==1):
    print("Element found at index: ",k)
else:
    print("Element not found")
```
## Sample input and Output
![alt text](<WhatsApp Image 2024-04-16 at 23.29.08_96df4d90.jpg>)
![alt text](<WhatsApp Image 2024-04-16 at 23.30.17_b8a369c6.jpg>)
![alt text](<WhatsApp Image 2024-04-16 at 23.30.40_9cc42571.jpg>)



## Result
Thus the linear search and binary search algorithm is implemented using python programming.
