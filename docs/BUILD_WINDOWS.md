# Build instructions for Windows

Prerequisites
- Visual Studio 2019/2022
- raylib installed or built; set Include and Lib directories in project settings.

Steps
1. Open Visual Studio and create or open the existing project.
2. Add `main.c` to the project.
3. In Project Properties -> C/C++ -> General -> Additional Include Directories add path to raylib includes.
4. Link with `raylib.lib` and add library directories in Linker -> General -> Additional Library Directories.
5. Copy the `assets/` folder to the output directory (where executable will be generated).
6. Build and run.
