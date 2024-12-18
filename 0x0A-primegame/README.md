Prime Game

For understanding purpose through different representation, let Maria be Chloe and John be Ben.
Chloe and John are playing a game. Given a set of consecutive integers starting from 1 up to and including n, they take turns choosing a prime number from the set and removing that number and its multiples from the set. The player that cannot make a move loses the game.

They play x rounds of the game, where n may be different for each round. Assuming Chloe always goes first and both players play optimally, determine who the winner of each game is.

Prototype: def isWinner(x, nums)
where x is the number of rounds and nums is an array of n
Return: name of the player that won the most rounds
If the winner cannot be determined, return None
You can assume n and x will not be larger than 10000
You cannot import any packages in this task

Example:

x = 3, nums = [4, 5, 1]
First round: 4

Chloe picks 2 and removes 2, 4, leaving 1, 3
John picks 3 and removes 3, leaving 1
John wins because there are no prime numbers left for Chloe to choose
Second round: 5

Chloe picks 2 and removes 2, 4, leaving 1, 3, 5
John picks 3 and removes 3, leaving 1, 5
Chloe picks 5 and removes 5, leaving 1
Chloe wins because there are no prime numbers left for John to choose
Third round: 1

John wins because there are no prime numbers for Chloe to choose
Result: John has the most wins
