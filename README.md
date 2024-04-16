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

'''
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: Gokul C
Register Number: 212223240040
'''

num=eval(input())
for i in range(len(num)):
    low=i
    for j in range(i+1,len(num)):
        if num[j]<num[low]:
            low=j
    num[i],num[low]=num[low],num[i]
print(num)

```
ii)	#Insertion Sort
```

'''
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: Gokul C
Register Number: 212223240040
'''

num=eval(input())
for i in range(1,len(num)):
    insert=num[i]
    j=i-1
    while j>=0 and num[j]>=insert:
        num[j+1]=num[j]
        j=j-1
    num[j+1]=insert
print(num)

```

## Output:

![Screenshot 2024-04-16 172506](https://github.com/Gokul1410/Sorting-Algorithms/assets/153058321/26ef2f90-5532-4c27-bc95-9b41c8d062ec)
![Screenshot 2024-04-16 172517](https://github.com/Gokul1410/Sorting-Algorithms/assets/153058321/82e9566c-570c-4de3-9d62-71f52ca91f04)
![Screenshot 2024-04-16 172532](https://github.com/Gokul1410/Sorting-Algorithms/assets/153058321/079296c1-d0d1-4d51-a090-ad90158dbdbb)
![Screenshot 2024-04-16 172544](https://github.com/Gokul1410/Sorting-Algorithms/assets/153058321/70985686-7710-4781-9091-3553b8253ef8)

## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
