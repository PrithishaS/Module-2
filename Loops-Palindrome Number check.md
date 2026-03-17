## Loops in Python: Palindrome Number Checker

## 🎯 Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

## 🧠 Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## 🧾 Program

# Reg.No: 212222210020
# Name: Prithisha S

n = int(input("Enter number of rows: "))

for i in range(n):
    num = 1
    for j in range(n - i):
        print(" ", end="")
    for j in range(i + 1):
        print(num, end=" ")
        num = num * (i - j) // (j + 1)
    print()
    
## Output

Enter number of rows: 5
     1
    1 1
   1 2 1
  1 3 3 1
 1 4 6 4 1

## Result
The programs were executed successfully and the expected outputs were obtained.
