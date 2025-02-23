Code for rock Scissor Paper:

import random
rock = """
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
"""

# Paper
paper = """
     _______
---'    ____)____
           ______)
          _______)
         _______)
---.__________)
"""

# Scissors
scissor = """
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
"""
choices=[rock,paper,scissor]
print("welocme to the rock paper scissor!!")
print("select the 0 for rock ,1 hand ,2 for scissor")
your_choice=int(input("enter your choice!!!!   "))
if your_choice not in [0,1,2]:
    print("your enter a invald number!!")
else:
    computer_choice=random.randint(0,2)
    print("your choice!!!")
    print(choices[your_choice])
    print("computer_choice")
    print(choices[computer_choice])
    if your_choice==computer_choice:
        print("it is a draw")
    elif (your_choice ==1 and computer_choice==0) or \
         (your_choice==2 and computer_choice==1) or \
         (your_choice==2 and computer_choice==0):
         print("you_win")
    else:
        print("your_lose")




















