#  Escape The Maze – The Lost Key 🚪 :

> A 2D OpenGL adventure game demonstrating core Computer Graphics concepts through interactive gameplay.

<p align="center">
  <img width="900" src="screenshots/gameplay.png" alt="Escape The Maze Gameplay Preview">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Language-C%2B%2B-blue">
  <img src="https://img.shields.io/badge/Graphics-OpenGL-green">
  <img src="https://img.shields.io/badge/Framework-GLUT-orange">
  <img src="https://img.shields.io/badge/Course-CS2206-purple">
  <img src="https://img.shields.io/badge/Status-Completed-success">
</p>

---

##  Project Description :

**Escape The Maze – The Lost Key** is a 2D adventure maze game developed using **C++ and OpenGL/GLUT**.

The player wakes up inside a mysterious maze and must collect **three hidden keys**, avoid traps and enemies, and escape through the exit door before the timer reaches zero.

---

##  Gameplay Demo 🎥 :

Replace the link below with your YouTube / Google Drive demo video link.

[![Watch Gameplay Demo](screenshots/menu.png)](PUT_YOUR_VIDEO_LINK_HERE)

**Direct Video Link:** PUT_YOUR_VIDEO_LINK_HERE

---

##  Screenshots :

Put your screenshots inside the `screenshots/` folder using these exact names.

| Main Menu | How To Play |
|---|---|
| <img src="screenshots/menu.png" width="420"> | <img src="screenshots/how-to-play.png" width="420"> |

| Gameplay | Victory |
|---|---|
| <img src="screenshots/gameplay.png" width="420"> | <img src="screenshots/victory.png" width="420"> |

| Game Over | Intro |
|---|---|
| <img src="screenshots/game-over.png" width="420"> | <img src="screenshots/intro.png" width="420"> |

---

##  Game Flow 🧩 :

Put your flowchart image here: `diagrams/game-flow.png`

<p align="center">
  <img width="750" src="diagrams/game-flow.png" alt="Game Flow Diagram">
</p>

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

---

##  Code Architecture :

Put your architecture diagram here: `diagrams/architecture.png`

<p align="center">
  <img width="750" src="diagrams/architecture.png" alt="Code Architecture Diagram">
</p>

```text
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

##  Characters :

Put character images inside the `characters/` folder.

<p align="center">
  <img width="220" src="characters/The boy 1.png" alt="The boy 1">
  <img width="220" src="characters/Imposter.png" alt="Imposter">
  <img width="220" src="characters/Fair.png" alt="Fair">
</p>

| Character | Role |
|---|---|
| Player | Main playable character |
| Enemy | Causes instant Game Over on collision |
| Torch | Decorative maze lighting element |

---

##  Game Objects 🗝️ 👻 :

Put object images inside the `objects/` folder.

<p align="center">
  <img width="110" src="objects/key1.png" alt="Key 1">
  <img width="110" src="objects/key2.png" alt="Key 2">
  <img width="110" src="objects/key3.png" alt="Key 3">
  <img width="130" src="objects/door.png" alt="Door">
  <img width="110" src="objects/trap.png" alt="Trap">
  <img width="110" src="objects/heart.png" alt="Heart">
</p>

---

##  Gameplay Features :

- Main menu with mouse interaction
- How To Play instructions screen
- Story intro screen
- Maze gameplay scene
- Victory screen
- Game Over screen
- Player movement using keyboard
- Key collection system
- Health system
- Timer system
- Trap damage feedback
- Enemy collision
- Door unlock condition

---

## Computer Graphics Concepts Applied 🧠 :

### 1. 2D Object Representation
The game uses rectangles, quads, polygons, and texture-mapped surfaces.

### 2. Texture Mapping
Images are loaded using `stb_image.h` and mapped onto OpenGL quads using texture coordinates.

### 3. Geometric Transformations

| Transformation | Applied To |
|---|---|
| Translation | Player movement |
| Rotation | Spinning keys |
| Scaling | Door pulse animation |

### 4. 2D Viewing
The project uses an orthographic projection:

```cpp
gluOrtho2D(0, 1000, 0, 700);
```

### 5. User Interaction

| Input | Usage |
|---|---|
| Keyboard | Player movement and shortcuts |
| Mouse | Menu buttons and navigation |

### 6. Animation
The project uses `glutTimerFunc()` to update:
- Key rotation
- Door scaling
- Timer countdown
- Damage flash effect

### 7. Collision Detection
Rectangle-based collision is used for walls, keys, traps, enemy, and door.

---

##  Controls 🎮 :

| Action | Input |
|---|---|
| Move Up | W / ↑ |
| Move Down | S / ↓ |
| Move Left | A / ← |
| Move Right | D / → |
| Start / Continue | Enter / Space |
| Back | B |
| Restart | R |
| Menu | M |
| Exit | ESC |

---

## Repository Structure :

```text
EscapeTheMaze/
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

##  How to Run :

### macOS / Xcode

1. Open the project in **Xcode**
2. Make sure the `assets/` folder is added to the project directory
3. Make sure `stb_image.h` is included
4. Build and run using **Command + R**

---

##  References :

- OpenGL Documentation: https://www.opengl.org/
- FreeGLUT Documentation: https://freeglut.sourceforge.net/
- `stb_image.h` by Sean Barrett: https://github.com/nothings/stb

---

##  Team Members 👩‍💻 :

| Member | Role |
|---|---|
| Member 1 | Project leader / Lina Saud Almatrafi |
| Member 2 | Jory Majed Alotaibi|
| Member 3 | Fouz Fawaz Alsharif |
| Member 4 | Lama Alaofy|

---

## 🔮 Future Work

- Add sound effects
- Add more maze levels
- Add moving enemies
- Add scoring system
- Add difficulty modes

---

<p align="center">
  <b>⭐ Escape The Maze – The Lost Key ⭐</b>
</p>
