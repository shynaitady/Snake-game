# Snake Game Course Work 
## made by Shyngys Zhaksylyk group EIRFU-23

## Overview
This Python project is an implementation of the classic Snake game using the `pygame` library. It features gameplay mechanics such as snake movement, food collection, score tracking, and a leaderboard system. The game showcases several Object-Oriented Programming principles and design patterns to provide a well-structured and extensible codebase.

## Installation
To run this game, you'll need Python and pygame installed on your machine.
- Python: Install from [python.org](https://www.python.org/downloads/)
- Pygame: Install using pip:
  ```bash
  pip install pygame

## How to start playing?
**To start a game:**
- Use hotkey: Ctrl + F5
- Press button "Run Python File" in VS Code.

**How to play?**
- Use __WASD__ or __Arrows__ to move snake
- Eat food to increase your score and length.

Food has two types: 
1. Red food gives you 10 points
2. Blue food gives you 20 points

# OOP pillars that are implemented in code:

## Polymorphism:
Polymorphism in OOP allows objects to be treated as instances of their parent class, with the ability to override or implement behaviors in different ways. In your code, polymorphism is evident in the way different game objects handle the draw() method:

- GameObject class declares an abstract method draw(). This method is then implemented distinctly in Snake and Food classes, each overriding the method to handle drawing specific to their type. Here, the same function name draw() is used for different object types, each behaving differently depending on the class that implements it.

## Abstraction:
Abstraction involves hiding complex implementation details and showing only the essential features of the object. In your code:

The GameObject class serves as an abstract base class for other game objects. It includes the abstract method draw(), which forces all subclasses to provide their own specific implementation of this method. The GameObject class provides a template and essential interfaces, hiding the details and complexity from the user (or developer in this case).

## Inheritance:
Inheritance allows one class to inherit attributes and methods from another. This helps in code reusability and can enhance the application’s architecture:
The Snake and Food classes inherit from the GameObject class. They use properties and methods defined in the GameObject class.
```ruby
class Snake(GameObject):
class Food(GameObject):
```