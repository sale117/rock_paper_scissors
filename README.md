# Rock, Paper, Scissors Game

This is a simple Rock, Paper, Scissors game implemented in Python. The game allows a user to play against the computer, displaying ASCII art for each choice.

### Importing the Random Module
`import random`  
The random module is imported to help the computer make a random choice.

### Defining ASCII Art
Three variables (rock, paper, scissors) are defined to hold the ASCII art for each choice.

### Storing Art in a List
`game_art = [rock, paper, scissors]`  
The game_art list holds the ASCII art for Rock, Paper, and Scissors. This allows easy access to the art based on the user's or computer's choice.

### Getting User Input
`user_choice = int(input('What do you choose? Type 0 for Rock, 1 for Paper or 2 for Scissors:\n'))`  
The user is prompted to enter a number (0, 1, or 2). The `input` function reads the user's input as a string, and `int` converts it to an integer.

### Displaying User Choice
`print(game_art[user_choice])`
The user's choice is used as an index to print the corresponding ASCII art from the `game_art list.`

### Generating Computer Choice
`computer_choice = random.randint(0, 2)`  
`print(f'Computer chose:')`  
`print(game_art[computer_choice])`  
The computer randomly selects a number between 0 and 2 using `random.randint.`

### Determining the Winner
`if user_choice >= 3 or user_choice < 0:`  
`  print('You typed an invalid number, you lose!')`  
`elif user_choice == 0 and computer_choice == 2:`  
`  print('You win!')`  
`elif computer_choice == 0 and user_choice == 2:`  
`  print('You lose')`  
`elif computer_choice > user_choice:`  
`  print('You lose')`  
`elif user_choice == computer_choice:`  
``print('It's a draw')``  
`  else:`  
`print('You win!')`

The code checks various conditions to determine the winner:  
If the user enters an invalid number (not 0, 1, or 2), they lose.  
Rock (0) beats Scissors (2).  
Scissors (2) beats Paper (1).  
Paper (1) beats Rock (0).  
If both choices are the same, it's a draw.  
Any other scenario results in a win for the user.  
