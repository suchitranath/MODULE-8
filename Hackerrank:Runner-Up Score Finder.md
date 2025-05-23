# EX.No:8(D) Hackerrank:Runner-Up Score Finder in Python

## AIM:
To write a Python program that takes a list of scores from participants and finds the **runner-up score** (i.e., the second-highest score), eliminating any duplicates.


## ALGORITHM:

1. **Start**
2. Create a variable `n` and get its value from the user (number of participants)
3. Read the list of `n` scores from the user using `input().split()` and convert them to integers
4. Store the scores in a list
5. Use `set()` to remove any duplicate scores
6. Convert the set back to a list and sort it in ascending order
7. Print the second-last element of the sorted list (i.e., the runner-up score)
8. **Stop**


## PROGRAM:
```
# Dictionary with student names and their marks in five subjects
student_marks = { 
    'Alice': [85, 92, 78, 90, 88], 
    'Bob': [75, 80, 70, 85, 90], 
    'Charlie': [95, 85, 92, 88, 91], 
    'Daisy': [60, 65, 70, 58, 62], 
    'Ethan': [88, 82, 85, 87, 90] 
} 

# Dictionary to store total marks
total_marks = {} 

# Calculate total marks
for name, marks in student_marks.items(): 
    total = sum(marks) 
    total_marks[name] = total 

# Find the topper
topper = max(total_marks, key=total_marks.get) 
top_score = total_marks[topper] 

# Display results
print("Total Marks of Each Student:")
for name, total in total_marks.items(): 
    print(f"{name}: {total}") 

print(f"\nTopper: {topper}") 
print(f"Top Score: {top_score}")

```

## OUTPUT
![image](https://github.com/user-attachments/assets/d81bf401-c3db-4640-88b4-caca08e391e2)

## RESULT
Thus the program has been successfully executed 
