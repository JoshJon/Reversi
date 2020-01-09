# Reversi

Something from when I was still a noob at coding 🙃

## About
Reversi is a classic board game for two players just like chess, checkers and go.

### Rules

Each player has 2 tokens placed in the locations specified. The token’s location is reffered to by two digits in a row, separated by a comma – firstly the column and then the row. For example, “1,1” would refer to the top left cell.

Players will be randomly assigned a colour, red or blue. The red player will always move first, and then players will take turns with their moves until one player concedes the game by pressing ctrl-d or the enter key on a new line.

A valid move is a move where a player captures some opponent pieces. Please see the reversi rules for further details: http://www.yourturnmyturn.com/rules/reversi.php

An example of the board structure can be found below.

```
     1   2   3   4   5   6   7   8  
====================================
 1 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
------------------------------------
 2 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
------------------------------------
 3 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
------------------------------------
 4 | 0 | 0 | 0 | 🔴| 🔵| 0 | 0 | 0 |
------------------------------------
 5 | 0 | 0 | 0 | 🔵| 🔴| 0 | 0 | 0 |
------------------------------------
 6 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
------------------------------------
 7 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
------------------------------------
 8 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
------------------------------------
====================================

- R & B represent red and blue tokens respectively.
- Tokens are actually colored in game
```

## Compiling and Running
Execute the following terminal commands whilst in the source directory:
```
make
./reversi
```
## Structure
**shared.h**
* Constants, macros and data structure definitions required for the whole program.

**utility.c/h**
* Contains utility functions to perform generic actions.

**gameboard.c/h**
* Contains all the functions and declarations relating to the gameboard.

**scoreboard.c/h**
* Contains all the functions and structs relating to the scoreboard.

**game.c/h**
* Contains all the functions and declarations needed to control the logic and flow of the game.

**reversi.c/h**
* Contains main and all the functions and declarations that manage the user interface.

## Author
**Joshua Jon** - [GitHub](https://github.com/JoshJon)

Start up code was provided by Paul Miller.
