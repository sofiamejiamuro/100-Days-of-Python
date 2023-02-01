### Day 2 - 013023

Data Types [Replit](https://replit.com/@sofiamejiamuro/day-2-start#main.py)


```py
#Data Types

#Subscripting
print("Hello"[0])

#Strings
#Numbers - Float and Integers
#Boolean
```

Function 

type()

### Type convertion - type casting

str() 

[Challenge](https://app.codingrooms.com/w/KoiNGHzVuxYb)

```py
# 🚨 Don't change the code below 👇
two_digit_number = input("Type a two digit number: ")
# 🚨 Don't change the code above 👆


####################################
#Write your code below this line 👇
print(int(two_digit_number[0]) + int(two_digit_number[1]))
```

### Mathematical operators

PEMDASLR

- Parenthesis
- Exponents
- Multiplication
- Division
- Addition 
- Subtraction

Calculation from left to right

[BMI Calculator](https://app.codingrooms.com/w/CIuBDpxpwc7Z)

```py
# 🚨 Don't change the code below 👇
height = input("enter your height in m: ")
weight = input("enter your weight in kg: ")
# 🚨 Don't change the code above 👆

#Write your code below this line 👇

weight_as_int = int(weight)
height_as_float = float(height)

# Using the exponent operator **
bmi = weight_as_int / height_as_float ** 2
# or using multiplication and PEMDAS
bmi = weight_as_int / (height_as_float * height_as_float)

bmi_as_int = int(bmi)

print(bmi_as_int)
```

### F strings

```py
f"string {variables}"
```

[Life in weeks challenge](https://app.codingrooms.com/w/Rz4NMmx0SVHp)

```py
# 🚨 Don't change the code below 👇
age = input("What is your current age? ")
# 🚨 Don't change the code above 👆

#Write your code below this line 👇

expected_life = 90
years_left = expected_life - int(age)
months_left = years_left*12
weeks_left = years_left*52
days_left = years_left*365

print(f"You have {days_left} days, {weeks_left} weeks, and {months_left} months left.")
```

