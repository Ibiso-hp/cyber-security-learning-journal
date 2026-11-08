# Linux Fundamentals: File Management and Text Processing

**Date:** November 8, 2026  
**Environment:** Kali Linux  
**Status:** Learning in progress

## Overview

Today's session focused on Linux file and directory management, reading file contents, standard input and output, pipes, and filtering text.

## 1. Standard Input, Output and Pipes

I learned about the three standard streams:

- **stdin:** Standard input, usually receiving data from the keyboard or another command.
- **stdout:** Standard output, where normal command results are displayed.
- **stderr:** Standard error, where error messages are sent.

### Pipes (`|`)

A pipe passes the output of one command as input to another command.

Example:

`cat filename.txt | grep "Linux"`

This displays lines containing the word Linux from the file.

## 2. File and Directory Management

| Command | Purpose |
|---|---|
| `cat` | Displays and concatenates file contents. |
| `touch` | Creates an empty file or updates its timestamps. |
| `mkdir` | Creates directories. |
| `cp` | Copies files and directories. |
| `mv` | Moves or renames files and directories. |

### Examples

Create a file:

`touch notes.txt`

Create a directory:

`mkdir cybersecurity`

Copy a file:

`cp notes.txt backup.txt`

Copy a directory:

`cp -r cybersecurity cybersecurity-backup`

Rename a file:

`mv notes.txt linux-notes.txt`

## 3. Reading Files

I learned different commands for displaying file contents.

| Command | Purpose |
|---|---|
| `cat` | Displays file contents. |
| `head` | Displays the beginning of a file. |
| `tail` | Displays the end of a file. |
| `nl` | Displays file contents with line numbers. |

### Examples

Display a file:

`cat filename.txt`

Display the first 20 lines:

`head -n 20 filename.txt`

Display the last 20 lines:

`tail -n 20 filename.txt`

Display numbered lines:

`nl filename.txt`

I also learned that `nl` numbers non-empty lines by default, unlike ordinary output from `cat`, `head`, and `tail`.

## 4. Filtering Text with grep

`grep` is a command-line utility that searches text for lines matching a specified word or pattern.

Example:

`cat filename.txt | grep "Linux"`

This filters the file contents and displays only lines containing Linux.

An alternative is:

`grep "Linux" filename.txt`

## Key Takeaways

- Linux provides commands for creating, copying, moving, and managing files and directories.
- `cat`, `head`, and `tail` provide different ways to read file contents.
- `nl` displays file contents with line numbers.
- Standard input, standard output, and standard error are important parts of command-line operations.
- Pipes allow commands to work together.
- `grep` makes it easier to search through files and command output.

## Cybersecurity Applications

These concepts are useful for:
- Managing configuration and log files.
- Searching system logs for specific events.
- Filtering command output during investigations.
- Organizing files used in security exercises.
- Combining Linux commands to perform tasks efficiently.

## Next Learning Goals

- Practise creating and managing files and directories.
- Understand input/output redirection.
- Practise combining commands using pipes.
- Explore more `grep` options and text-processing techniques.
