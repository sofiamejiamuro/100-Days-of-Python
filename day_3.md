### Day 3 - 013023


**COMPARISION OPERATORS**

[Even or Odd challenge](https://app.codingrooms.com/w/WA0XL13tIp4W)

```py
# 🚨 Don't change the code below 👇
number = int(input("Which number do you want to check? "))
# 🚨 Don't change the code above 👆

#Write your code below this line 👇

if number%2 != 0:
    print("This is an odd number.")
else:
    print("This is an even number.")

```

**NESTED IF/ELSE**

[BMI challenge](https://app.codingrooms.com/w/Z0BtWrxHqeLw)
```py
# 🚨 Don't change the code below 👇
height = float(input("enter your height in m: "))
weight = float(input("enter your weight in kg: "))
# 🚨 Don't change the code above 👆

#Write your code below this line 👇

bmi = weight/(height ** 2)
#print(bmi)

if bmi < 18.5:
    print(f"Your BMI is {round(bmi,2)}, you are underweight.")
elif bmi < 25:
    print(f"Your BMI is {round(bmi,2)}, you have a normal weight.")
elif bmi < 30:
    print(f"Your BMI is {round(bmi,2)}, you are slightly overweight.")
elif bmi < 35:
    print(f"Your BMI is {round(bmi,2)}, you are obese.")
else:
    print(f"Your BMI is {round(bmi,2)}, you are clinically obese.")

```

[Leap Year Challenge](https://app.codingrooms.com/w/Xv6Pkwv6W9T6)

```py
# 🚨 Don't change the code below 👇
year = int(input("Which year do you want to check? "))
# 🚨 Don't change the code above 👆

#Write your code below this line 👇

if year%4 == 0:
    if year%100 != 0:
        print(f"Leap year.100")
    else:
        if year%400 == 0:
            print(f"Leap year 400" )      
else:
    print(f"Not leap year.1" )


# Refactor
if year%4 == 0:
    if year%100 == 0:
        if year%400 == 0:
            print(f"Leap year.")
        else:
            print(f"Not leap year." )
    else:
        print(f"Leap year." )      
else:
    print(f"Not leap year." )
```

**MULTIPLE IF** All if statements are excecuted

```py
print("Welcome to the rollercoaster!")
height = int(input("What is your height in cm? "))
bill = 0

if height >= 120:
  print("You can ride the rollercoaster!")
  age = int(input("What is your age? "))
  if age < 12:
    bill = 5
    print("Child tickets are $5.")
  elif age <= 18:
    bill = 7
    print("Youth tickets are $7.")
  else:
    bill = 12
    print("Adult tickets are $12.")
  
  wants_photo = input("Do you want a photo taken? Y or N. ")
  if wants_photo == "Y":
    bill += 3
  
  print(f"Your final bill is ${bill}")

else:
  print("Sorry, you have to grow taller before you can ride.")

```

(Pizza Order Challenge)[https://app.codingrooms.com/w/WPyj07c4v1Gb]

```py
# 🚨 Don't change the code below 👇
print("Welcome to Python Pizza Deliveries!")
size = input("What size pizza do you want? S, M, or L ")
add_pepperoni = input("Do you want pepperoni? Y or N ")
extra_cheese = input("Do you want extra cheese? Y or N ")
# 🚨 Don't change the code above 👆

#Write your code below this line 👇
final_bill = 0

if size == "L":
    final_bill = 25
    if add_pepperoni == "Y":
        final_bill = final_bill + 3
elif size == "M":
    final_bill = 20
    if add_pepperoni == "Y":
        final_bill = final_bill + 3
elif size == "S":
    final_bill = 15
    if add_pepperoni == "Y":
        final_bill = final_bill + 2

if extra_cheese == "Y":
    final_bill = final_bill + 1

print(f"Your final bill is: ${final_bill}")

# REFACTOR

final_bill = 0

if size == "L":
    final_bill = 25
elif size == "M":
    final_bill = 20
elif size == "S":
    final_bill = 15

if add_pepperoni == "Y":
    if size == "S":
        final_bill += 2
    else:
        final_bill += 2

if extra_cheese == "Y":
    final_bill += 1

print(f"Your final bill is: ${final_bill}")
```

**LOGICAL OPERATORS**

[tickets](https://replit.com/@sofiamejiamuro/day-3-end#main.py)

[Love Calculator Challenge](https://app.codingrooms.com/w/cB8Va9z69My8)

```py
# 🚨 Don't change the code below 👇
print("Welcome to the Love Calculator!")
name1 = input("What is your name? \n")
name2 = input("What is their name? \n")
# 🚨 Don't change the code above 👆

#Write your code below this line 👇

t = name1.lower().count("t") + name2.lower().count("t")
r = t + (name1.lower().count("r") + name2.lower().count("r"))
u = r + (name1.lower().count("u") + name2.lower().count("u"))
e = u +(name1.lower().count("e") + name2.lower().count("e"))

l = name1.lower().count("l") + name2.lower().count("l")
o = l + (name1.lower().count("o") + name2.lower().count("o"))
v = o + (name1.lower().count("v") + name2.lower().count("v"))
e_2 = v + (name1.lower().count("e") + name2.lower().count("e"))

total_true = e
total_love = e_2

print(total_true)
print(total_love)

total = int(str(total_true) + str(total_love))
#print(type(total))

if total < 10 or total > 90:
    print(f"Your score is {total}, you go together like coke and mentos.")
elif total >= 40 and total <= 50:
    print(f"Your score is {total}, you are alright together.")
else:
    print(f"Your score is {total}.")

#Refactor
# Concatenate the names from the beggining

names = name1 + name2

```

