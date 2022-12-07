# Cycle Game

## Overview

Cycle is a game where the players try to cut each other off using cycles that leave a trail behind them.

## Rules

Rules
Cycle is played according to the following rules.

    * Players can move up, down, left and right...
        * Player one moves using the W, S, A and D keys.
        * Player two moves using the I, K, J and L keys.

    * Each player's trail grows as they move.
    * Players try to maneuver so the opponent collides with their trail.
    * If a player collides with their opponent's trail...
        * A "game over" message is displayed in the middle of the screen.
        * The cycles turn white.
        * Players keep moving and turning but don't run into each other.

## Getting Started

Make sure you have Python 3.8 or newer and Raylib Python CFFI 3.7 installed and running on your machine. You can install Raylib Python CFFI by opening a terminal and running the following command.

```
python3 -m pip install raylib
```

After you've installed the required libraries, open a terminal and browse to the project's root folder. Start the program by running the following command.

```
python3 cycle
```

You can also run the program from an IDE like Visual Studio Code. Start your IDE and open the 
project folder. Select the main module inside the cycle folder and click the "run" icon.

## Project Structure

The project files and folders are organized as follows:

```
root                    (project root folder)
+-- cycle               (source code for game)
  +-- game              (specific game classes)
  +-- __main__.py       (entry point for program)
+-- README.md           (general info)
```

## Required Technologies

* Python 3.8
* Raylib Python CFFI 3.7

## Authors

* M. Scott Reynolds rey22006 at byui.edu

## FAQ

Q. What is polymorphism and why is it important?
A. Polymorphism in programming is the ability to have a method's behavior change depending on the programming context. A parent class can define a method that behaves in a certain or default way. Child classes of that parent class can override that same method, by defining a method with the same name and parameters and changing its behavior. This is important because it allows placing common methods and attributes in a single parent class and then having the child classes only implement the different behavior of a particular method. This can greatly simplify programming by reducing the need to define identical methods in multiple child classes.

Q. How did you apply polymorphism in your program's design?
A. Polymorphism is used in the Action class and its child classes. The execute_action() method doesn't do anything in the base Action class and must be further defined in each child class. The child class will override the execute_action() method to perform whatever it is the child class is designed to do. For example, a child class could be designed to draw the current state of the game. Another child class can get the users input. And another class can take the users input and update the state and scores of the game.


      
