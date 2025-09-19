# Level 50 Mons Modifier

A simple Java program to automate the transformation of `.species = SPECIES_XXXX,` lines in your `level_50_mons.h` file to `{count}_XXXX,`.

## Usage

1. Place your original `level_50_mons.h` file in the `input/` folder.
2. Compile and run the Java program:
    ```bash
    javac src/Level50MonsModifier.java
    java -cp src Level50MonsModifier
    ```
3. The modified file will be written to `output/level_50_mons_modified.h`.

## Requirements

- Java 8 or newer

## How it works

- Each line matching `.species = SPECIES_XXXX,` is replaced by `{count}_XXXX,`.
- All other lines are left unchanged.