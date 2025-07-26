# 🧠 Beginner Python Practice

Welcome to this beginner-friendly Python exercise repository!
This project is designed to help you strengthen your core programming skills by working through small but meaningful problems. These tasks cover essential Python topics including:

- Lists

- Strings

- Dictionaries

- Tuples

- Loops & Conditions

- Functions

- Input/Output

- Basic algorithmic thinking

Whether you're just starting out or reviewing the basics, this project is for you!

🎯 **Project Goals**

By the end of this project, you will be able to:

- Manipulate and transform data using lists, dictionaries, and tuples

- Write reusable functions

- Practice looping, conditional logic, and string manipulation

- Apply real-world thinking to common problem patterns

- Improve your understanding of Python syntax and logic step by step

🧠 **Problem-Solving Mindset (Step-by-Step Guide)**

Each exercise follows a logical approach that you can use when solving any Python problem:

1. Read & Understand the Problem
→ Identify the goal, keywords, and the expected input/output

2. Clarify Input and Output
→ Know the required data type and format clearly

3. Sketch a Quick Plan
→ Outline your solution idea briefly

4. Link Back to What You've Learned
→ Map your plan to Python knowledge: loops, conditions, etc.

5. Break Down the Problem
→ Think in smaller steps:

    - Looping through data

    - Checking conditions

    - Updating variables or collections

6. Write a Function Skeleton
→ Example: def function_name(params): ...

7. Implement Step-by-Step Logic
→ Code exactly what you planned using loop → condition → update flow

8. Test with Sample Inputs
→ Compare actual output with the expected one

9. Refactor if Needed
→ Improve readability, fix bugs, or optimize performance

# 📚 [**List of Exercises**](https://drive.google.com/file/d/1SOQ5xhdK-ieWegT4aIXgcnkpl_TDr7RN/view?usp=sharing)

## 🔢 Exercise 1: Given a list of numbers. write a program to turn every item of a list into its square.

Input: [1, 2, 3, 4, 5, 6, 7]

* Code

```ruby
numbers = [1, 2, 3, 4, 5, 6, 7]
sqr = []
for i in numbers:
    sqr.append(i ** 2)

print(sqr)
```

* Results

<img width="414" height="59" alt="image" src="https://github.com/user-attachments/assets/2c8e7e9b-a59c-48bc-a08b-7ca428a50bb7" />

## 🔍 Exercise 2: Display numbers which are both divisible by 3 and not divisible by 5 from a list.

Input: [10, 20, 33, 46, 54, 60]

* Code

```ruby
num_list = [10, 20, 33, 46, 54, 60]
print("Given list:", num_list)
print("Numbers divisible by 3 but not by 5:")
for num in num_list:
    if num % 3 == 0 and num % 5 != 0:
        print(num)
```

* Results

<img width="488" height="123" alt="image" src="https://github.com/user-attachments/assets/5a17faff-8742-46b8-bfa6-7d0c12c2f225" />

## 🧱 Exercise 3: Convert two lists (with same size) into a dictionary 

Input: keys = ['Ten', 'Twenty', 'Thirty']; values = [10, 20, 30]

* Code

```ruby
keys = ['Ten', 'Twenty', 'Thirty']
values = [10, 20, 30]

result = dict(zip(keys, values))
print(result)
```

* Results

<img width="552" height="54" alt="image" src="https://github.com/user-attachments/assets/28f54e00-2ae9-4e4f-b5a9-3dc7a69c713b" />

## 📍 Exercise 4: Write a program to accept a string from the user and display characters that are present at an odd index number. 

For example, str = "unigap" so you should display 'n', 'g', 'p'. 

* Code

```ruby
# accept input string from a user
word = input('Enter word: ')
print("Original String:", word)

# get the length of a string
size = len(word)

# iterate a each character of a string
# start: 0 to start with first character

# step: 2 to get the characters present at odd index like 1, 3, 5
print("Printing only even index chars")
for i in range(1, size, 2):
    print("index[",i,"]", word[i])
```

* Results

<img width="537" height="164" alt="image" src="https://github.com/user-attachments/assets/c0b275fa-f867-4923-af69-0d9b3a5f5145" />

## 🔁 Exercise 5: Reverse a given integer number 

Given: 65869

* Code

```ruby
num = int(input('Given Number: '))
reverse_number = 0
while num > 0:
    reminder = num % 10
    reverse_number = (reverse_number * 10) + reminder
    num = num // 10
print("Reverse Number:", reverse_number)
```

* Results

<img width="552" height="72" alt="image" src="https://github.com/user-attachments/assets/7dc50ab4-a9a2-4c1c-8cb7-bbabb5a8d964" />

## ➕ Exercise 6: Calculate the sum of all numbers from 5 to a given number

Write a program to accept a number from a user and calculate the sum of all numbers from 5 to a given number.

For example, if the user entered 10 the output should be equal 5+6+7+8+9+10 = 45

* Code

```ruby
# s: store sum of all numbers
s = 0
n = int(input("Enter number "))
# run loop n times
# stop: n+1 (because range never include stop number in result)
for i in range(5, n + 1, 1):
    # add current number to sum variable
    s += i
print("\n")
print("Sum is: ", s)
```

* Results

<img width="478" height="125" alt="image" src="https://github.com/user-attachments/assets/2d008d51-6b31-4aac-8d5b-2404d1bd9372" />

## 💰 Exercise 7: Calculate income tax for the given income by adhering to the below rules.

<img width="891" height="368" alt="image" src="https://github.com/user-attachments/assets/51a75cfd-c7e0-494b-9b11-cc6e0ddf18c1" />

For example, suppose the taxable income is 45000 the income tax payable is

10000x0% + 10000x10% + 25000x20% = $6000.

* Code

```ruby
income = 45000
tax_payable = 0
print("Given income", income)

if income <= 10000:
    tax_payable = 0
elif income <= 20000:
    # no tax on first 10,000
    x = income - 10000
    # 10% tax
    tax_payable = x * 10 / 100
else:
    # first 10,000
    tax_payable = 0

    # next 10,000 10% tax
    tax_payable = 10000 * 10 / 100

    # remaining 20%tax
    tax_payable += (income - 20000) * 20 / 100

print("Total tax to pay is", tax_payable)
```

* Results

<img width="560" height="77" alt="image" src="https://github.com/user-attachments/assets/1559a3a0-ca00-44ce-a494-63fedf18020d" />

## 🔢 Exercise 8: Convert a given tuple of integers into a new tuple which contains cube of each element of the original tuple.

For example, if the original tuple is (1,2,3,4), the expected output is (1,8,27,64)

* Code

```ruby
def sqr_tuple(original_tuple):
    sqr_list = [x**3 for x in original_tuple]
    sqr_tuple = tuple(sqr_list)
    return sqr_tuple
sqr_tuple((1,2,3,4))
```

* Results

<img width="415" height="60" alt="image" src="https://github.com/user-attachments/assets/54c7c848-b171-4b62-9e3d-1944cb2cdb4d" />

## 🔍 Exercise 9: Determine the number of even, odd, and divisible by 3 in a list (using Def) 

Input: list_num = [1,2,3,4,5,6,7]

* Code

```ruby
def even_num(a):
    even_num = 0
    for i in a:
        if i % 2 == 0:
            even_num += 1
    print("total even num is:", even_num)

def odd_num(a):
    odd_num = 0
    for i in a:
        if i % 2 != 0:
            odd_num += 1
    print("total odd num is:", odd_num)

def div_3_num(a):
    div_3 = 0
    for i in a:
        if i % 3 == 0:
            div_3 += 1
    print("total num divisible by 3 is:", div_3)


list1 = [1,2,3,4,5,6,7]
even_num(list1)
odd_num(list1)
div_3_num(list1)
```

* Results

<img width="511" height="104" alt="image" src="https://github.com/user-attachments/assets/e45c246a-5420-48ca-a8b6-0acf4bb79adb" />

## 🔐 Exercise 10: Given a sequence of characters to be considered a password. Check if the password is valid or not.

A password is valid if and only if all of the following conditions are satisfied:

- At least 1 lowercase letter [a-z]
- At least 1 number [0-9]
- At least 1 uppercase letter [A-Z]
- At least 1 symbol in [$ @ #]
- Minimum password length: 6
- Maximum password length: 12

* Code

```ruby
A = input('Your password is ')
def valid_pass(password):
  total_lower = 0
  total_upper = 0
  total_number = 0
  total_special = 0
  for i in A:
      if i.islower():
          total_lower +=1
      if i.isupper():
          total_upper +=1
      if i >='0'and i <='9':
          total_number +=1
      if i in ['$','@','#']:
          total_special +=1

  if total_lower >= 1 and total_upper >=1 and total_number >=1 and total_special >=1 and len(A)>=6 and len(A)<= 12:
      print("valid password")
  else:
      print("invalid password")
valid_pass(A)
```

* Results

<img width="555" height="81" alt="image" src="https://github.com/user-attachments/assets/d0fa75b0-8062-4bd8-8bd1-1a03f44be01c" />

## 🧼 Exercise 11: Write a program that will be able to remove duplicates from a given array.

The output should meet the following requirements:

- Sorted in ascending order

- Leading and trailing spaces removed

- Duplicates removed

- Each element's first character is uppercase.

Input: ["Panasonic ", " pensonic", "panasonic ", " Haier", "electrolux","Electrolux"]

* Code

```ruby
l = ["Panasonic ", " pensonic", "panasonic  ", " Haier", "electrolux","Electrolux"]
print("Original string: ",l)
for i in range(len(l)):
    l[i] = l[i].strip().capitalize()
l = sorted(l)
l = list(dict.fromkeys(l))
l = [i.replace(", ","") for i in l]

print("Output: ", l)
```

* Results

<img width="1132" height="80" alt="image" src="https://github.com/user-attachments/assets/0a452586-68fb-4d71-a79e-c5ec64070df7" />

🤝 Contributing
This is an open project to help beginners learn Python through practical examples.
Feel free to fork the repository, submit pull requests with new exercises, or suggest improvements.

