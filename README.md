# 0x16. C - Simple Shell

## Description

In this project we are tasked with creating our own simple UNIX command interpreter. The program must have the exact same output as sh (/bin/sh) as well as the exact same error output. The only difference is when you print an error, the name of the program must be equivalent to your argv[0].

## Instructions

Compiling the program: 

``` 
gcc -Wall -Werror -Wextra -pedantic *.c -o hsh
```
Your shell should work like this

Interactive mode:

``` 
$ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
$
```

Non-interactie mode:

``` 
$ echo "/bin/ls" | ./hsh
hsh main.c shell.c test_ls_2
$
$ cat test_ls_2
/bin/ls
/bin/ls
$
$ cat test_ls_2 | ./hsh
hsh main.c shell.c test_ls_2
hsh main.c shell.c test_ls_2
$
```

## Requirements

## General

Allowed editors: vi, vim, emacs

All your files will be compiled on Ubuntu 20.04 LTS using gcc, using the options -Wall -Werror -Wextra -pedantic -std=gnu89

All your files should end with a new line

A README.md file, at the root of the folder of the project is mandatory

Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl

Your shell should not have any memory leaks

No more than 5 functions per file

All your header files should be include guarded

Use system calls only when you need to (why?)

Write a README with the description of your project

You should have an AUTHORS file at the root of your repository, listing all individuals having contributed content to the repository. Format, see Docker

## Tasks

### 0. README, man, AUTHORS

### 1. Write a (README)[./README.md]

Write a (man)[./man_1_simple_shell] for your shell.
You should have an (AUTHORS)[./AUTHORS] file at the root of your repository, listing all individuals having contributed content to the repository.


### 1. Betty would be proud

Write a beautiful code that passes the Betty checks

### 2. Simple shell 0.1

Write a UNIX command line interpreter.

Your Shell should:

Display a prompt and wait for the user to type a command. A command line always ends with a new line.

The prompt is displayed again each time a command has been executed.

The command lines are simple, no semicolons, no pipes, no redirections or any other advanced features.

The command lines are made only of one word. No arguments will be passed to programs.

If an executable cannot be found, print an error message and display the prompt again.

Handle errors.

You have to handle the "end of file" condition (Ctrl+D)

### 3. Simple shell 0.2

Handle command lines with arguments

### 4. Simple shell 0.3

Handle the PATH

### 5. Simple shell 0.4

Implement the exit built-in, that exits the shell

Usage: exit

You dont have to handle any argument to the built-in exit

### 6. Simple shell 1.0

Implement the env built-in, that prints the current environment

### 7. What happens when you type ls -l in the shell

## Collaborators

[Laban Rotich](https://github.com/laban254)
[Edmund Spira](https://github.com/edmundspira)
