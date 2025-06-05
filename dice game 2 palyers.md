
Awesome! A two-player game will help you practice loops, conditionals, variables, and turn-taking logic.

---

### Let’s break it down step-by-step with questions to guide you:

---

### Question 1:

How will you **store scores** for two players?
Hint: Use two variables like `score1` and `score2`.

---

### Question 2:

How will you **alternate turns** between Player 1 and Player 2?
Hint: Use a variable like `current_player` and switch it each round.

---

### Question 3:

How will you **ask each player** if they want to roll?
Hint: Inside the loop, prompt the current player, e.g., `"Player 1, roll? (y/n): "`.

---

### Question 4:

How will you **update and display the correct player’s score** after rolling?

---

### Question 5:

What will be your **win condition**?
Hint: Maybe first to reach 50 points wins. Make sure to check it for both players.

---

### Bonus:

How will you **end the game** when one player wins?
Hint: Use `break` or set a game-over flag.

---

**Try to answer these questions by writing code snippets or the whole program step by step. I’m here to help and check!**
## solution
```python

import random
score1 = 0
score2 = 0
current_player = 1

while True:
    if current_player == 1:
        roll = input("Player 1, roll? (y/n): ").lower()
        if roll in ["y", "yes"]:
            die = random.randint(1, 6)
            score1 += die
            print(f"Player 1 rolled a {die}. Score: {score1}")
        else:
            print("Player 1 skipped this turn.")
        # Check if Player 1 won
        if score1 >= 50:
            print("Player 1 wins!")
            break
        current_player = 2

    else:  # current_player == 2
        roll = input("Player 2, roll? (y/n): ").lower()
        if roll in ["y", "yes"]:
            die = random.randint(1, 6)
            score2 += die
            print(f"Player 2 rolled a {die}. Score: {score2}")
        else:
            print("Player 2 skipped this turn.")
        # Check if Player 2 won
        if score2 >= 50:
            print("Player 2 wins!")
            break
        current_player = 1
  ```
