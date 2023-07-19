# rock_paper_scissors
import random 
rock = """ ROCK
_______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
"""
paper= """ PAPER
_______
---'    ____)____
           ______)
          _______)
         _______)
---.__________)
"""
scissors = """ SCISSORS
_______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
"""
play = int(input("Type 0 for Rock, 1 for Paper and 2 for Scissors "))
print()
if play == 0:
  print(rock)
elif play == 1:
  print(paper)
else: print(scissors)
print()
computer_play = random.randint(0,2)
print("Computer plays: ")
print()
if computer_play == 0:
  print(rock)
elif computer_play == 1:
  print(paper)
else: print(scissors)
print()
if play==0 and computer_play==0:
  print("TIE") 
elif play==0 and computer_play==1:
  print("You LOSE")
elif play==0 and computer_play==2:
  print("You WIN")
elif play==1 and computer_play==0:
  print("You WIN")
elif play==1 and computer_play==1:
  print("TIE")
elif play==1 and computer_play==2:
  print("You LOSE")
elif play==2 and computer_play==0:
  print("You LOSE")
elif play==2 and computer_play==1:
  print("You WIN")
else:
  print("Its a tie")
