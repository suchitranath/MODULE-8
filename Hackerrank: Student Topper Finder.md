# EX.No:8(A)  Hackerrank:# 🏆 Student Topper Finder

This Python program helps determine the **top-performing student** based on the total marks across five subjects. It uses a dictionary to store each student’s marks and identifies the topper using simple calculations and built-in functions.

## Aim

To maintain a dictionary of students with their marks in five subjects, calculate their **total marks**, store them in a new dictionary, and identify the **student with the highest total (topper)**.


## Algorithm

1. **Start** the program.
2. Create a dictionary `student_marks`:
   - Keys → Student names.
   - Values → List of marks in five subjects.
3. Initialize an empty dictionary `total_marks`.
4. Loop through `student_marks`:
   - Calculate the total marks using `sum()`.
   - Store the result in `total_marks`.
5. Use `max()` on `total_marks` to find the student with the highest total.
6. Print:
   - The `total_marks` dictionary.
   - The **topper's name and score**.


##  PROGRAM:
```
l1 = []
l2 = []

for _ in range(int(input())):
    name = input()
    score = float(input())
    l1.extend([name, score])
    l2.append(l1)
    l1 = []

l3 = []
l4 = []

for i in l2:
    l3.append(i[1])

l3 = sorted(list(set(l3)))  # Removes duplicates and sorts the scores

for i in l2:
    if i[1] == l3[1]:  # Second lowest score
        l4.append(i[0])

l4.sort()

for i in l4:
    print(i)

```

## OUTPUT
![image](https://github.com/user-attachments/assets/c9736d5a-a7c0-409a-baef-433f82a8b950)

## RESULT
Thus the python program for finding the students with second lowest grade has been implemented and 
executed successfully. 
