# ⚔️ HexBlade

A 2D pixel-art turn-based fighting game featuring magical fantasy combat between two players. Choose your character class, master your abilities, and defeat your opponent in strategic tactical battles.

![Game Type](https://img.shields.io/badge/Type-Turn--Based%20Fighter-blue)
![Players](https://img.shields.io/badge/Players-2-green)
![Style](https://img.shields.io/badge/Style-Pixel%20Art-purple)
![Language](https://img.shields.io/badge/Language-C++-00599C?logo=cplusplus)

## 🎮 Game Overview

HexBlade is a turn-based combat game where players select from distinct character classes and battle using unique abilities and items. Each class offers a different playstyle, requiring players to think strategically about their moves and resource management.

### Character Classes

- **⚔️ Warrior** - Powerful melee combatant with high defense and devastating physical attacks
- **🗡️ Rogue** - Agile fighter specializing in critical hits and evasive maneuvers
- **🌿 Druid** - Nature-wielding spellcaster with healing and elemental abilities
- **✨ More classes to discover...**

### Core Features

- ✨ **Pixel Art Graphics** - Nostalgic 2D pixel art aesthetic
- 🎯 **Turn-Based Combat** - Strategic gameplay with careful planning
- 🎭 **Multiple Character Classes** - Unique abilities and playstyles
- 📦 **Item System** - Collectible and usable items to turn the tide of battle
- 🖼️ **Graphical Interface** - Intuitive and visually appealing UI
- 🎪 **2-Player Battles** - Face off against a friend in local combat

## 🏗️ Object-Oriented Design

HexBlade is built using robust OOP principles and design patterns to ensure maintainable, extensible, and clean code architecture.

### OOP Paradigms & Techniques Implemented

#### **Encapsulation**
- Each character class encapsulates its own stats, abilities, and behaviors
- Private attributes with public accessor methods ensure data integrity
- Item and ability systems maintain internal state management

#### **Inheritance**
- Abstract base `Character` class defines common properties (HP, attack, defense)
- Specific classes (`Warrior`, `Rogue`, `Druid`) inherit and extend base functionality
- Shared combat mechanics inherited across all character types
- Item hierarchy with base `Item` class extended by specific item types

#### **Polymorphism**
- Unified interface for all character actions through method overriding
- Different character classes implement unique versions of `attack()`, `useAbility()`, and `takeDamage()`
- Items can be used polymorphically regardless of their specific type
- Combat system treats all characters uniformly while respecting their unique behaviors

#### **Abstraction**
- Abstract `Character` class defines the contract for all playable characters
- Combat mechanics abstracted into reusable methods
- Game state management separated from rendering logic
- Clear separation between game logic and UI layers

### Design Patterns Used

- **Factory Pattern** - Character and item creation
- **Strategy Pattern** - Ability execution and combat calculations
- **Observer Pattern** - UI updates responding to game state changes
- **Singleton Pattern** - Game state and resource management

### Code Organization

```
HexBlade/
├── src/
│   ├── characters/          # Character classes and base abstractions
│   │   ├── Character.h      # Abstract base class
│   │   ├── Character.cpp
│   │   ├── Warrior.h
│   │   ├── Warrior.cpp
│   │   ├── Rogue.h
│   │   ├── Rogue.cpp
│   │   ├── Druid.h
│   │   └── Druid.cpp
│   ├── items/              # Item system
│   ├── combat/             # Combat mechanics and turn management
│   ├── ui/                 # Graphical interface components
│   └── main.cpp            # Entry point
├── assets/                 # Sprites and pixel art resources
├── include/                # Header files
└── CMakeLists.txt          # Build configuration
```

## 🚀 Getting Started

### Prerequisites

- C++ compiler (GCC 9+ or Clang 10+)
- CMake 3.15 or higher
- SDL2 or SFML (for graphics rendering)

### Installation & Running

1. Clone the repository:
```bash
git clone https://github.com/yourusername/HexBlade.git
cd HexBlade
```

2. Build and run:
```bash
mkdir build && cd build
cmake ..
make
./HexBlade
```

## 🎯 How to Play

1. **Select Your Character** - Each player chooses their character class
2. **Take Turns** - Players alternate turns in combat
3. **Choose Actions** - Attack, use abilities, or consume items
4. **Strategic Combat** - Manage health, resources, and timing
5. **Victory** - Reduce opponent's HP to zero to win!

## 🛠️ Technical Highlights

- **Clean Architecture** - Separation of concerns between game logic, data, and presentation
- **SOLID Principles** - Adherence to industry-standard design principles
- **Extensibility** - Easy to add new characters, abilities, and items
- **Maintainability** - Well-documented code with clear class responsibilities

## 🔮 Future Enhancements

- [ ] Additional character classes
- [ ] More diverse item types
- [ ] Special combo abilities
- [ ] Tournament mode
- [ ] Enhanced visual effects
- [ ] Sound effects and music

## 👥 Contributing

Contributions are welcome! Feel free to submit pull requests or open issues for bugs and feature requests.

## 📜 License

This project is open source and available under the MIT License.

## 👨‍💻 Authors

*Add your name(s) here*

---

**Enjoy the battle in HexBlade!** ⚔️✨
