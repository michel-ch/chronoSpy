# GameJam 2024: ChronoSpy

## About the Game
ChronoSpy is a 2D maze game where a time-powered secret agent must navigate through 2 levels with the objective of defusing a bomb while escaping from laboratory guards. Across both levels, the agent will have different objectives, with the final goal of escaping the lab within a time limit that can be manipulated using special abilities.

The chronometer represents the bomb's timer. This timer can be slowed down by collecting bonuses that the agent picks up throughout the maze.

When collecting a bonus placed in the labyrinth, time stops for a short duration (10 seconds).

## Game Levels

### First Level:
The agent must first navigate through the maze and collect a code that allows them to defuse the bomb placed in the 2nd level, all while escaping from enemies.
- A checkpoint is placed in the maze that allows saving the current moment and returning to it by pressing **C**
- If enemies are alerted (the agent enters their field of vision), all enemies will chase the player
- If the agent collects the code, they proceed to the second level
- If the agent gets touched by an enemy, they lose

### Second Level:
The goal of this level is to defuse the bomb. The agent navigates through the maze, still escaping from enemies in the same manner, and must reach the bomb.
Once the bomb is defused, a door appears in the maze allowing the agent to escape.

## Time Management:
Time management comes with the player's abilities:
- **Time Stop**: Temporarily freeze time
- **Time Travel**: Return to a saved checkpoint

## Requirements

### System Requirements
- Python 3.7 or higher
- Windows, macOS, or Linux

### Python Dependencies
- pygame
- numpy

## Installation & Setup

### 1. Clone or Download the Repository
```bash
git clone <repository-url>
cd chronoSpy
```

### 2. Install Python Dependencies

#### Option A: Using requirements.txt (Recommended)
```bash
# Install all dependencies at once
pip install -r requirements.txt
```

#### Option B: Using virtual environment (Best practice)
```bash
# Create virtual environment
python -m venv chronospy-env

# Activate virtual environment
# On Windows:
chronospy-env\Scripts\activate
# On macOS/Linux:
source chronospy-env/bin/activate

# Install dependencies from requirements file
pip install -r requirements.txt
```

#### Option C: Manual installation
```bash
pip install pygame numpy
```

### 3. Verify Installation

#### Check Dependencies
```bash
# Verify pygame installation
python -c "import pygame; print('pygame version:', pygame.version.ver)"

# Verify numpy installation
python -c "import numpy; print('numpy version:', numpy.__version__)"
```

#### File Structure
Make sure all game assets are present in your directory:
```
chronoSpy/
├── main.py                 # Main game file
├── requirements.txt        # Python dependencies
├── README.md              # This file
├── data/                  # Game assets
│   ├── blocks/           # Block sprites
│   ├── font/             # Game fonts
│   ├── items/            # Item sprites
│   ├── menu/             # Menu graphics
│   ├── people/           # Character sprites
│   └── portail/          # Portal sprites
└── sounds/               # Audio files
    ├── background_music.wav
    ├── alert.wav
    └── ... (other sound files)
```

## How to Run

### Starting the Game
Navigate to the game directory and run:

```bash
python main.py
```

### Game Controls
- **Arrow Keys** or **WASD**: Move the agent
- **C**: Return to saved checkpoint (time travel)
- **Space**: Stop time (when bonus is collected)
- **ESC**: Pause/Resume game

### Gameplay Tips
1. **Stealth**: Avoid entering guards' line of sight to prevent alerting them
2. **Checkpoints**: Use checkpoints strategically to save your progress
3. **Time Management**: Collect bonuses to slow down the bomb timer
4. **Code Collection**: In level 1, find and collect the code before proceeding
5. **Bomb Defusal**: In level 2, reach the bomb to defuse it and open the escape door

## Troubleshooting

### Common Issues

**Game doesn't start / Import errors:**
- Make sure Python 3.7+ is installed
- Verify pygame and numpy are installed: `pip list | grep pygame` and `pip list | grep numpy`
- Try reinstalling dependencies: `pip install --upgrade pygame numpy`

**No sound:**
- Check system audio settings
- Ensure sound files exist in the `sounds/` directory

**Graphics issues:**
- Update your graphics drivers
- Try running in different display modes

**Performance issues:**
- Close other resource-intensive applications
- Ensure adequate system resources are available

### Getting Help
If you encounter issues:
1. Check that all game files are present and unmodified
2. Verify Python and dependency versions
3. Check the console for error messages
4. Ensure proper file permissions

## Game Features
- **2D Maze Navigation**: Navigate through complex labyrinths
- **Stealth Gameplay**: Avoid guard detection
- **Time Manipulation**: Use special abilities to control time
- **Multiple Levels**: Progress through different challenges
- **Checkpoint System**: Save and restore game states
- **Audio**: Immersive sound effects and background music
- **Pixel Art Graphics**: Retro-style visual design

## Development
This game was created for GameJam 2024 using:
- **Python**: Core game logic
- **Pygame**: Game engine and graphics
- **NumPy**: Maze data structure and calculations

---

Enjoy playing ChronoSpy! 🕵️‍♂️⏰
