# GameEngineBonus
Ewan Chang - 100787343
1 + 0 + 0 + 7 + 8 + 7 + 3 + 4 + 3 = 33 = Odd Number

My designated game is Wrecking Crew. The challenge is that I need to implement demonstrate a singleton design pattern for the main character damage manager
and explain how it works and why I implemented it this way. The next challenge is to implement and demonstrate the command design pattern for inverting the
mapped keys that control the main character in the game. The third challenge is to explain a use for the observer pattern in the designated game and how
I would implement it and why. The final challenge is to create a low-fidelity scene of the game in Unity.


Observer Pattern Explanation:

I implemented the observer pattern by having the player be the subject while the enemy/fireball objects are the observers.
I implemented it in this manner because it seems like an efficient way to keep track of when the player gets hit.
As shown in the flowchart, enemy objects will chase the player in the level while fireballs will be spawned randomly.
If the player gets hit by one of them, they lose a life. The game will check if the player is out of lives, if NO, then enemies will
continue chasing the player and fireballs continue to spwan randomly. If the player is OUT of lives, then it's game over and the game ends.
While that is going on, for the levels where Spike is present, if the player gets hit by Spike, the player will fall to the bottom of the level.
This implementation benefits the game by making it easy to establish the relations between objects, and also add new enemies that act similarly
to the ones aready present in the game if someone wants to add a new enemy.