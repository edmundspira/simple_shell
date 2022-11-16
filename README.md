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


## Steps in order to use our shell

To try out our shell use the following steps

Step 1: Clone our repository using this command, (you need to have git installed on your machine first)

``` git clone https://github.com/edmundspira/simple_shell  ``` 

Step 2: Change directory to simple_shell:

``` cd simple_shell ```

Step 3: Compile the C files in this way:

``` gcc -Wall -Werror -Wextra -pedantic *.c -o hsh ```

Step 4: Run the shell

``` ./hsh ```

Exiting the shell When you want to exit the shell, you can use one of the following methods: 

1: Type the command "exit"

``` exit ```

2: Press on  Ctrl + D 


## Collaborators

[Laban Rotich](https://github.com/laban254)

[Edmund Spira](https://github.com/edmundspira)

## References

[Let's Build a Command Line Shell in C](http://www.dmulholl.com/lets-build/a-command-line-shell.html#:~:text=Let%27s%20Build%20a%20Command%20Line%20Shell%20in%20C,...%204%20Step%204%20%E2%80%94%20Supporting%20Builtins%20)

[Tutorial to code a simple shell in C](https://www.linkedin.com/pulse/tutorial-code-simple-shell-c-ricardo-hincapi%C3%A9-trujillo/)

[Make your own simple shell in C](https://www.linkedin.com/pulse/make-your-own-simple-shell-c-norman-isaza/)

Make sure you Have a valid and updated compiler. Use Clang if you have to :)
            Download Clang here:<< https://releases.llvm.org/download.html >>
