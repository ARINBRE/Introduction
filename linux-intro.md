### Introduction to Linux

A command in the terminal generally follows a simple structure:

| Component | Description | Example |
| :--- | :--- | :--- |
| **Command** | The name of the program or utility to be executed. | `ls` |
| **Options (Flags)** | Modifiers that change the command's behavior, preceded by one or two hyphens. | `-l` (for long listing) |
| **Arguments** | The input or targets on which the command operates (e.g., a file name, a directory path). | `/home/user/data` |

**Example:**

```bash
ls -l usr/project_data
```

# Linux Essentials – Command Reference

This table summarizes commonly used Linux commands for navigation, file manipulation, system information, and text editing (Vim).

---

## File System Navigation

| Command | Description |
|--------|-------------|
| `pwd` | Print current working directory |
| `ls` | List directory contents |
| `cd <dir>` | Change directory |
| `mkdir <dir>` | Create a new directory |
| `rm -r <dir>` | Remove a directory recursively |

---

## Vim Text Editor Basics

| Command | Description |
|--------|-------------|
| `vi filename.txt` | Open or create file using Vim |
| `i` | Insert mode (edit text) |
| `Esc` | Return to command mode |
| `:w` | Save file |
| `:wq` | Save and quit |
| `:q!` | Quit without saving |
| `A` | Append at end of line |
| `I` | Insert at beginning of line |
| `gg` / `G` | Jump to first / last line |
| `/pattern` | Search forward |
| `?pattern` | Search backward |
| `n` / `N` | Next / previous search match |
| `:%s/old/new/g` | Replace all occurrences |
| `:%s/old/new/gc` | Replace with confirmation |

---

## File & Directory Manipulation

| Command | Description |
|--------|-------------|
| `touch <file>` | Create an empty file or update timestamp |
| `cp <src> <dest>` | Copy file or directory |
| `mv <src> <dest>` | Move or rename a file or directory |
| `rm <file>` | Remove a file |

---

## Viewing File Contents

| Command | Description |
|--------|-------------|
| `cat <file>` | Show entire file |
| `less <file>` | View file with scroll support |
| `more <file>` | View file page-by-page |
| `head <file>` | First 10 lines of file |
| `tail <file>` | Last 10 lines of file |

---

## System Information

| Command | Description |
|--------|-------------|
| `uname -a` | Display system details |
| `whoami` | Show current user |
| `top` | Display running processes and resource usage |

---

## ⍰ Getting Help

| Command | Description |
|--------|-------------|
| `man <command>` | Open manual page for a command |



---
Dive into the world of conda with us at [Next Page &rarr;](conda-intro.md)
