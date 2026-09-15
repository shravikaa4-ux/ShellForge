# ShellForge

ShellForge is a Unix-like shell developed as part of the Operating Systems and Systems Programming Project-Based Learning course.

## Project Overview

ShellForge is developed step by step as part of the Operating Systems and Systems Programming Project-Based Learning course.

The project demonstrates basic shell functionality, command input handling, command parsing, and preparation of commands for process execution.

## Features (Week 1)

- Interactive REPL loop
- Makefile-based build
- Git repository
- Linux development environment

## Features (Week 2)

- Dynamic command input
- Memory allocation using malloc()
- Automatic buffer expansion using realloc()
- Proper memory cleanup using free()

## Features (Week 3)

- Command parsing using strtok()
- Dynamic argv[] construction
- Modular parser implementation
- Ready for process execution with execvp()

## Project Structure

```text
ShellForge/
│
├── Makefile
├── README.md
├── .gitignore
│
├── include/
│   ├── shell.h
│   ├── input.h
│   └── parser.h
│
├── src/
│   ├── main.c
│   ├── input.c
│   └── parser.c
│
├── docs/
├── tests/
├── screenshots/
└── bin/
