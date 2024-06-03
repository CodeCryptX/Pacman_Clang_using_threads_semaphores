# 🕹️ Multi-threaded Pac-Man Game in C

<img src="https://png.pngtree.com/png-clipart/20220303/original/pngtree-pac-man-png-image_7389760.png" alt="Pac-Man Game" width="200"/>

## Project Description

This project is a multi-threaded version of the classic Pac-Man game developed in C using OPENGL. It utilizes synchronization techniques core concepts of operating systems, to manage interactions between Pac-Man and multiple computer-simulated ghosts. The game features a game engine thread, a user interface thread, and individual threads for each ghost controller. 

### Features:
- Game Engine Thread: Handles game flow, input, game state updates, and rendering.
- User Interface Thread: Manages UI components, menus, and player input events.
- Ghost Controller Threads: Individual threads for each ghost to control their behavior.

## How to Run

To compile the game, use the following command:
```
gcc -o pacman_game game.c main.c texture.c menu.c -lGL -lGLU -lglut -lm -lSOIL -lpthread -lm `sdl2-config --cflags --libs` -lSDL2_mixer
```

Make sure to download the SOIL library from [GitHub](https://github.com/soil) and install SDL2 and SDL properly before compiling.

### Installing SDL2 and SDL

On Ubuntu, you can install SDL2 and SDL using the following commands:
```
sudo apt-get update
sudo apt-get install libsdl2-dev
sudo apt-get install libsdl2-mixer-dev
```

## Note
- The game may contain bugs, and some features like tracking of ghosts are not fully implemented but have function definitions available (commented out).
- Extra files for additional features are included in the project.

---
Contributions to solve bugs and improve the game are welcome!

