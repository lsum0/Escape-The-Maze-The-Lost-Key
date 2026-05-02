# 🚪 Escape The Maze – The Lost Key

> A 2D OpenGL adventure game demonstrating core Computer Graphics concepts through interactive gameplay with immersive audio effects.

<p align="center">
  <img src="https://img.shields.io/badge/Language-C%2B%2B-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Graphics-OpenGL-green?style=for-the-badge">
  <img src="https://img.shields.io/badge/Framework-GLUT-orange?style=for-the-badge">
  <img src="https://img.shields.io/badge/Course-CS2206-purple?style=for-the-badge">
  <img src="https://img.shields.io/badge/Project-Completed-success?style=for-the-badge">
</p>

<p align="center">
  <b>Built with Computer Graphics fundamentals using OpenGL & GLUT</b>
</p>

---

## Project Description :

**Escape The Maze – The Lost Key** is a 2D adventure maze game developed using **C++ and OpenGL/GLUT**.

The player wakes up inside a mysterious maze and must collect **three hidden keys**, avoid traps and enemies, and escape through the exit door before the timer reaches zero.

This project applies core Computer Graphics concepts through a complete interactive game experience.

---

## Table of Contents :

* [Gameplay Demo](#-gameplay-demo)
* [Screenshots](#-screenshots)
* [Game Flow](#-game-flow-)
* [Code Architecture](#-code-architecture)
* [Characters](#-characters)
* [Game Objects](#-game-objects--)
* [Gameplay Features](#-gameplay-features)
* [Computer Graphics Concepts Applied](#-computer-graphics-concepts-applied-)
* [Controls](#-controls-)
* [Repository Structure](#-repository-structure)
* [How to Run](#-how-to-run)
* [References](#-references)
* [Team Members](#-team-members-)

---

## Gameplay Demo 🎥 :

<p align="center">
  <img src="objects/Play.gif" width="850">
</p>

<p align="center">
  <b>Escape The Maze – Live Gameplay Preview</b>
</p>

---

## Screenshots :

A quick preview of the game's main scenes and gameplay experience.

| Main Menu                                    | How To Play                                         |
| -------------------------------------------- | --------------------------------------------------- |
| <img src="screenshots/menu.png" width="430"> | <img src="screenshots/how-to-play.png" width="430"> |

| Gameplay                                         | Victory                                         |
| ------------------------------------------------ | ----------------------------------------------- |
| <img src="screenshots/gameplay.png" width="430"> | <img src="screenshots/victory.png" width="430"> |

| Game Over                                         | Gameplay Demo                            |
| ------------------------------------------------- | ---------------------------------------- |
| <img src="screenshots/game-over.png" width="430"> | <img src="objects/Play.gif" width="430"> |

---

## 🧩 Game Flow

<p align="center">
  <img width="750" src="diagrams/Game Flow.png" alt="Game Flow">
</p>

```text
Main Menu
   ↓
How To Play
   ↓
Intro
   ↓
Gameplay
   ↓
Collect 3 Keys
   ↓
Unlock Door
   ↓
Victory / Game Over
```

---

## Code Architecture :

<p align="center">
  <img width="750" src="diagrams/ARCHITECTURE DIAGRAM.png" alt="Architecture Diagram">
</p>

```text
main()
  ↓
init()
  ↓
display()
  ↓
keyboard() / mouse()
  ↓
timer()
  ↓
glutMainLoop()
```

---

## Characters :

<p align="center">
  <img width="220" src="characters/The boy 1.png">
  <img width="220" src="characters/Imposter.png">
  <img width="220" src="characters/Fair.png">
</p>

| Character  | Role                                           |
| ---------- | ---------------------------------------------- |
| **Player** | Main playable character                        |
| **Enemy**  | Causes instant Game Over on collision          |
| **Torch**  | Decorative lighting element used in UI screens |

---

## Game Objects 🗝️ :

<p align="center">
  <img width="110" src="objects/Key1.png" alt="Key 1">
  <img width="110" src="objects/Key2.png" alt="Key 2">
  <img width="110" src="objects/Key3.png" alt="Key 3">
  <img width="130" src="objects/TheDoor.png" alt="Door">
  <img width="110" src="objects/Rocks3.png" alt="Trap">
  <img width="110" src="objects/Heart.png" alt="Heart">
</p>

| Object    | Function                           |
| --------- | ---------------------------------- |
| **Keys**  | The player must collect three keys |
| **Door**  | Opens after collecting all keys    |
| **Trap**  | Reduces player hearts              |
| **Heart** | Represents player health           |
| **Enemy** | Ends the game when touched         |

---

## Gameplay Features 🎮 :

* Main menu with mouse interaction
* How To Play instructions screen
* Story intro screen
* Maze gameplay scene
* Victory screen
* Game Over screen
* Player movement using keyboard
* Key collection system
* Health / hearts system
* Countdown timer
* Trap damage feedback
* Enemy collision
* Door unlock condition
* Background music
* Interactive sound effects
* Audio feedback for gameplay events

---

## Computer Graphics Concepts Applied :

### 1. 2D Object Representation

The game uses rectangles, quads, polygons, and texture-mapped surfaces to represent game objects.

### 2. Texture Mapping

Images are loaded using `stb_image.h` and mapped onto OpenGL quads using texture coordinates.

### 3. Geometric Transformations

| Transformation  | Applied To           |
| --------------- | -------------------- |
| **Translation** | Player movement      |
| **Rotation**    | Spinning keys        |
| **Scaling**     | Door pulse animation |

### 4. 2D Viewing

The project uses an orthographic projection:

```cpp
gluOrtho2D(0, 1000, 0, 700);
```

### 5. User Interaction

| Input        | Usage                         |
| ------------ | ----------------------------- |
| **Keyboard** | Player movement and shortcuts |
| **Mouse**    | Menu buttons and navigation   |

### 6. Animation

The project uses:

```cpp
glutTimerFunc()
```

to update:

* Key rotation
* Door scaling
* Timer countdown
* Damage flash effect

### 7. Collision Detection

Rectangle-based collision detection is used for:

* Walls
* Keys
* Traps
* Enemy
* Door

---

## Controls 🎮:

| Action           | Input         |
| ---------------- | ------------- |
| Move Up          | W / ↑         |
| Move Down        | S / ↓         |
| Move Left        | A / ←         |
| Move Right       | D / →         |
| Start / Continue | Enter / Space |
| Back             | B             |
| Restart          | R             |
| Menu             | M             |
| Exit             | ESC           |

---

## Repository Structure :

```text
Escape-The-Maze-The-Lost-Key/
│
├── README.md
├── main.cpp
├── stb_image.h
│
├── assets/
├── screenshots/
├── characters/
├── objects/
├── diagrams/
├── video/
└── docs/
```

---

## How to Run :

### macOS / Xcode

1. Open the project in **Xcode**
2. Make sure the `assets/` folder (including `assets/audio/`) is added to the project directory
3. Make sure `stb_image.h` is included
4. Build and run using:

```text
Command + R
```

---

## References :

* OpenGL Documentation: https://www.opengl.org/
* FreeGLUT Documentation: https://freeglut.sourceforge.net/
* `stb_image.h` by Sean Barrett: https://github.com/nothings/stb
* macOS `afplay` command-line audio player (used for sound playback)

---

## Team Members 👩‍💻:

| Name                    | Student Number |
| ----------------------- | -------------- |
| **Lina Saud Almatrafi** | 441011792      |
| **Jory Majed Alotaibi** | 44411907       |
| **Fouz Fawaz Alsharif** | 44412064       |
| **Lama Alaofy**         | 44411741       |

---

<p align="center">
  <img src="https://img.shields.io/badge/Built%20With-OpenGL%20%26%20Creativity-gold?style=for-the-badge">
</p>

<p align="center">
  <b>⭐ Escape The Maze – The Lost Key ⭐</b><br>
  Computer Graphics Project – CS2206
</p>
