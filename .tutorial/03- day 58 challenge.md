# 👉 Day 58 Challenge

This challenge is all about using the debugger.

Copy the broken code below into 'main.py' and use the debugger to help spot the mistakes in it. 

```python
import random, os, time
totalAttempts = 0

def game():
  attempts = 0
  while True:
    number = random.randint(1,100)
    guess = int(input("Pick a number between 1 and 100: "))
    if guess > number:
      print("Too high")
      attempts+=1
    elif guess < number:
      print("Too low")
      attempts+=1
    else:
      print("Just right!")
      print(f"{attempts} attempts this round")
      return attempts

while True:
  menu = input("1: Guess the random number game\n2: Total Score\n3: Exit\n> ")
  if menu == 1:
    totalAttempts+= game()
  elif menu == 2:
    print(f"You've had {totalAttempts} attempts")
  else:
    break
```


<details> <summary> 💡 Hints </summary>

- Set breakpoints where you want the code to pause.
- Use the 'next step' to track the contents of variables and lists line by line when you're not sure what's going on.

</details>

