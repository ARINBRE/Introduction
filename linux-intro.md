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

###  (Print Working Directory): Shows the absolute path of the directory you are currently in.

```
pwd
# Output: /home/jdoe/ARINBRE_project
```

### (List): Lists the contents (files and directories) of the current directory.

```
ls -lF 
# -l (long format) and -F (adds indicators like '/' for directories)
```

### (Change Directory): Changes the current directory to a specified path.

```
cd results/
# Go into the 'results' directory

cd ..
# Go up one level (parent directory)
```



---
Dive into the world of conda with us at [Next Page &rarr;](conda-intro.md)
