🐍 Snake Game (C++ Console) — README
📌 Overview

This is a simple console-based Snake Game written in C++.
The player controls a snake inside a 20×20 grid, tries to eat fruits, grows longer, and avoids colliding with its own tail.

🚀 Features

Classic snake mechanics

WASD controls

Auto-refreshing game loop

Random fruit generation

Score tracking

Screen clears and redraws each frame

Snake tail grows as you eat fruits

Wrap-around wall behavior (no wall death)

🎮 How to Play
Controls
Key	Action
W	Move Up
A	Move Left
S	Move Down
D	Move Right
X	Quit Game
Objective

Move the snake (O) to eat the fruit (F).

Each fruit gives +10 score.

Snake grows longer with every fruit.

Game Over

You lose if the snake collides with its own tail.

You can also press X to exit.

🧱 Game Board Representation
######################
#                    #
#                    #
#        O           #  ← Snake Head
#                    #
#   F                #  ← Fruit
#                    #
######################
Score: 20


# = Border

O = Snake head

o = Snake tail

F = Fruit

🛠️ How to Compile & Run
Windows (MinGW / g++)
g++ snake.cpp -o snake
snake

Linux / macOS
g++ snake.cpp -o snake
./snake


Note: Windows uses <conio.h> and Sleep().
On Linux, you must replace input handling with termios or ncurses.

📂 File Structure
Snake-Game/
│── snake.cpp
│── README.md

🤖 Main Functions Explained
Setup()

Initializes snake position

Spawns fruit at random

Sets score to 0

Draw()

Clears screen

Draws border

Draws snake, fruit, and tail

Prints score

Input()

Uses _kbhit() and _getch()

Reads WASD keys

Logic()

Moves snake

Moves tail

Checks fruit collision

Checks self-collision

Wraps around walls

🧩 Future Improvements (Optional)

You can add:

Difficulty selection

Colorful console output

Sound effects

Menu & pause screen

High score saving

If you want any of these, I can implement them for you.
