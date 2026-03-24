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

# Input from user
num = int(input("Enter a number: "))

original = num
reverse = 0

# Reverse using loop
while num > 0:
    digit = num % 10
    reverse = reverse * 10 + digit
    num = num // 10

# Check palindrome
if original == reverse:
    print("Palindrome number")
else:
    print("Not a palindrome")

## Output
<img width="1919" height="978" alt="image" src="https://github.com/user-attachments/assets/87a1e7e4-c7ac-4708-9b9f-9ec520002709" />

## Result
