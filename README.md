# Simple Shell Project

# Overview
This project involves creating a simple Unix shell program. A shell is a command-line interpreter that provides a user interface for accessing an operating system's services. In this project, we will build a simple version of a shell (hsh) using various system calls and functions allowed in Unix/Linux environments.

# Project Objectives
* To understand the workings of a Unix shell.
* To learn how to interact with the kernel and gain a deeper understanding of system calls.
* To apply knowledge of C programming to create a functional shell.
* To practice using system-level functions for file and process management.

# Features
* The program will replicate functionalities of a traditional Unix shell.
* It will handle commands input from standard input (stdin).
* The program will execute commands in the PATH or specified with a full path.
* Error handling will be implemented for invalid commands or arguments.
  
# Requirements
## General
* Allowed editors: vi, vim, emacs
* All your files will be compiled on Ubuntu 20.04 LTS using gcc, using the options -Wall -Werror -Wextra -pedantic -std=gnu89
* All your files should end with a new line
* A README.md file, at the root of the folder of the project is mandatory
* Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl
* Your shell should not have any memory leaks
* No more than 5 functions per file
* All your header files should be include guarded
* Use system calls only when you need to (why?)
* Write a README with the description of your project
* You should have an AUTHORS file at the root of your repository, listing all individuals having contributed content to the repository. Format, see Docker

# List of allowed functions and system calls
* access (man 2 access)
* chdir (man 2 chdir)
* close (man 2 close)
* closedir (man 3 closedir)
* execve (man 2 execve)
* exit (man 3 exit)
* _exit (man 2 _exit)
* fflush (man 3 fflush)
* fork (man 2 fork)
* free (man 3 free)
* getcwd (man 3 getcwd)
* getline (man 3 getline)
* getpid (man 2 getpid)
* isatty (man 3 isatty)
* kill (man 2 kill)
* malloc (man 3 malloc)
* open (man 2 open)
* opendir (man 3 opendir)
* perror (man 3 perror)
* read (man 2 read)
* readdir (man 3 readdir)
* signal (man 2 signal)
* stat (__xstat) (man 2 stat)
* lstat (__lxstat) (man 2 lstat)
* fstat (__fxstat) (man 2 fstat)
* strtok (man 3 strtok)
* wait (man 2 wait)
* waitpid (man 2 waitpid)
* wait3 (man 2 wait3)
* wait4 (man 2 wait4)
* write (man 2 write)

# Compilation

Your shell will be compiled this way:

gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh

# Testing

Your shell should work like this in interactive mode:


## Explain
$ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
$

But also in non-interactive mode:


## Explain
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


# Tasks
0. Betty would be proud
1. Simple shell 0.1
2. Simple shell 0.2
3. Simple shell 0.3
4. Simple shell 0.4
5. Simple shell 1.0
6. Simple shell 1.1
7. Simple shell 0.2.1
8. Simple shell 0.4.1
9. setenv, unsetenv
10. cd
11.  ;
12.  && and ||
13.  alias
14.  Variables
15.  Comments
16.  File as input

# Authors
👤Daniel Izevbije  👤 Benedict Igbukolu