# CSC8507 - Advanced Game Technologies

A C++ 3D game development project developed as part of the Advanced Game Technologies module at Newcastle University.

This project explores core game programming concepts, including game physics, collision detection, artificial intelligence, networking, rendering and gameplay systems. It builds upon the Newcastle University game technology framework and extends it with custom gameplay mechanics and interactive game environments.

## Overview

The project implements a 3D game environment featuring player interactions, multiple levels, collectibles, enemy AI, boss encounters and gameplay progression.

The primary focus is on applying game development principles through C++ and object-oriented programming, with an emphasis on implementing and integrating different game systems.

## Features

- **3D Game Environment:** Interactive environments with multiple levels and gameplay areas.
- **Player System:** Player health, collectibles, inventory management and item usage.
- **Gameplay Mechanics:** Pickups, power-ups, doors, level transitions and interactive objects.
- **Artificial Intelligence:**
  - State machine-based enemy behaviour.
  - Behaviour tree-based boss AI.
  - Player tracking, chasing and attack behaviours.
- **Physics and Collision Detection:** Object interactions, collision responses and physics-based gameplay.
- **Networking:** Client-server architecture and network communication using ENet.
- **Rendering:** 3D rendering using OpenGL, with optional Vulkan rendering support.
- **Audio:** Sound management and audio integration using FMOD.

## Technology Stack

| Category | Technologies |
|---|---|
| Programming Language | C++ |
| Graphics API | OpenGL, Vulkan (optional) |
| Build System | CMake |
| IDE | Visual Studio |
| AI | State Machines, Behaviour Trees |
| Physics | Custom Physics Framework |
| Networking | ENet, Client-Server Architecture |
| Audio | FMOD |
| Version Control | Git |

## Project Structure

```text
CSC8507/
│
├── Assets/                 # Game assets, models, textures and shaders
│
├── CMake/                  # CMake configuration utilities
│
├── CSC8503/                # Main game application
│   ├── Main.cpp
│   ├── GameLevel.cpp
│   ├── Player.cpp
│   ├── Boss.cpp
│   ├── GhostAI.cpp
│   ├── Door.cpp
│   ├── Coin.cpp
│   ├── SoundManager.cpp
│   └── NetworkedGame.cpp
│
├── CSC8503CoreClasses/     # Gameplay and engine systems
│   ├── AI/
│   ├── Physics/
│   ├── Collision Detection/
│   └── Networking/
│
├── NCLCoreClasses/         # Core mathematical and engine utilities
│
├── OpenGLRendering/        # OpenGL rendering implementation
│
├── VulkanRendering/        # Optional Vulkan rendering implementation
│
├── SOIL/                   # Image loading library
├── externals/              # External dependencies
│
├── CMakeLists.txt
└── CSC8503.sln
```

## Getting Started

### Requirements

The project is configured primarily for Windows development.

- Windows 10 or later
- Visual Studio 2022 with C++ development tools
- CMake 3.16 or later
- C++20 compatible compiler
- Required external libraries and dependencies included or referenced in the repository

### Building the Project

**Option 1: Visual Studio**

1. Clone the repository:

   ```bash
   git clone https://github.com/ayeshatazeen1/CSC8507.git
   ```

2. Navigate to the project directory.

3. Open `CSC8503.sln` in Visual Studio 2022.

4. Select the `x64` platform and choose either `Debug` or `Release` configuration.

5. Build the solution.

6. Run the `CSC8503` startup project.

**Option 2: CMake**

Generate the Visual Studio solution using:

```bash
cmake -S . -B build -A x64
```

Build the project using:

```bash
cmake --build build --config Release
```

Note: The project uses external dependencies, including FMOD. Ensure the required libraries and runtime components are available and correctly configured before building.

## Key Areas of Implementation

### Artificial Intelligence

The project explores different AI architectures for controlling game entities.

- State machines for enemy movement, patrolling and player pursuit.
- Behaviour trees for boss decision-making.
- Distance-based conditions for switching between AI states.
- Chase, attack and ranged attack behaviours.

### Gameplay Systems

The player system supports health management, collectible tracking and inventory-based item usage. Interactive objects and gameplay events contribute to level progression and player interaction.

### Physics and Collision

The project uses game object transformations, collision volumes and physics systems to manage interactions between objects in the 3D environment.

### Networking

Network functionality is implemented using a client-server architecture, supported by ENet for network communication.

## Learning Outcomes

This project provided practical experience in:

- Object-oriented programming and C++ game architecture.
- Implementing AI using state machines and behaviour trees.
- Understanding physics, collision detection and object interactions.
- Developing modular gameplay systems.
- Working with graphics APIs and rendering pipelines.
- Understanding network communication and multiplayer architecture.
- Integrating external libraries into a C++ application.

## License and Attribution

This repository builds upon the Newcastle University CSC8503 game technology framework.

The original framework includes work by its respective contributors. Refer to the [LICENSE](LICENSE) file for licensing information.

---

**Author:** Ayesha Tazeen

**Module:** Advanced Game Technologies
