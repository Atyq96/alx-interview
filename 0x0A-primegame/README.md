0x0A. Prime Game
Maria and Ben are playing a competitive game with a set of consecutive integers starting from 1 up to n. During each round, they take turns selecting a prime number from the set and removing that prime along with all of its multiples from the set. The game continues until one player can no longer make a valid move, at which point they lose the round.

The game is played over x rounds, with the value of n potentially being different in each round. Maria always plays first, and both players are assumed to use optimal strategies. The objective is to determine who wins the most rounds.

Objective:
Determine the player who wins the majority of the rounds after all rounds have been played.

Inputs:
x: The number of rounds in the game.
nums: A list of integers where each number represents the value of n for the corresponding round.
Output:
The function should return the name of the player with the most wins—either "Maria" or "Ben".
If both players have an equal number of wins, return None.
Key Considerations:
The values of n and x will not exceed 10,000.
No external libraries or packages should be used to solve the task.
Example Scenario:
Suppose x = 3 and the list nums = [4, 5, 1]:

Round 1 (n = 4):

Maria picks the prime number 2 and removes both 2 and 4, leaving the set {1, 3}.
Ben picks the prime number 3 and removes 3, leaving {1}.
Ben wins this round since Maria has no more prime numbers to choose.
Round 2 (n = 5):

Maria picks the prime number 2 and removes 2 and 4, leaving the set {1, 3, 5}.
Ben picks the prime number 3 and removes 3, leaving {1, 5}.
Maria picks the prime number 5 and removes 5, leaving {1}.
Maria wins this round since Ben has no more prime numbers to choose.
Round 3 (n = 1):

There are no prime numbers for Maria to select, so Ben wins by default.
Final Outcome:
In this example, Ben wins two rounds and Maria wins one round. Therefore, Ben is declared the overall winner.
