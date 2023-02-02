# Day 3 Proyect - Treasure Island

https://replit.com/@sofiamejiamuro/treasure-island-start#main.py

```py
print("Welcome to Treasure Island.")
print("Your mission is to find the treasure.") 

#https://www.draw.io/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=Treasure%20Island%20Conditional.drawio#Uhttps%3A%2F%2Fdrive.google.com%2Fuc%3Fid%3D1oDe4ehjWZipYRsVfeAx2HyB7LCQ8_Fvi%26export%3Ddownload

#Write your code below this line 👇

question_1 = input("Do you wanna go Left or Right? ").lower()

if question_1 == "left":
  question_2 = input("Do you wanna Swim or Wait? ").lower()
  if question_2 == "wait":
    question_3 = input("Choose a door. Red, Yellow, Blue ").lower()
    if question_3 == "yellow":
      print("You Win!")
    elif question_3 == "blue":
      print("Eaten by beasts. Game Over.")
    elif question_3 == "red":
      print("Burned by fire. Game Over.")
    else: 
      print("Game Over.")
  else:
    print("Attacked by trout. Game Over.")
else:
  print("Fall into a hole. Game Over.")

``` 