
import random

def play_game():
    # Generate a random number between 1 and 1006
    secret_number = random.randint(1, 100)
    attempts = 0

    print("Welcome to the Number Guessing Game!")
    print("I'm thinking of a number between 1 and 100.")
    print("Can you guess it?\n")

    while True:
        # Get input from the user
        try:
            guess = int(input("Enter your guess: "))
        except ValueError:
            print("Please enter a valid number!\n")
            continue

        attempts += 1

        # Check the guess
        if guess < secret_number:
            print("Too low! Try a higher number.\n")
        elif guess > secret_number:
            print("Too high! Try a lower number.\n")
        else:
            print(f"\n🎉 Correct! The number was {secret_number}.")
            print(f"You got it in {attempts} attempt(s)!")
            break

    # Ask to play again
    again = input("\nPlay again? (yes/no): ").lower()
    if again == "yes" or again == "y":
        play_game()
    else:
        print("Thanks for playing! Goodbye.")

# Run the game
play_game()
