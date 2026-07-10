# Technical Description

This project is a Java implementation of the classic Minesweeper game. It was developed as a final project and focuses on reproducing the core mechanics of the original game while applying object-oriented programming principles.

The application is structured around a grid-based system where each cell represents a playable tile. The game logic manages hidden cells, mines, flags, revealed tiles, and the calculation of neighbouring mines. The player interacts with the board through a graphical interface, allowing tiles to be revealed or marked with flags.

## Main Objectives

The goal of this project is to build a functional desktop Minesweeper game while demonstrating the use of Java, object-oriented design, event handling, and graphical user interface management.

The project also aims to separate the main responsibilities of the application into dedicated components, such as the grid logic, individual tile representation, user interface controls, game settings, and application entry point.

# Core Features
## Grid-Based Game Logic

The game is based on a dynamic grid composed of individual boxes. Each box stores its own state, such as whether it contains a mine, whether it has been revealed, whether it has been flagged, and how many mines are located around it.

The grid handles the overall game structure and is responsible for generating the board, placing mines, managing tile states, and checking game progression.

## Tile and Box Management

Each tile represents an interactive element of the game board. Tiles can be revealed by the player or marked with a flag when the player suspects that a mine is hidden underneath.

The project includes visual resources for the tiles and flags, allowing the interface to provide a clearer and more user-friendly experience.

## Graphical User Interface

The application includes a graphical interface that allows the player to interact with the Minesweeper board. User interactions are handled through controller logic, which connects the visual components to the underlying game model.

The interface reacts to player actions such as clicking on a tile, revealing a box, placing or removing a flag, and updating the board display according to the current game state.

## Game Controller

A dedicated controller manages the interaction between the graphical interface and the game logic. It listens to player actions, updates the grid accordingly, and refreshes the displayed board.

This separation helps keep the project organized by distinguishing between the visual layer and the logical layer of the game.

## Settings Management

The project includes a settings component used to manage configurable game parameters. These settings may include elements such as the size of the grid, the number of mines, or other gameplay-related values.

This makes the project easier to extend with different difficulty levels or custom game configurations.

# Technical Approach

The project follows an object-oriented architecture. Each major concept of the game is represented by a dedicated class:

Main handles the application entry point.  
Grid manages the overall Minesweeper board.  
Box represents the state and behaviour of an individual cell.  
GridViewController manages interactions between the interface and the game logic.  
TileButton represents the clickable graphical elements of the board.  
Settings stores configurable game parameters.  

The application separates the game model from the user interface logic, making the code easier to understand, maintain, and extend.

+ Technologies Used
+ Java
+ Gradle project structure
+ Graphical user interface components
+ Event-driven programming
+ Object-oriented programming
