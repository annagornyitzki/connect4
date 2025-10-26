# connect 4

A classic Connect 4 game built with HTML, CSS, and JavaScript featuring an intelligent AI opponent.

<div align="center">
  <img src="https://github.com/annagornyitzki/connect4/blob/main/connect4-gameplay.png?raw=true" width="550"/>
</div>

**Gameplay**
- Play as **Red** against an AI opponent (**Yellow**)
- Click any column to drop a piece  
- AI responds automatically with strategic moves
- Get four in a row to win  
- Board automatically resets after a win or draw  
- Press **Restart** to start a new match at any time

Play it here: **[Live Game](https://annagornyitzki.github.io/connect4/)**

## Overview
This project is an interactive browser-based Connect 4 game where you compete against an AI opponent to line up four pieces horizontally, vertically, or diagonally. The game features intelligent AI decision-making, automatic win detection, a restart button, and a wipe-board animation that resets the grid after the match ends.

## AI Features
The AI opponent uses **minimax algorithm with alpha-beta pruning** to make intelligent moves:
- **Look-ahead depth**: Evaluates moves 4 turns ahead
- **Strategic positioning**: Prioritizes center column control
- **Defensive play**: Blocks opponent winning moves
- **Offensive play**: Seeks winning combinations
- **Natural timing**: 600ms delay for realistic gameplay feel
  
## Project Structure
- `index.html`: The main HTML file that serves as the entry point for the game.
- `connect4.css`: Contains the styles for the game interface.
- `connect4.js`: The main JavaScript file that contains the game logic.

## Game Logic
Implemented in **`connect4.js`** as follows:
- **Board Initialization**  
  Creates a 6×7 grid dynamically and manages open slots using a tracking array.
- **Turn Management**  
  Human player (Red) alternates with AI opponent (Yellow).
- **AI Decision Engine**  
  Uses minimax algorithm to evaluate board positions and select optimal moves.
- **Board Evaluation**  
  Scores positions based on winning patterns, center control, and blocking opportunities.
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

1. Play it here [Live Game](https://annagornyitzki.github.io/connect4/)
2. Open `index.html` in a web browser to start the game.

## Technical Details
- **No dependencies**: Pure vanilla JavaScript, HTML, and CSS
- **No build tools**: Run directly in any modern browser
- **Minimax depth**: Configurable (default: 4 for balanced performance/difficulty)
- **Alpha-beta pruning**: Optimizes AI performance by eliminating unnecessary calculations
