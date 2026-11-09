# C Maze Game

A terminal maze game written in C for my first-year Procedural Programming module at the University of Leeds.

The program loads a maze from a text file, finds the start (`S`) and finish (`E`), and lets the player move with `W` `A` `S` `D` until they reach the exit. It validates the map (size, rectangular shape, allowed symbols) and rejects illegal moves into walls or out of bounds.

## Run it

```bash
gcc Skeletoncode.c -o maze
./maze Maps/MazeGame.simple.map
```

## Tests

`tests.sh` builds the game and runs it against the maps in `Maps/` and the scripted inputs in `Inputs/`. It covers valid mazes of different sizes, empty, non-rectangular and badly formed maps, invalid controls, walking into walls and moving out of bounds.

```bash
./tests.sh
```

## Tech

C (standard library only), Bash for the test harness.
