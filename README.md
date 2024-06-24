# **Number Guessing Game in Python**

## **Description**:
A number guessing game in Python is a simple and fun interactive program where the computer randomly selects a number within a specified range, and the player attempts to guess this number. The computer provides feedback on whether the player's guess is too high, too low, or correct.
The computer chooses a random number between 1 to 50
The Program Asks For the User if they want it to be 'easy' or 'hard'
The 'easy' level gives maximum 10 attempts
the 'hard' level gives maximum 5 attempts
If the number the user guessed is higher than the choosen number then the output would be "Your guess is too high"
If the number the user guessed is lower than the choosen number then the output would be "Your guess is too low"

## Creating logo_art file

* Create a logo of the design you like from this [website](https://patorjk.com/software/taag/#p=display&f=Graffiti&t=Type%20Something%20)
* Select the font you like and paste it inside logo_art.py file

```python
logo = "your logo"
```

## Import packages in your file
```python
import random
import logo_art
```
## Expected Output:
```
   _____                       _______ _            _   _                 _               
  / ____|                     |__   __| |          | \ | |               | |              
 | |  __ _   _  ___  ___ ___     | |  | |__   ___  |  \| |_   _ _ __ ___ | |__   ___ _ __ 
 | | |_ | | | |/ _ \/ __/ __|    | |  | '_ \ / _ \ | . ` | | | | '_ ` _ \| '_ \ / _ \ '__|
 | |__| | |_| |  __/\__ \__ \    | |  | | | |  __/ | |\  | |_| | | | | | | |_) |  __/ |   
  \_____|\__,_|\___||___/___/    |_|  |_| |_|\___| |_| \_|\__,_|_| |_| |_|_.__/ \___|_|   

Let me think of a number between 1 to 50.
Choose level of difficulty...Type 'easy' or 'hard': 
```
## Main Function:
```python
def easy_hard(choose_num,attempts):
    print("You have ",attempts," attempts remaining to guess the number!")
    for i in range(1,attempts+1):
        guess = int(input('make a guess'))
        if guess > choose_num:
            print("Your guess is too high")
            print(no_guess(attempts,i)) 
        elif guess < choose_num:
            print("Your guess is too low")
            print(no_guess(attempts,i))
        else:
            print("Your guess is right..The answer was ",choose_num)
            break
```
This is the main function which takes the user input after printing the number of attempts left
Then it prints if the User guess is Too high or Too low or Correct guess
For Calculating the Number of guesses left, we used no_guess() function



