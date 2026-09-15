# ShellForge

ShellForge is a Unix-like shell developed as part of the Operating Systems and Systems Programming (OSSP) course.

## Features (Week 1)

* Interactive REPL loop
* Makefile-based build
* Git repository
* Linux development environment

## Build

```bash
make
```

## Run

```bash
make run
```

## Week 2 Features

* Dynamic command input
* Memory allocation using `malloc()`
* Automatic buffer expansion using `realloc()`
* Proper memory cleanup using `free()`

## Week 3 Features

* Command parsing
* Tokenization of user input
* Creation of argument tokens
* Dynamic memory allocation for tokens
* Proper memory cleanup using `free_tokens()`

## Week 4 Features

* Process creation using `fork()`
* Command execution using `execvp()`
* Parent-child synchronization using `waitpid()`
* Error handling using `perror()`

## Project Structure

```text
ShellForge/
├── bin/
│   └── shellforge
├── include/
│   ├── input.h
│   ├── parser.h
│   ├── process.h
│   └── shell.h
├── src/
│   ├── input.c
│   ├── main.c
│   ├── parser.c
│   └── process.c
├── tests/
├── screenshots/
├── docs/
├── Makefile
└── README.md
```

## Week 4 Commands Supported

ShellForge can execute Linux commands such as:

```bash
ls
pwd
date
whoami
```

Invalid commands are handled using `perror()`.

## Technologies Used

* C Programming
* Linux
* GCC
* Make
* Git
* POSIX System Calls

## System Calls Used

* `fork()` - Creates a child process
* `execvp()` - Executes a Linux command
* `waitpid()` - Waits for the child process to finish
* `perror()` - Displays error messages

## Compilation

To compile the project:

```bash
make clean
make
```

## Running the Shell

```bash
./bin/shellforge
```

or:

```bash
make run
```

## Example

```text
=================================
ShellForge Version 1.0
=================================
myshell> ls
myshell> pwd
myshell> date
myshell> whoami
myshell> exit
Goodbye!
```

