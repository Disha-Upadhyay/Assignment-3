# Assignment-3
Snake-Water-Gun Game 

This is a simple command-line implementation of the classic Snake-Water-Gun game (similar to Rock-Paper-Scissors).
The user selects one option, the computer randomly selects another, and the program determines the winner.

Game Rules

The game uses the following rules:

Snake (s) drinks Water (w) → Snake wins

Water (w) damages Gun (g) → Water wins

Gun (g) kills Snake (s) → Gun wins

If both choices are the same → Draw

How the Program Works

The program generates a random number using rand() and assigns the computer's choice:

1–32 → Snake

33–65 → Water

66–100 → Gun

The user is prompted to enter a character:

's' → Snake

'w' → Water

'g' → Gun

The function snakeWaterGun() compares the choices and returns:

1 → User wins

-1 → Computer wins

0 → Draw

The result is displayed to the user.

Compilation & Execution
Compile the program
gcc game.c -o game

Run the program
./game

Input Example
Enter 's' for snake, 'w' for water and 'g' for gun
s

Output Example
You chose s and computer chose w. You win!

File Structure
game.c     # Source code of the Snake-Water-Gun game

Notes / Improvements

Validate user input (prevent invalid characters).

Improve randomness by scaling distribution equally.

Allow replaying the game in a loop.

Provide a menu or better user interface.
