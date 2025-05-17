# Blob Evolution Game

A browser-based evolution game where you guide and train a blob through different biomes, helping it evolve and develop new traits.

## Features

- Multiple biomes (Desert, Water, Mountains, Forest)
- Evolution system with unique traits
- Food gathering and training mechanics
- Inventory system
- Dynamic evolution based on environment
- Pet taming and training system
- Building mechanics
- Character progression

## How to Play

1. Open `blob-evolution/standalone.html` in a web browser
2. Use WASD or arrow keys to move

### Controls
- **Arrow Keys/WASD**: Move your character
- **G**: Toggle collection mode (automatically collect items in range)
- **B**: Toggle build mode (build structures)
- **N**: While in build mode, cycle through building types
- **N**: When a blob is tamed as a pet, name your pet
- **I**: Toggle inventory view
- **Click** on inventory items to select them for use
- **R**: Restart game if your blob dies

### Biomes and Their Effects

Each biome affects your blob differently:
- **Forest**: Balanced temperature, food includes berries and nuts
- **Desert**: Very hot, reduces energy faster, food includes cactus
- **Water**: Cools blob, reduces movement speed unless blob has fins, food includes fish
- **Mountains**: Very cold, reduces movement speed unless blob has fur, food includes minerals

### Stats and Survival

Your blob's stats are interconnected and critical for survival:

- **Hunger**: Decreases over time (6% per second). When below 45%, energy drains faster. Below 25%, health starts decreasing. Keep fed by collecting food.

- **Energy**: Decreases while moving (3.8 per second) and more slowly when stationary (2.2% per second when hungry). When energy falls below 20%, health starts decreasing. Completely depleted energy causes rapid health loss.

- **Temperature**: Affected by biomes. Extreme temperatures (below 8°C or above 32°C) drain energy faster. Very extreme temperatures (below 3°C or above 37°C) cause health damage.

- **Health**: Reaches zero when your blob dies. Naturally regenerates only under excellent conditions (high hunger, energy, and comfortable temperature).

### Evolution System

Your blob evolves based on:
- Experience gained from eating food
- Time spent in specific biomes
- Types of food consumed

Each evolution level grants new traits and abilities:
- **Level 1 (Tamed Blob)**: Adaptation to dominant biome
- **Level 2 (Friendly Blob)**: Adaptation based on diet preference
- **Level 3 (Loyal Blob)**: Special abilities, significantly faster movement
- **Level 4 (Companion Blob)**: Enhanced speed and environmental mastery
- **Level 5 (Guardian Blob)**: Advanced abilities and maximum speed

## Development

The game is built using vanilla JavaScript and HTML5 Canvas.

### File Structure

- `blob-evolution/` - Main game directory
  - `standalone.html` - Complete game file
  - `assets/` - Game assets and resources

## Backup Instructions

1. Regular commits should be made after significant changes
2. Use descriptive commit messages
3. Push to remote repository regularly
4. Keep local backups of the repository

## Version History

### v1.0.0 - Initial Release
- Basic blob movement and physics system
- Simple canvas rendering
- Basic game loop implementation

### v1.1.0 - Core Systems
- Added inventory system with item management
- Implemented item rarity system (common, uncommon, rare, epic, legendary)
- Added custom item icons and drawing system
- Basic UI elements and inventory display

### v1.2.0 - Biome System
- Implemented biome-specific traits and effects
- Added temperature effects for different biomes
- Biome-specific resource distribution
- Environmental interactions

### v1.3.0 - Evolution Mechanics
- Added evolution system based on biome interactions
- Implemented trait development
- Added inventory capacity upgrades through evolution
- Biome-specific evolution paths

### v1.4.0 - Game Mechanics
- Added death and restart mechanics
- Implemented resource gathering system
- Added building materials system
- Enhanced UI with item details and tooltips

### v1.5.0 - Mobile Optimization
- Optimized UI for mobile devices
- Adjusted inventory layout for better mobile experience
- Improved touch controls
- Enhanced visual feedback for mobile interactions

### v1.6.0 - Pet System
- Added ability to tame blobs as pets
- Implemented pet evolution paths
- Added pet naming feature
- Created loyalty and training mechanics

### v1.7.0 - Building System
- Added construction mechanics
- Implemented resource consumption for building
- Created multiple structure types
- Added building progression system

### v1.8.0 - Collection Mode
- Added automatic collection mode (toggle with G key)
- Implemented collection radius visualization
- Added visual feedback for collected items
- Improved resource gathering experience

### v1.9.0 - Speed Enhancements
- Adjusted blob speed progression through evolution levels
- Implemented specific speed values for each evolution stage:
  - Level 0 (Wild): 0.8
  - Level 1 (Tamed): 0.95
  - Level 2 (Friendly): 1.1
  - Level 3 (Loyal): 1.7
  - Level 4 (Companion): 2.1
  - Level 5+ (Guardian): 2.5

### v2.0.0 - Difficulty Balance (Current)
- Increased hunger decay rate from 4.0% to 6.0% per second
- Increased energy decay rate from 1.5% to 2.2% per second when not moving
- Increased movement energy cost from 2.5 to 3.8
- Raised health decay rate from 0.3% to 0.45% per second in bad conditions
- Adjusted hunger and energy thresholds for health penalties
- Enhanced temperature effects on health and energy
- Fine-tuned overall game difficulty for better challenge 