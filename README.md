# connect 4

A classic Connect 4 game built with HTML, CSS, and JavaScript.

<div align="center">
  <img src="https://github.com/annagornyitzki/connect4/blob/main/connect4-gameplay.png?raw=true" width="550"/>
</div>

**Gameplay**
- Red goes first  
- Click any column to drop a piece  
- Get four in a row to win  
- Board automatically resets after a win or draw  
- Press **Restart** to start a new match at any time

Play it here: **[Live Game](https://annagornyitzki.github.io/connect4/)**

## Overview
This project is an interactive browser-based Connect 4 game where two players compete to line up four pieces horizontally, vertically, or diagonally. The game features automatic win detection, a restart button, and a wipe-board animation that resets the grid after the match ends.


## Project Structure
- `index.html`: The main HTML file that serves as the entry point for the game.
- `connect4.css`: Contains the styles for the game interface.
- `connect4.js`: The main JavaScript file that contains the game logic.

## Game Logic
Implemented in **`connect4.js`** as follows:
- **Board Initialization**  
  Creates a 6×7 grid dynamically and manages open slots using a tracking array.
- **Turn Management**  
  Players alternate between **Red** and **Yellow** pieces.
- **Win & Draw Detection**  
  Checks for four in a row horizontally, vertically, and along both diagonals.
- **Wipe Board Animation**  
  After a victory or draw, the board clears automatically and rebuilds itself.
- **Manual Restart**  
  A button allows players to reset instantly without waiting.

## UI/UX Design

The interface focuses on clean visuals and responsive interaction:

- **Circular tile design** to mimic real Connect 4 pieces  
- **Blue game board** with a navy border for high contrast  
- **Soft mint patterned background** to match the game’s playful theme  
- **Restart button hover** for better user engagement

## How to Run

1. Play it here [Live Game](https://annagornyitzki.github.io/connect4/)**
2. Open `index.html` in a web browser to start the game.
