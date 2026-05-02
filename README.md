# 🚪 Escape The Maze – The Lost Key

> A 2D OpenGL adventure game demonstrating core Computer Graphics concepts through interactive gameplay.

![Language](https://img.shields.io/badge/Language-C%2B%2B-blue)
![Graphics](https://img.shields.io/badge/Graphics-OpenGL-green)
![Framework](https://img.shields.io/badge/Framework-GLUT-orange)
![Course](https://img.shields.io/badge/Course-CS2206-purple)
![Status](https://img.shields.io/badge/Project-Completed-success)

---

## 📖 Project Overview

**Escape The Maze – The Lost Key** is a 2D adventure puzzle game developed using **C++ and OpenGL (GLUT)** for the **Computer Graphics (CS2206)** course project.

The player wakes up trapped inside a mysterious maze and must:

✔ Explore the maze  
✔ Collect **three hidden keys**  
✔ Avoid dangerous traps  
✔ Escape from enemies  
✔ Reach the exit door before time runs out

This project was designed to apply fundamental computer graphics concepts in a practical and interactive way.

---

## ✨ Features

### 🎬 Multiple Interactive Scenes
- Main Menu
- How To Play Screen
- Story Intro Scene
- Gameplay Scene
- Victory Screen
- Game Over Screen

---

### 🎮 Gameplay Mechanics
- Smooth player movement
- Keyboard controls (WASD + Arrow Keys)
- Mouse button interaction
- 3 collectible keys system
- Health / hearts system
- Countdown timer
- Locked / unlocked exit door
- Enemy collision detection
- Trap damage system
- Restart system

---

### 🎨 Graphics & Visual Effects
- Texture mapping
- Animated rotating keys
- Door scaling pulse animation
- Player glow effect
- Damage flash effect
- Layered scene composition
- HUD system (time / hearts / keys)

---

## 🧠 Computer Graphics Concepts Applied

This project directly applies major topics from the course:

### 1) 2D Object Representation
Objects are represented using:
- Rectangles
- Quads
- Polygons
- Texture mapped surfaces

---

### 2) Geometric Transformations

#### Translation
Used for:
- Player movement

#### Rotation
Used for:
- Key spinning animation

#### Scaling
Used for:
- Door pulse effect

---

### 3) Texture Mapping
Textures are mapped onto 2D quads for:
- Player
- Maze walls
- Floor
- Keys
- Door
- Enemy
- Traps
- UI elements

---

### 4) Animation
Animation is implemented using:

```cpp
glutTimerFunc()
```

Used for:
- Rotation updates
- Scale pulse updates
- Game timing
- Visual feedback

---

### 5) User Interaction

#### Keyboard:
- W → Up
- A → Left
- S → Down
- D → Right
- Arrow Keys → Movement

#### Mouse:
- Menu navigation
- Buttons interaction

---

### 6) Collision Detection
Rectangle collision detection is used for:
- Walls
- Keys
- Traps
- Enemy
- Door

---

## 🧱 Project Structure

```text
EscapeTheMaze/
│
├── assets/
│   ├── textures
│   ├── UI images
│   ├── player sprites
│   ├── environment assets
│
├── stb_image.h
├── main.cpp
└── README.md
```

---

## ⚙️ Program Architecture

Program flow:

```text
Menu
 ↓
How To Play
 ↓
Intro
 ↓
Gameplay
 ↓
Victory / Game Over
```

Main OpenGL callbacks:

```cpp
init()
display()
keyboard()
mouse()
timer()
reshape()
main()
```

---

## 🎮 Controls

| Action | Input |
|------|------|
| Move Up | W / ↑ |
| Move Down | S / ↓ |
| Move Left | A / ← |
| Move Right | D / → |
| Start | Enter / Space |
| Back | B |
| Restart | R |
| Main Menu | M |
| Exit | ESC |

---

## 🛠️ Technologies Used

- **C++**
- **OpenGL**
- **GLUT / FreeGLUT**
- **GLEW**
- **stb_image.h**

---

## 📚 References

### stb_image Library
Sean Barrett  
https://github.com/nothings/stb

### OpenGL Documentation
https://www.opengl.org/

### GLUT Documentation
https://freeglut.sourceforge.net/

---

## 🚀 How to Run

### macOS
Open in **Xcode** and run:

```bash
⌘ + R
```

Make sure:

```text
assets/
```

folder exists inside project directory.

---

## 🔮 Future Improvements
- Add sound effects
- Add multiple maze levels
- Add moving enemies
- Add collectibles / score system
- Add save system

---

## 👩‍💻 Team
Computer Graphics Project Team  
Faculty of Computing and Information Technology  
CS2206 – Computer Graphics

---

## 🏁 Final Note

This project was developed as an educational implementation of Computer Graphics concepts through a complete 2D interactive game experience.

---
⭐ Escape The Maze – The Lost Key
