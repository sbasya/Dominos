Introduction
The JavaFX Scrabble Game is a fun digital version of the well-known board game, Scrabble. It's made using Java and JavaFX, which means it has a user-friendly visual interface. This allows one person to play a strategic word game against a computer. This document talks about how the game is put together, what each part does, and how the game works.



Design Overview
This part wraps up everything about the Scrabble game project. It includes all the parts you see and interact with, as well as the behind-the-scenes rules that make the game work. It's all about taking the classic Scrabble game we know.

Classes: 

ValidateTile.java
Where the game begins. This class sets everything up, checks your moves, and does the math for your score.
It also loads the dictionary and processes board configurations to validate moves and calculate scores.

Trie.java
Implements a trie data structure for efficient storage and retrieval of dictionary words for gameplay validation.

BoardTileCell.java
Represents each cell on the Scrabble board, capable of holding a letter tile and displaying score multipliers.

TileRepository.java
Manages the collection of all letter tiles used in the game, like the physical bag of tiles in Scrabble.

Main.java
Entry point for the application, handling the integration of all game components and user interface.

Manager.java
Coordinates the flow of the game, manages turns, and processes user interactions.



Player.java
Handles the human player's actions, such as tile placement and score calculation.

ScrabbleBotOpponent.java
Simulates the computer opponent's behavior and strategy during the game.

ReversedDictionary.java
Stores a reverse-lookup version of the game dictionary to aid in computer player word selection.

ScoreBoard.java
Displays the current score and remaining tile count.

ScrabbleBoard.java
Maintains the state of the Scrabble board throughout the game.

ScrabbleBoardGUI.java
Manages the graphical interface of the Scrabble board, updating visuals after each move.

ScrabbleGame.java
Orchestrates the overall gameplay, integrating all other classes for a seamless experience.

ScrabbleLetter.java
Encapsulates the properties of Scrabble letter tiles, such as letter value and score.

ScrableTileCell.java
Controls the individual cells of the player's tile rack in the GUI.

Tile.java
Represents an individual Scrabble tile with a letter and score value.

TileDisplayGUI.java
Manages the graphical representation of the player's tile rack.

TileRack.java
Stores the collection of tiles currently available to a player.

TileSlot.java
Manages individual cells in the player's tile rack, allowing interaction with the game board.

Trie.java
Implements the trie data structure to store the game dictionary for word validation.


Text Files

dictionary.txt:
Contains all the valid words for Scrabble gameplay, used for word validation.

scrabble_board.txt:
Describes the layout of the Scrabble board with multipliers and bonuses.

scrabble.txt:
Details the scores and frequencies for each Scrabble letter tile.

How To Play:
•	Before you can start playing, you need to compile the Java files within the project directory. Ensure you have the Java Development Kit (JDK) installed on your system.

•	Once the compilation is complete, you can start the game by running the Main class.

•	When you run this command, the game will prompt you to select a dictionary file. Choose dictionary.txt to start the game with the standard Scrabble dictionary. The game initializes and presents the Scrabble board on the screen.

Playing the Game
The game follows the traditional Scrabble rules with the added benefit of a graphical user interface. Here's what you need to know to navigate the gameplay:
•	Starting the Game: Once you've chosen your dictionary file, the game's initial state will be displayed. If it's your turn, you'll see your tile rack at the bottom of the screen.
•	Placing Words: Select tiles from your rack and place them on the board to form words either horizontally or vertically. Words must be connected and present in the dictionary you selected at the beginning.
•	Scoring: Points are awarded based on the letter values and any multipliers (like double letter score or triple word score) that your word covers on the board.
•	Taking Turns: After placing your word and scoring, click the 'Play' button to confirm your move. The computer opponent will then make a move.
•	Drawing Tiles: If you can't play any tiles, you may draw new ones from the tile repository by clicking the 'Exchange Rack' button, provided there are enough tiles left.
•	Ending the Game: The game ends when all tiles are used up or no valid moves are left. The final scores are tallied, and the player with the highest score wins.
•	Exiting the Game: You can exit the game at any time by closing the application window.






Prerequisites:
Java JDK 11 or newer.
JavaFX SDK 11 or newer.

Developed by Sanjaya Basyal
UNM ID: 101977557
![image](https://github.com/user-attachments/assets/f5fb00da-f0a0-4c56-9562-d2e3af990dae)
