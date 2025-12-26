# Build instructions for Linux

Install raylib (example for Ubuntu):

sudo apt install libraylib-dev

Build with gcc:

gcc -o pacman main.c -lraylib -lm -lGL -pthread -ldl -lrt -lX11

Place `assets/` next to the compiled executable.
