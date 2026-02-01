# Super Crossy Bros: Bug Fix Edition 🎮

A Python pygame 2D platformer game inspired by the classic Mario. Players need to jump upward through multiple rows of obstacles, including moving enemies, cloud platforms, and coins, to reach the pipes at the top.

## Features

✨ **Gameplay**
- **Multi-level Stages**: 12 different game areas including:
  - 🏠 Start Zone (bottom)
  - 🛣️ Two Traffic Lanes (lower and upper)
  - ☁️ Cloud Platform Zone (requires jumping on clouds)
  - 🌱 Safe Rest Areas
  - 🏁 Goal Zone (enter pipes to win)

- **Enemy Types**:
  - 🍄 Goomba (brown enemies)
  - 💥 Bullets (black fast enemies)
  - Various speeds and directions

- **Collection System**:
  - 💰 Coins: +1 point each
  - 🔴 Pipes: +5 points and advance to next level

- **Mario-style Visual Design**:
  - Pixel-art Mario character (hat, mustache, body)
  - Classic color scheme
  - Environmental elements: bricks, grass, pipes, clouds

## Game Controls

1. **Movement**:
   - ⬆️ UP Arrow - Move up
   - ⬇️ DOWN Arrow - Move down
   - ⬅️ LEFT Arrow - Move left
   - ➡️ RIGHT Arrow - Move right

2. **Win Condition**:
   - Reach the pipes at the top and enter them
   - Gain 5 points for completing each level

3. **Lose Condition**:
   - Collide with enemies → Game Over
   - Fall off platforms in cloud zones → Game Over

4. **Restart Game**:
   - Press `SPACEBAR` after game over to restart

## Technical Implementation

### Core Classes

- **Player** - Character control and rendering
- **Enemy** - Enemy spawning, movement, and rendering
- **Cloud** - Cloud platform logic
- **Coin** - Collectible coins
- **Pipe** - Goal pipes for winning
- **GameManager** - Core game logic, collision detection, and level management

### Key Features

- ✅ Precise collision detection system
- ✅ Cloud platform mechanics (active in specific rows)
- ✅ Randomized enemy and coin generation
- ✅ 60 FPS game loop
- ✅ Score tracking system

## Installation & Setup

### Requirements
- Python 3.7+
- pygame

### Install Dependencies
```bash
pip install pygame
```

### Run the Game
```bash
python game
```

## File Structure
```
game/
├── README.md          # This file
└── game              # Main game file (Python script)
```

## Game Parameters

Main customizable parameters in the code:

```python
GRID_SIZE = 50           # Grid size (pixels)
SCREEN_WIDTH = 800       # Screen width
SCREEN_HEIGHT = 700      # Screen height
FPS = 60                # Game frame rate
```

## Color Palette

Game uses a Mario-themed color scheme:
- 🔵 Sky Blue - Background
- 🟤 Brick Brown - Bricks
- 🔴 Mario Red - Hat and decorations
- 🟦 Mario Blue - Body
- 🟢 Pipe Green - Pipes
- ⭐ Coin Gold - Coins

## Bug Fixes

This version includes the following fixes:
1. ✅ Fixed collision detection offset in cloud platform rows
2. ✅ Increased cloud density for better gameplay

## License

Open source project