# DiceGame Class - Dice Rolling Game
The DiceGame class represents a simple console-based dice rolling game where the player competes against an AI enemy. The game simulates rolling a six-sided dice for both the player and the enemy for a total of 10 rounds. After each round, the game announces the winner or declares a draw, and keeps track of the score for both the player and the enemy. At the end of the 10 rounds, the game determines the overall winner based on the total points earned by each side.

## Main Method
The Main method is the entry point of the application. It initializes variables to store the random numbers rolled by the player and the enemy, as well as their respective points.

The application uses the Random class to generate random numbers. It creates an instance of the Random class and enters a loop that runs for 10 rounds, representing the number of times the dice is rolled.

## Dice Rolling Loop
In each iteration of the loop:

* The program prompts the player to roll the dice by displaying the message: "Press any key to roll the dice." The player presses any key to proceed.
* The player's random number is generated using random.Next(1, 7), which simulates rolling a six-sided dice and stores the result in playerRandomNum.
* The player's roll result is displayed to the console with the message: "You rolled a [playerRandomNum]."
* A brief delay of 1 second is added to simulate a pause: "..."
* The enemy AI's random number is generated using random.Next(1, 7) and stored in enemyRandomNum.
* The enemy's roll result is displayed to the console with the message: "Enemy AI rolled a [enemyRandomNum]."
## Determining Round Winner
* The application compares the player's roll result (playerRandomNum) with the enemy's roll result (enemyRandomNum).
* If the player's roll is greater than the enemy's, the player wins the round, and their score (playerPoints) is incremented by one. The message "Player wins this round!" is displayed.
* If the player's roll is less than the enemy's, the enemy wins the round, and their score (enemyPoints) is incremented by one. The message "Enemy wins this round!" is displayed.
* If both the player and the enemy roll the same number, it is a draw, and the message "Draw!" is displayed.
## Displaying Round Scores
* After each round, the current scores for both the player and the enemy are displayed with the message: "The score is now - Player: [playerPoints]. Enemy: [enemyPoints]."
## Determining Overall Winner
* After the 10 rounds are completed, the application compares the total points earned by the player (playerPoints) and the enemy (enemyPoints) to determine the overall winner.

* If the player's score is greater than the enemy's, the message "You Win!" is displayed.

* If the player's score is less than the enemy's, the message "You lose!" is displayed.

* If both the player and the enemy have the same total points, the message "It's a draw" is displayed.

* The application waits for the player to press any key before closing.

The game provides a fun and simple experience where the player can roll the dice and compete against the AI enemy, trying to get the higher roll to win each round and be the overall winner of the game.