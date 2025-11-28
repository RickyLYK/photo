# COMP2113-GroupPrj-Boaz-Ricky

## Team Members
- LI Yik Kei - 3036370786
- LAI Kwan Yu - 3036327040

## Application Description
**2048 Boss Battle** is an innovative twist on the classic 2048 puzzle game that combines number merging mechanics with RPG boss fighting elements. Players merge numbered tiles to generate attack power and battle against a formidable boss. The goal is to reduce the boss's health to zero by achieving a tile sum greater than its maximum health.

## Features

### Core Gameplay
- **Classic 2048 Mechanics** - Slide and combine tiles using WASD controls
- **Boss Battle System** - Each tile contributes to damaging the boss
- **Multiple Difficulty Levels** - Easy and Hard modes with different boss health values
- **Dynamic Board Sizes** - 4x4 (Classic) and 5x5 (Challenge) boards
- **Real-time Health Display** - Visual boss health bar with ASCII art

### User System
- **User Registration & Login** - Persistent player accounts with saved progress
- **Global Leaderboard** - Competitive ranking system tracking high scores
- **Auto-save System** - Automatic progress saving during gameplay

### Technical Implementation
- **Cross-Platform Compatibility** - Works on Windows, Linux, and Mac systems
- **Visual Feedback** - Color-coded tiles and dynamic ASCII boss art
- **File Persistence** - Player data and game states saved between sessions

## Coding Requirements Implementation

### 1. Generation of Random Events
- **Implementation**: `generate_tile_value()` and `add_random_tile()` functions
- **Purpose**: Randomly spawns new tiles (values 2 or 4) in empty positions after each move
- **Feature Support**: Core gameplay mechanics and unpredictability

### 2. Data Structures for Storing Data
- **Implementation**: `struct Player`, `struct LeaderboardEntry`, 2D dynamic arrays for game board
- **Purpose**: Organizes player data, leaderboard entries, and game state information
- **Feature Support**: User profiles, score tracking, and game state management

### 3. Dynamic Memory Management
- **Implementation**: `initialize_board()` and `cleanup_board()` functions using `new`/`delete`
- **Purpose**: Dynamically allocates and deallocates memory for game boards of different sizes
- **Feature Support**: Flexible board sizing and memory efficiency

### 4. File Input/Output
- **Implementation**: `save_game()`, `load_game()`, `save_player_progress()` in `file_operations.cpp`
- **Purpose**: Saves/loads game states and player data to `player_base.txt`
- **Feature Support**: Persistent user accounts and game progression

### 5. Program Codes in Multiple Files
- **Implementation**: Modular code structure with separate header and implementation files
- **Files**: `main.cpp`, `function.cpp`, `file_operations.cpp`, `leaderboard.cpp`, `login.cpp`, `register.cpp`, `menu.cpp`, `graphics.cpp`
- **Purpose**: Organized codebase for maintainability and collaboration

### 6. Multiple Difficulty Levels
- **Implementation**: `set_boss_health()` and `choose_gamemode()` functions
- **Levels**: Easy (3000/20000 HP) and Hard (6000/40000 HP) based on board size
- **Feature Support**: Adjustable challenge levels for different player skills

## Non-Standard Libraries
- **None** - This project uses only standard C++ libraries (`iostream`, `fstream`, `vector`, `algorithm`, `iomanip`, `cstdlib`, `ctime`, `string`) that don't require additional installation.

## Compilation and Execution

### Prerequisites
- g++ compiler (supporting C++11 standard)
- Terminal/Command Prompt with ANSI escape code support for colors

### Compilation
```bash
make
