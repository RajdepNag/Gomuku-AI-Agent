# Gomoku AI Agent


Gomoku is a popular game played on the Go board, following much simpler rules. 

- There are two players, one placing black pieces and the other white pieces, at the grid intersections of the board. 
- The two players take turns to place one piece each time. Pieces are never moved or removed from the board. 
- The players' goal is to have five pieces of their own color to form an unbroken line horizontally (`examples/ex1.png`), vertically (`examples/ex2.png`), or diagonally (`examples/ex3.png`). Of course, these are unlikely realistic games between reasonable players. A real game is more like `examples/ex4.png` (black is still very lame at the end).  
- The game engine starts with human against a random-play agent. Click any grid intersections and see what the computer does. Press enter to see a random game between two random-play agents (also press enter to pause autoplay and switch back to human vs random). Press 'm' to switch to manually playing both sides.  

Here's a youtube video of a competitive Gomoku game (in case you're interested, or want to procrastinate): https://www.youtube.com/watch?v=siYgHaEwmZU&ab_channel=SandraJones

I've mplement MCTS in `ai.py`. 

In MCTS, the search exits when the "computation budget" is reached. The current default value is 1000, which will be used for testing. You can increase or decrease it to see the different behaviors of AI. For instance, with a budget over 6000, a correctly implemented MCTS AI should be able to play a fairly interesting game against you (although it may still make some obvious mistakes when the number of next actions to consider gets larger). 

