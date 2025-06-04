Great! Practicing conditional logic with dice-based problems is a fun and effective way to improve your programming skills.

Here’s a **dice rolling problem** with layered conditions to help you improve your `if`, `elif`, `else`, and logical operators:

---

### 🎯 **Dice Game Problem: “Lucky 7s”**

#### 🔸 Problem Statement:

Write a program that simulates rolling **two 6-sided dice**. Based on the total value of the dice, perform the following actions using conditional statements:

#### 🎲 Game Rules:

* If the total is **7 or 11**, print: `"You win!"`
* If both dice show the **same number (doubles)**:

  * If it's **double 1s**, print: `"Snake Eyes! You lose."`
  * If it's **double 6s**, print: `"Boxcars! Try again."`
  * Otherwise, print: `"Doubles! Roll again."`
* If the total is **2, 3, or 12**, print: `"Craps! You lose."`
* In all other cases, print: `"No win. Try again."`

---

### 🧠 Hints:

* Use `random.randint(1, 6)` for each die.
* Use `if`, `elif`, and `else` to test conditions.
* Combine conditions with `and`, `or` as needed.

---

### 💻 Starter Code (You Fill the Logic)

```python
import random

# Roll the dice
die1 = random.randint(1, 6)
die2 = random.randint(1, 6)
total = die1 + die2

print(f"You rolled: {die1} and {die2} (Total: {total})")

# Apply game rules using conditional statements
if total == 7 or total == 11:
    print("You win!")
elif die1 == die2:
    if die1 == 1:
        print("Snake Eyes! You lose.")
    elif die1 == 6:
        print("Boxcars! Try again.")
    else:
        print("Doubles! Roll again.")
elif total in [2, 3, 12]:
    print("Craps! You lose.")
else:
    print("No win. Try again.")
```

---

Would you like a **harder version** that includes scorekeeping, loops, or a player-vs-computer mode?

