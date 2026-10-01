# ShellForge

ShellForge is a Unix-like shell and Operating Systems practical project developed as part of the **Operating Systems and Systems Programming (OSSP)** course.

The project demonstrates Linux processes, signals, inter-process communication, memory management, file I/O, and POSIX system calls using C programming.

## Practicals Completed

* Practical 6 — Signals and FIFO-based Inter-Process Communication
* Practical 7 — Linux Process Memory Analysis
* Practical 8 — Dynamic Memory Management and Copy-on-Write
* Practical 9 — File I/O and `dup2()` Redirection

## Project Structure

```text
ShellForge/
├── practical6/
│   ├── fifo_client.c
│   ├── fifo_server.c
│   └── signal_handler.c
│
├── practical7/
│   ├── memory_demo.c
│   └── prog7_linuxaddr.c
│
├── practical8/
│   ├── dynamic_memory.c
│   └── cow_demo.c
│
├── practical9/
│   ├── copy_lowlevel.c
│   ├── copy_stdio.c
│   ├── redirect_input.c
│   └── redirect_output.c
│
└── README.md
```

## Practical 6 — Signals and FIFO IPC

Topics demonstrated:

* POSIX signals
* Signal handling using `sigaction()`
* `SIGINT`
* `SIGTERM`
* `SIGUSR1`
* Named pipes (FIFO)
* Client-server communication
* Inter-Process Communication (IPC)
* `mkfifo()`
* `read()`
* `write()`

### Programs

```text
fifo_client.c
fifo_server.c
signal_handler.c
```

## Practical 7 — Linux Process Memory Analysis

Topics demonstrated:

* Linux process address space
* Code/Text segment
* Global/Data segment
* BSS segment
* Heap
* Stack
* Dynamic memory allocation using `malloc()`
* Process memory inspection using `/proc`

### Programs

```text
prog7_linuxaddr.c
memory_demo.c
```

Useful Linux commands:

```bash
cat /proc/<PID>/maps
cat /proc/<PID>/status
cat /proc/<PID>/smaps
pmap <PID>
readelf -S memory_demo
size memory_demo
```

## Practical 8 — Dynamic Memory and Copy-on-Write

Topics demonstrated:

* `malloc()`
* `calloc()`
* `realloc()`
* `free()`
* Memory leak detection
* `fork()`
* Copy-on-Write (COW)
* Process memory behavior

### Programs

```text
dynamic_memory.c
cow_demo.c
```

Memory debugging was tested using Valgrind.

## Practical 9 — File I/O and Redirection

Topics demonstrated:

* Low-level file I/O
* Standard I/O
* `open()`
* `read()`
* `write()`
* `close()`
* `fopen()`
* `fread()`
* `fwrite()`
* `dup2()`
* Standard input redirection
* Standard output redirection

### Programs

```text
copy_lowlevel.c
copy_stdio.c
redirect_input.c
redirect_output.c
```

## Technologies Used

* C Programming
* Linux / WSL
* GCC
* POSIX System Calls
* Make
* Git
* GitHub

## Important System Calls and Functions

| Function      | Purpose                      |
| ------------- | ---------------------------- |
| `fork()`      | Creates a child process      |
| `execvp()`    | Executes a program           |
| `waitpid()`   | Waits for a child process    |
| `sigaction()` | Installs signal handlers     |
| `mkfifo()`    | Creates a named pipe         |
| `open()`      | Opens a file                 |
| `read()`      | Reads data                   |
| `write()`     | Writes data                  |
| `close()`     | Closes a file descriptor     |
| `dup2()`      | Duplicates a file descriptor |
| `malloc()`    | Allocates dynamic memory     |
| `realloc()`   | Resizes allocated memory     |
| `free()`      | Releases allocated memory    |

## Compilation

Individual practical programs can be compiled using GCC.

Example:

```bash
gcc -Wall -Wextra -g program.c -o program
```

Run the compiled program:

```bash
./program
```

## Git and GitHub

The project is maintained using Git and hosted on GitHub.

Basic commands used:

```bash
git status
git add .
git commit -m "Commit message"
git push
```

## Learning Objectives

ShellForge provides practical experience with:

* Linux process management
* Inter-Process Communication
* POSIX signals
* Process memory management
* Dynamic memory allocation
* Copy-on-Write
* Linux file I/O
* File descriptor manipulation
* Input/output redirection
* Git and GitHub workflow

## Status

**ShellForge practical work through Practical 9 has been completed and pushed to GitHub.**
