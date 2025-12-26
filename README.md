# PAC-MAN Raylib Clone

Authentic Pac-Man clone implemented in C using raylib.

Features
- Playable Pac-Man with ghosts AI, power pellets, fruit, levels, and scoring
- Simple, portable code designed to work with raylib

Prerequisites
- raylib (tested with v5.x)
- C compiler (MSVC / MinGW) or Visual Studio

Repository layout
- `main.c` — game source
- `assets/` — spritesheet and audio files (not included in this repository by default)

Quick start
1. Install raylib:
   - Windows (Visual Studio): build or install raylib and make its `include` path and `raylib.lib` available to your project.
   - Linux: install the `libraylib-dev` package or build from source.
   - macOS: install via Homebrew: `brew install raylib`.

2. Open the project in Visual Studio (if present) or compile from command line:
   - Visual Studio: open the solution or create a Visual C project, add `main.c`, set Additional Include Directories to point to raylib headers and link against `raylib.lib`. Copy the `assets/` folder next to the compiled executable.
   - MinGW / GCC (pkg-config available):
     `gcc main.c -o pacman -lraylib -lGL -lm -lpthread -ldl -lrt -lX11` (Linux example — use `pkg-config --cflags --libs raylib` on supported distros).

3. Prepare assets
   - Create an `assets/` folder in the executable directory containing:
     - `spritesheet.png`
     - `Intro.wav`, `chomp.wav`, `death.wav`, `eat_ghost.wav`, `ghost_running_away.wav`, `eat_fruit.wav`, etc.
   - See `ASSETS.md` for details.

Running
- Run the compiled executable. Use arrow keys to move Pac-Man and SPACE to start.

License
- This repository is licensed under the MIT License (see `LICENSE`).

Contributing
- See `CONTRIBUTING.md` for contribution guidelines.

Notes
- Assets (graphics and audio) are not included in this repository. Make sure you have the legal right to distribute any assets you add.
- If `raylib.h` cannot be found by your compiler, add the raylib include directory to your project's include path or change the include in the source to the correct relative path (for example `#include "path/to/raylib.h"`).
