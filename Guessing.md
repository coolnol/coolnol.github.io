''' mermaid
flowchart TD
    A[Start Game] --> B[Generate a Random Number]
    B --> C[Prompt User for a Guess]
    C --> D{Is Input Numeric?}
    D -- Yes --> E{Is Guess within Range?}
    D -- No --> C
    E -- No --> C
    E -- Yes --> F{Is Guess Correct?}
    F -- Yes --> G[Display "Correct! You Win!"]
    F -- No --> H{Is Guess Too High?}
    H -- Yes --> I[Display "Too High! Try Again!"]
    H -- No --> J[Display "Too Low! Try Again!"]
    I --> C
    J --> C
    G --> K[End Game]
'''


 The start game will start the game, then it will generate a number in a specified range, next the user is asked to put in a guess, it will then check to see if it is a valid number and that it is in the specified range.
 After all that it will check to see if the guess was right or not, if it is the game ends and a message is displayed; if the guess is wrong it will check if the guess was to high or to low providing feedback on what it found,
 and is asked to try again. 
