# Project-3-CMSC313

## Compile EXE
1. gcc -O0 -o hexfile hexfile.c
2. gcc -O1 -o hexfile hexfile.c
3. gcc -O3 -o hexfile hexfile.c

## Compile Assembly Files
1. gcc -O0 -S -o hexfile_O0.s hexfile.c
2. gcc -O1 -S -o hexfile_O1.s hexfile.c
3. gcc -O3 -S -o hexfile_O3.s hexfile.c

## Run
./hexfile binary.out

## Compile Analysis
- O0 - The compiler does not improve the code at all. Every local variable lives on the stack and is stored on every access.
- O1 - Improvements are made to memory optimization so inner loops do not read/write on every iteration.
- O3 - Builds on O1 and heavily optimizes the code, but makes debgging more difficult, increases compile time, but decreases execution time.
