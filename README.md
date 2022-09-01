# rock-paper-scissors
import random


def game(com, you):
    if com == 'r':
        if you == 'p':
            return True
        elif you == 's':
            return False
    elif com == 'p':
        if you == 's':
            return True
        elif you == 'r':
            return False
    elif com == 's':
        if you == 'r':
            return True
        elif you == 'p':
            return False
    elif com == you:
            return None


RandInt = random.randint(1, 3)
print("computer turn rock(r),paper(P),scrissor(s)")
if RandInt == 1:
    com = 'r'
if RandInt == 2:
    com = 'p'
if RandInt == 3:
    com = 's'

you = input("enter your turn rock,paper,scissors ")
b = game(com, you)
print(f"computer turn is  {com}")
print(f"your turn is  {you}")

if b ==None:
    print("game is tie")
elif b :
    print("win")
else:
    print("lose")
