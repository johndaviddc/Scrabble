# SCRABBLE WORD SCORER

This program allows two players to input words and calculates their scores using the standard Scrabble point system. The player with the highest score wins, and in the case of a tie, the program will declare a tie.

## How to Use

1. Compile the program using a C compiler.
2. Run the compiled program in a terminal or command prompt.
3. When prompted, enter a word for Player 1 and press enter.
4. When prompted, enter a word for Player 2 and press enter.
5. The program will then output which player has won or if there is a tie.

## How it Works

The program uses an array of integer values called **'POINTS'**, which assigns a point value to each letter of the alphabet. It then accepts input words from both players, calculates their scores using the point values assigned to each letter, and compares the scores to determine the winner.

The **'compute_score()'** function takes in a string as input and returns an integer score. It iterates through each character in the string, converts it to uppercase, and calculates the index of the character in the **'POINTS'** array. If the character is a letter, it adds the corresponding point value to the score.

The **'main()'** function prompts the user to input words for both players, calls **'compute_score()'** to calculate the score for each word, and compares the scores to determine the winner. If one player's score is higher than the other's, the program prints the message "Player X wins!" (where X is either 1 or 2). If the scores are tied, the program prints the message "Tie!".