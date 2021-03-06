# Oxotree

`oxotree.c` is a modified version of Tic-Tac-Toe. Instead of a noughts and crosses game between two players, it is a noughts and crosses game between a human player and the computer.

## Install

A Makefile is included in the repo with the necessary flags, and it will work on Windows, MacOS and any Linux distro, so just type `make` in the console in the folder with the `huff.c` source file.

## Running

The program is run with `./oxotree X` or `./oxotree O`,  so that the human player chooses whether they want to go first or second. X always goes first. The player has to input the coordinates of the cell they want to play.

## Extra info

The computer player uses a game tree to decide what the best move is.  The scoring function is based on the winning player and the game depth, so the computer ends a game as fast as possible. The computer always plays a perfect game (it either always wins, or ends in a draw). The function to find the best move makes use of a minimax algorithm. Every possible outcome is calculated each time the computer choses a new move.

Testing of the additional functions is done with `./oxotree`, however, the fact that the computer runs through all the remaining possible games before deciding on the best move makes it particularly unpredictable.

## Resources used:

- Game tree: https://en.wikipedia.org/wiki/Game_tree

- Minimax algorithm: https://en.wikipedia.org/wiki/Minimax
