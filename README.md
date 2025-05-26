## Console Checkers (Checkers in C#)
A simple console-based implementation of the checkers (draughts) game for two players. The project is written in C# and runs as a console application.

## 🎮 Game Description
The game is intended for two players playing on the same computer.

Each player takes turns, aiming to eliminate all of the opponent's pieces.

A piece can move diagonally forward (or both directions if it becomes a king).

Jumping over an opponent’s piece removes it from the board.

## ♟️ Piece Symbols:
O – Player 1 (regular piece)

K – Player 1 (king)

X – Player 2 (regular piece)

Q – Player 2 (king)

- – Empty space

## ▶️ Running the Game
Open the project in any C# IDE (e.g., Visual Studio or Rider).

Compile and run the project as a Console Application.

Alternatively, run the compiled .exe from the command line:

```bash
dotnet run
```
## 🕹️ Controls
The game runs in the console, and players manually enter their moves using coordinates.

Coordinates are entered in the format: row column (space-separated).

First, enter the starting position of the piece, then the target position.

Example move:
```bash
Enter starting row and column (separated by space): 2 0  
Enter target row and column (separated by space): 3 1
```
If the move is invalid, a message will be displayed, and the player must try again.

When a regular piece reaches the last row, it is promoted to a king (K or Q).

## ⚠️ Limitations
Multiple jumps are not implemented.

King movement logic (especially diagonal backward movement) is partially incomplete.

Input validation is basic – players must enter correct numbers (0–7).

## 📁 Structure
Program.cs – the main file containing the game logic

All methods (IsValidMove, CheckWin, DrawBoard) are defined in the same class

## 🛠️ Possible Improvements
Add an AI opponent

Improve rules (e.g., multi-jumps, forced jumps)

Add a graphical user interface (GUI) using WinForms or WPF

Implement saving and loading of game state

