# Random-dice-generator
import random

print("--------Welcome to DICE GAME!-----------")

i=" "
scr = 0

while i != "no":
    x = int(input("Enter Number from (1-6): "))
    y = random.randint(1, 6)
    if x not in range(1, 6 + 1):
        print("Number must be between 1 to 6!")
    else:
        print(x, y)
        if x == y:
            scr += 5
    i = str(input("Do you want to continue? (Yes/no): "))

print("Game Exited!")
print("Your Score:", scr)
print("----Thanku for playing----")
