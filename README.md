# Python-Number-Guessing-Game-_-Project
# 🎯 Number Guessing Game

A simple command-line game where the player tries to guess a randomly generated number between 1 and 100. After each guess, the game provides feedback to help narrow down the answer.

---

## 📖 Description

The game generates a secret random number between **1 and 100** at the start of each round. The player keeps guessing until they find the correct number, receiving "Too high" or "Too low" hints along the way. Once guessed correctly, the total number of attempts is displayed. The player can then choose to play again or quit.

### Features

- Random number generation each round
- Directional hints after every guess (Too high / Too low)
- Attempt counter that tracks how many guesses were made
- Input validation — handles non-numeric entries gracefully
- Play again option at the end of each round
- Recursive replay support

---

## 🛠️ Technologies Used

| Technology | Version | Purpose |
|------------|---------|---------|
| Python | 3.x | Core programming language |
| `random` (stdlib) | Built-in | Generating the secret number |

No external libraries or dependencies are required — the game runs entirely on the Python standard library.

---
