# Aneesh Bulusu: CPSC 210 Personal Project

## Number Guessing Game

- *What will the application do?*

The application will be a simple number guessing game. A random number will be generated by the computer
and the player will input guesses. If the input is not equal to the generated number, the application will
return "higher" or "lower" accordingly. If the input is equal to the generated number, the application will return 
some sort of congratulatory message. Further features will be implemented to increase challenge and difficulty, such as
limited attempts, time limits, and allowing the player to choose the range of numbers from which the random number
is generated. 

- *Who will use it?*

Anyone who wants to play a simple game to kill time can use this application. People who want to test their luck or 
deductive reasoning skills may also play it and increase the difficulty settings to give themselves a satisfying and 
rewarding experience. 

- *Why is this project of interest to you?*

This project interests me because from the start of CPSC 210 I knew I wanted to develop some sort of game for my term 
project. This game in particular interests me as it involves a decent level of math and probability which I am really 
passionate about as I am a math and computer science major. The logic required to implement such a game is also 
something I am excited to work with, and I feel that the graphical interface and design can be as complicated or as 
simple as I prefer, provided I stay within the guidelines of the project deliverables, which gives me a fair level of 
freedom when designing the application and working through the phases. 

## User Stories 

- As a user, I want to add my guess to a list of all my previous guesses, and see all of them upon completing the game
- As a user, I want to be able to input a number and have the application give me appropriate feedback
- As a user, I want to be able to restart the game 
- As a user, I want to specify the range of numbers from which the computer generates a random number 
- As a user, I want to choose how many attempts I have to guess the number 
- As a user, I want to be able to quit and save the game 
- As a user, I want to be able to load up my saved game 

## Phase 4: Task 2 

For task 2 of phase 4 I decided to choose the first option i.e., test and design a class in my model package that is 
robust. 

I made the GuessingGame class robust. I implemented exception handling in the setMax and the setAttempts method. 
For the setMax method, I designed the NonPositiveMaximumException, which is a checked exception. 
For the setAttempts method, I designed the NonPositiveAttemptsException, which is a checked exception. 

## Phase 4: Task 3

If I had more time to work on the project, I would do the following in terms of refactoring:

- Split the methods and functionality inside the GuessingGameGUI class into distinct gameFrame, gamePanel, gameLabel, 
and gameButton classes 
- Refactor the GuessingGameApp class to have separate classes that can handle user input and apply 
it to the model code 
- Reduce the number of associations in the UML diagram by having my GUI-related code have only a GuessingGame field 
as far as fields from the model package go, thus taking advantage of the uni-directional relationships between 
GuessingGame and PreviousGuesses, and PreviousGuesses and Guess to access all model behaviour while reducing 
coupling in the code.
