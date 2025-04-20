# Number-guessing-game-
Number guessing game 
import random

secret_number = random.randint(1, 100)
guess = None
tries = 0

while guess != secret_number:
    guess = int(input("Guess a number between 1 and 100: "))
    tries += 1

    if guess < secret_number:
        print("Too low! Bro, guess a bigger number.")
    elif guess > secret_number:
        print("Too high! Guess a smaller number.")
    else:
        print(f"Good job! You guessed the number in {tries} tries.")
