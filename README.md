# CHIP-8 Emulator in C++ (SDL2)

A complete CHIP-8 emulator written in **C++** using **SDL2** for graphics and keyboard input.

This project emulates the classic CHIP-8 virtual machine and can run games like **PONG**, **TETRIS**, **INVADERS**, and the famous **IBM Logo ROM**.

---

## Features

- 4KB memory implementation  
- 16 general purpose registers (V0–VF)  
- Stack & program counter emulation  
- Opcode fetch–decode–execute cycle  
- Sprite rendering (64×32 resolution)  
- Keyboard input using SDL2  
- ROM loading from external files  

---

## Controls (CHIP-8 Keypad)

| CHIP-8 | Keyboard |
|--------|----------|
| 1 2 3 C | 1 2 3 4 |
| 4 5 6 D | Q W E R |
| 7 8 9 E | A S D F |
| A 0 B F | Z X C V |


---

## Build Instructions (Windows – MSYS2 MinGW64)

```bash
g++ main.cpp chip8.cpp -IC:/msys64/mingw64/include/SDL2 -LC:/msys64/mingw64/lib -lmingw32 -lSDL2main -lSDL2 -mwindows -o chip8.exe

RUN
./chip8.exe roms/ibm_logo.ch8
