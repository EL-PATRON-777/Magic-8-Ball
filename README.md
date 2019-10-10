# Magic-8-Ball
#Magic 8 Ball
#Bienvenido a Bola Majica 8
#Created by Joshua
from tkinter import *
import random

#Variable
textbox_width = 40
textbox_height = 1
button_width = 10

#Functions
def quit_magicball():
    window.withdraw()
    window.quit()
    
def ask():
    

#Answers
 ans1= "Without a doubt; Sin  duda."
ans2="My sources say no; Mis informantes dicen que no."
ans3="Reply hazy try again; Respuesta confusa, vuelva intentar."
ans4="You may rely on it; Puedes confiar en ello."
ans5="Most Likely; Probablemente."
ans6="What, you have lost yor marbles!; Se te perdio un tornillo!"
ans7="Better not tell you now; Mejor no te lo digo ahora"
ans8="Do not count on it"
'''
#Types of answers
yes = 3
maybe = 2
no = 3
'''
answers = ["Without a doubt; Sin duda.",
           "My sources say no; Mis informantes dicen que no.",
           "Reply hazy try again; Respuesta confusa, vuelva intentar.",
           "You may rely on it; Puedes confiar en ello.",
           "Most Likely; Probablemente.",
           "What, you have lost yor marbles!; Se te perdio un tornillo!",
           "Better not tell you now; Mejor no te lo digo ahora"
           "Do not count on it; No cuentes con eso"
           ]
#Make Answer
count = 1
for answer in answers:
    vars() ["ans%d" % count] = answer
    count += 1
name = input("What is your name?; Como te llamas?")
if name == "":
    name = "My King, Mi Rey"
print("Hello; Hola,", name)
print("Welcome to Magic 8 Ball; Bienvenido a Magic 8 Ball")
question = input("Ask your question.")
print("Shaking like never before, shaking...that bacon\n"*8)
choice = random.randint(0,5)

#Use randit() to select answer
if choice == 1:
    answer = ans1

elif choice == 1:
    answer = ans1
elif choice == 2:
    answer = ans2
elif choice == 3:
    answer = ans3
elif choice == 4:
    answer = ans4
elif choice == 5:
    answer = ans5
elif choice == 6:
    answer = ans6
print(answers[random.randint(0,3)])
'''
if thing:
    do something
elif another thing:
    do something else
else:
        do default actoin
'''
