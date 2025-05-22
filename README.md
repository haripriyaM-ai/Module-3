# MODULE - 3
# EXP 11: List Operations in Python: Sum of List Items

## Aim
To write a Python program that calculates the **sum of all elements** in a list.

## Algorithm
1. Define a list of numbers.
2. Use Python’s built-in `sum()` function to calculate the total.
3. Print the result.

##  Program

```
my_list=[]
for i in range(4):
    my_list.append(int(input()))
    
print(sum(my_list))
```

## Output
![image](https://github.com/user-attachments/assets/0e5bc1bd-503c-4ccb-afac-0feb4566e65d)

## Result
Thus, the program is verified successfully

---

# EXP 12: Regex in Python: Filter Words Without the Letter 'e'

## Aim
To write a Python program that filters out and returns all elements from a list **that do not contain the letter `'e'`**, using **regular expressions (regex)**.

## Algorithm
1. Import the `re` module.
2. Initialize an empty list `l1` to store results.
3. Define a list of words:  
   `items = ['goal', 'new', 'user', 'sit', 'eat', 'dinner']`
4. Iterate through each word in the list:
   - Use `re.search(r"e", i)` to check if the word contains `'e'`.
   - If **not**, append the word to `l1`.
5. Print the final filtered list.

## Program
```
import re

l1 = []
items = ['goal', 'new', 'user', 'sit', 'eat', 'dinner']

for i in items:
    if not re.search(r"e", i):
        l1.append(i)

print("Filtered list:", l1)

```
## Output
![image](https://github.com/user-attachments/assets/630b8ee1-0067-4691-941e-2dae28969da5)

## Result
Thus, the program is verified successfully

---

# EXP 13: Strings-Remove Nth Index Character from a String

## Aim
To write a Python program that accepts a string and removes the character at a specified index.

## Algorithm
1. Define a function named `remove` that takes the input string as an argument.
2. Read the index `n` from the user input.
3. Initialize an empty string `a` to store the new string.
4. Iterate over each index of the string using a `for` loop.
5. Check if the current index `i` is not equal to `n`.
6. If `i != n`, append the character at index `i` to string `a`.
7. After the loop, return the modified string `a`.
8. Print the final result.

## Program
```
def remove(s):
    n = int(input())
    a = ""
    for i in range(len(s)):
        if i != n:
            a += s[i]
    return a

s = input()
print("Modified string:", remove(s))
```
## Output
![image](https://github.com/user-attachments/assets/f3de0626-d504-4ec5-83e4-3e7c184c4d51)

## Result
Thus, the program is verified successfully

---

# EXP 14: Strings-Palindrome Check in Python (Without Built-in Functions)

## Aim
To write a Python program to check whether the string `"google"` is a **palindrome** or not, without using built-in palindrome checking functions.

## Algorithm
1. Assign the string `"google"` to a variable.
2. Reverse the string manually using slicing (`[::-1]`).
3. Compare the original string with the reversed string.
   - If they are equal, print that the string is a palindrome.
   - Otherwise, print that it is not a palindrome.
4. Execute the program.

## Program

```
s = "google"
rev = s[::-1]

if s == rev:
    print("The string is a palindrome.")
else:
    print("The string is not a palindrome.")
```

## Output
![image](https://github.com/user-attachments/assets/5a4b72f1-a245-45c4-9e11-9c9d1467b981)

## Result
Thus, the program is verified successfully.

---

# EXP 15: Tuple in Python: Check Element Existence

## Aim
To write a Python program that checks if the element `'n'` and the element `8` exist within a given tuple.

## Algorithm
1. Define a tuple `x` with some letters and numbers.
2. Use the `in` operator to check if the string `'n'` exists within the tuple.
3. Use the `in` operator to check if the integer `8` exists within the tuple.
4. Print the results.

## Program
```
x=('H','popcorn',8,19,'rice')
n=input()
print(n in x)
print(8 in x)
```

## Output
![image](https://github.com/user-attachments/assets/6346825a-292a-4d8b-863f-1bc201b4399d)

## Result
Thus, the program is verified successfully.
