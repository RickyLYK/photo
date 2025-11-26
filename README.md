# 2048 Boss Battle - COMP2113 Course Project

## Team Members
- [Team Member 1 Name] - [Student ID]
- [Team Member 2 Name] - [Student ID] 
- [Team Member 3 Name] - [Student ID]
- [Team Member 4 Name] - [Student ID]

## Application Description
**2048 Boss Battle** is an innovative twist on the classic 2048 puzzle game, combining tile-matching mechanics with RPG boss fighting elements. Players combine numbered tiles to generate attack power against a formidable boss monster, with the goal of reducing the boss's health to zero by reaching high-value tile combinations.

## Features

### Core Gameplay
- 🎮 **Classic 2048 Mechanics** - Slide and combine numbered tiles
- ⚔️ **Boss Battle System** - Each tile combination damages a boss monster
- 🎯 **Multiple Difficulty Levels** - Easy (3000 HP) and Hard (6000 HP) modes
- 📊 **Dynamic Board Sizes** - 4x4 (Classic) and 5x5 (Challenge) options

### User System
- 👤 **User Registration & Login** - Persistent player accounts
- 🏆 **Leaderboard** - Global ranking system
- 💾 **Save/Load System** - Automatic progress saving

### Technical Features
- 🖥️ **Cross-Platform** - Works on Windows and Linux
- 🎨 **Visual Feedback** - Color-coded tiles and ASCII art
- ⌨️ **Intuitive Controls** - WASD keys for movement

## Coding Requirements Implementation

| Requirement | Implementation | Features Supported |
|-------------|----------------|-------------------|
| **Random Events** | `generate_tile_value()` function | Random tile spawning (2 or 4) |
| **Data Structures** | `Player` struct, 2D arrays, vectors | User profiles, game state, rankings |
| **Dynamic Memory** | `initialize_board()`, `cleanup_board()` | Dynamic board allocation |
| **File I/O** | `file_operations.cpp` | Save/load game, player progress |
| **Multiple Files** | 10+ organized header/source files | Modular code structure |
| **Difficulty Levels** | Easy (3000 HP) and Hard (6000 HP) | Adjustable game challenge |

## Non-Standard Libraries
This project uses only **standard C++ libraries** with no additional dependencies:
- `<iostream>`, `<fstream>`, `<vector>`, `<algorithm>`, `<cstdlib>`, `<ctime>`, `<iomanip>`

## Compilation and Execution

### Prerequisites
- GCC/G++ compiler (C++11 compatible)

### Compilation
```bash
# Using Makefile
make

# Or manual compilation
g++ -std=c++11 -o 2048_game *.cpp
```

### Execution
```bash
./2048_game
```

### Quick Start
1. **Compile** the program using the instructions above
2. **Run** the executable: `./2048_game`
3. **Register** new account or **Login** with existing credentials
4. **Choose** from main menu: New Game, Resume Game, or Leaderboard
5. **Select** game mode (Easy/Hard) and board size (4x4/5x5)
6. **Play** using WASD keys:
   - `W` - Move Up
   - `A` - Move Left  
   - `S` - Move Down
   - `D` - Move Right
   - `Q` - Save and Quit

## Game Rules
- Combine tiles with same numbers to double their value
- Each tile combination deals damage to the boss
- Defeat the boss by reducing its health to zero
- Game ends when no more moves are possible

## File Structure
```
project/
├── main.cpp              # Program entry point
├── function.h/cpp        # Core game logic
├── graphics.h/cpp        # UI and visual elements
├── file_operations.h/cpp # Save/load system
├── login.h/cpp           # User authentication
├── register.h/cpp        # User registration
├── menu.h/cpp            # Navigation menus
├── leaderboard.h/cpp     # Ranking system
├── player.h              # Data structures
├── Makefile              # Build instructions
└── player_base.txt       # Player database (auto-generated)
```

## Technical Notes
- Program automatically creates `player_base.txt` for data storage
- Game progress saves automatically when quitting
- Cross-platform console clearing supported
- All data persists between game sessions

---

**Developed for COMP2113 Programming Technologies - 2025/2026 1st Semester**
