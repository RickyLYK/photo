# COMP2113-GroupPrj-Boaz-Ricky

## Team Members
- LI Yik Kei - 3036370786
- LAI Kwan Yu - 3036327040

## Application Description
**2048 Boss Battle** is an revolutionized 2048 puzzle game. It combines number merging mechanics with boss fighting elements. Players merge  tiles to get attack power and tr to defeat the boss. The ultimate goal is to have teh sum of all tiles' values greather than boss's health.

## Features

### Core Gameplay
- **Classic 2048 Mechanics** - Slide and combine tiles
- **Boss Battle** - Each tile sums up damage to attack the boss
- **Multiple Difficulty Levels** - Easy (3000 HP) and Hard (6000 HP) modes
- **Dynamic Board Sizes** - 4x4 (Classic) and 5x5 (Challenge) boards

### User System
- **User Registration & Login** - Persistent player accounts
- **Leaderboard** - Global ranking system
- **Save/Load System** - Automatic progress saving

### Technical Features
- **Cross-Platform** - Works on Windows, Linux. and Mac
- **Visual Feedback** - Color-coded tiles and ASCII art
- **Intuitive Controls** - WASD keys for movement

## Compilation and Execution

### Prerequisites
- g++ compiler (pre-defined using C++11 as version)

### Compilation
```bash
make
./2048
```

### Quick Start
1. **Run** the executable: `./2048`
2. **Register** new account or **Login** with existing user
3. **Choose** from main menu: New Game, Resume Game, or Leaderboard
4. **Select** game mode (Easy/Hard) and board size (4x4/5x5)
5. **Play** using WASD keys:
   - `W` - Move Up
   - `A` - Move Left  
   - `S` - Move Down
   - `D` - Move Right
   - `Q` - Save and Quit, `Y` to confirm or `N` to cancel quit

## Game Rules
- Combine tiles with same numbers to double their value
- Each tile combination deals damage to the boss
- Defeat the boss by reducing its health to zero
- Game ends when no more moves are possible
- All data persists between game sessions
