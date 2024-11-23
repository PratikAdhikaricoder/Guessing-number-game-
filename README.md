# Guessing-number-game-
#This is a funny game depends on your calculation and luck
import random
number_to_guess = random.randint(1, 100)
while True:
    try:
        guess = int(input("Guess the number betweeen 1 and 100: "))

        if guess < number_to_guess:
            print("Too low!")
        elif guess > number_to_guess:
            print("Too high!")
        else:
            print("Congratulations! You guess the right number ")
            break
    except ValueError:
        print("Please enter a valid number")
