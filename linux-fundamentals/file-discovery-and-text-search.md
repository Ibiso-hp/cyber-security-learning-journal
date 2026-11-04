# Linux Fundamentals: File Discovery and Text Searching

## Overview

In this lesson, I explored Linux commands used to locate files, identify executable programs, understand command paths, and search through text output.

## 1. File Discovery Commands

### locate
- Searches for files and directories using an indexed database.
- Generally provides faster results than searching the filesystem directly.
- Its results depend on how recently the database was updated.

### whereis
- Locates binary files, source files, and manual pages associated with a command.

### which
- Identifies the executable that would run when a command is entered in the shell.
- Searches directories listed in the PATH environment variable.

### find
- Searches for files and directories within specified locations.
- Offers more control through search conditions and expressions.
- Can search using criteria such as filenames, file types, and other attributes.

## 2. Understanding Binary Files and PATH

**Binary files:** Files containing machine-readable data or instructions. Executable binaries are used to run programs.

**PATH:** An environment variable containing directories that the shell searches when looking for executable commands.

## 3. Wildcards

Wildcards are special characters used to match patterns in filenames.

| Symbol | Meaning |
|---|---|
| `*` | Matches zero or more characters. |
| `?` | Matches exactly one character. |

Examples:

- `report*` matches filenames beginning with report.
- `file?.txt` matches filenames such as file1.txt and fileA.txt.

## 4. Understanding the find Command

A common command structure is:

`find [starting-directory] [options] [expression]`

Example:

`find /home -name "*.txt"`

This searches the `/home` directory for files with names ending in `.txt`.

## 5. Understanding grep

`grep` is a command-line utility used to search text for lines matching a specified pattern.

It can also be combined with other commands using a pipe (`|`) to filter their output.

Example:

`ls /home | grep "Documents"`

This filters the output of `ls /home` and displays lines containing the word Documents.

## Key Takeaways

- `locate`, `whereis`, `which`, and `find` serve different purposes when searching for files and executables.
- PATH determines where the shell searches for executable commands.
- Wildcards make filename pattern matching possible.
- `find` provides flexible filesystem searches.
- `grep` helps filter and search text output.

## Practical Applications in Cybersecurity

These commands can be useful when:
- Locating configuration files and security-related tools.
- Finding executable programs.
- Searching system directories.
- Filtering log output for specific keywords.
- Investigating files in an authorized Linux environment.

## Next Learning Goals

- Practise the file discovery commands independently.
- Explore more `find` expressions.
- Learn additional `grep` options.
- Practise searching through Linux log files.

**Status:** Learning in progress.
