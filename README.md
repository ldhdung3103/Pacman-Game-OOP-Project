# Pacman Game - OOP Project

## Overview

Pacman Game is a Java-based implementation of the classic Pacman arcade game developed as an Object-Oriented Programming (OOP) course project.

The player controls Pacman through a maze, collecting food pellets while avoiding ghosts. Special power-ups allow Pacman to temporarily hunt ghosts and gain bonus points. The game features multiple levels, score tracking, respawn mechanics, and a graphical user interface built with Java Swing.

---

## Features

### Gameplay

* Classic Pacman movement system
* Multiple ghost enemies
* Food pellet collection
* Power mode mechanics
* Cherry bonus items
* Score system
* Multiple levels
* Win and Game Over screens
* Ghost respawn system

### User Interface

* Main Menu
* Game Screen
* Level Complete Screen
* Victory Screen
* Game Over Screen

### Technical Features

* Object-Oriented Design
* Collision Detection System
* Entity Management System
* State Management
* Event-Driven Input Handling
* Modular Architecture

---

## Project Structure

```text
src
├── Entities
│   ├── Block.java
│   ├── MovableBlock.java
│   ├── PacmanPlayer.java
│   ├── Ghost.java
│   └── Updatable.java
│
├── Input
│   └── InputHandler.java
│
├── Logic
│   ├── GameEngine.java
│   ├── GameState.java
│   ├── CollisionDetector.java
│   ├── PacmanSystem.java
│   ├── GhostSystem.java
│   ├── GhostController.java
│   ├── ItemSystem.java
│   └── RespawnSystem.java
│
├── Map
│   ├── GameMap.java
│   └── MapData.java
│
├── UI
│   ├── Menu.java
│   ├── PacmanGamePanel.java
│   ├── LevelWinScreen.java
│   ├── GameWinScreen.java
│   └── GameOverScreen.java
│
├── Utils
│
└── Main
    └── Main.java
```

---

## OOP Concepts Applied

### Encapsulation

Game data and behaviors are encapsulated within classes such as:

* PacmanPlayer
* Ghost
* GameState
* GameEngine

### Inheritance

The project uses inheritance to reduce code duplication.

```text
Block
   └── MovableBlock
           ├── PacmanPlayer
           └── Ghost
```

### Polymorphism

The `Updatable` interface allows different game entities to implement their own update logic.

### Abstraction

Game logic is separated into specialized systems:

* PacmanSystem
* GhostSystem
* ItemSystem
* RespawnSystem

This keeps the architecture modular and easier to maintain.

---

## Game Architecture

The project follows a layered architecture:

```text
UI Layer
     ↓
Game Engine
     ↓
Game Systems
     ↓
Entities & Map
```

### Main Components

#### GameEngine

Acts as the central coordinator of the game.

Responsibilities:

* Update game state
* Manage systems
* Load levels
* Control game flow

#### GameState

Stores all runtime information:

* Score
* Lives
* Current level
* Power mode status
* Active entities

#### CollisionDetector

Handles collision checking between:

* Pacman and walls
* Pacman and ghosts
* Pacman and items

#### GhostController

Controls ghost movement behavior and direction changes.

---

## How to Run

### Requirements

* Java JDK 8 or higher
* IntelliJ IDEA / Eclipse / NetBeans

### Clone Repository

```bash
git clone https://github.com/ldhdung3103/OOPProject-PacmanGame.git
```

### Run

Open the project in your IDE and execute:

```java
Main.Main
```

or run:

```bash
java Main.Main
```

---

## Controls

| Key | Action     |
| --- | ---------- |
| ↑   | Move Up    |
| ↓   | Move Down  |
| ←   | Move Left  |
| →   | Move Right |

---

## Design Goals

* Apply Object-Oriented Programming principles
* Build a maintainable game architecture
* Separate UI, Logic, and Entity layers
* Demonstrate inheritance and polymorphism in a real project

---

## Future Improvements

* Smarter ghost AI
* Additional levels
* Sound effects and background music
* High score leaderboard
* Save and load functionality
* Difficulty settings

---

## Authors

Developed as an Object-Oriented Programming course team project.

---

## License

This project is licensed under the MIT License - see the LICENSE file for details.
