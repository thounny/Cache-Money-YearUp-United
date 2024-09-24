# Bash Command Line Basics

This guide is designed to help you understand some fundamental Bash commands and concepts, focusing on directory navigation, file manipulation, and understanding terminal commands.

---

## Terminal vs Shell: What's the Difference?

- **Terminal**: The terminal is the interface you interact with to type commands. It's a text interface that allows you to control your computer without a graphical user interface (GUI).
  
- **Shell**: The shell is the program that interprets the commands you type into the terminal. Bash (Bourne Again Shell) is one of the most commonly used shells.

Think of the **terminal** as the keyboard you type into and the **shell** as the brain that understands and executes the commands.

---

## Directories (Folders)

A **directory** is the same thing as a folder. It's a place where files and other directories are stored.

- **Current Directory (`.`)**: The current working directory you are in.
- **Parent Directory (`..`)**: The directory that is one level up from your current location.

---

## Listing Files and Directories: `ls`

The `ls` command is used to list the contents of a directory.

- **Command**:
  ```bash
  ls
  ```

  This command will list all files and directories in the current folder.

- **Example**:
  ```bash
  ls
  ```

- **Long Format with Hidden Files**: `ls -la`
  - `-l` shows more details (permissions, file size, and modification time).
  - `-a` includes hidden files (files that start with a dot `.`).

  **Command**:
  ```bash
  ls -la
  ```

  **Example**:
  ```bash
  ls -la
  ```

---

## Navigating Directories: `cd`

The `cd` command is used to **change directories**.

- **Command**:
  ```bash
  cd directory_name
  ```

  This will move you into the specified directory.

- **Go to Parent Directory**:
  ```bash
  cd ..
  ```

  This moves you one level up to the parent directory.

- **Example**:
  ```bash
  cd my_folder
  ```

  This will take you into the `my_folder` directory.

---

## Creating or Updating Files: `touch`

The `touch` command is used to **create a new file** or **update the timestamp** of an existing file.

- **Command**:
  ```bash
  touch file_name
  ```

- **Example**:
  ```bash
  touch newfile.txt
  ```

  This creates a new file called `newfile.txt` in the current directory.

---

## Making a Directory: `mkdir`

The `mkdir` command is used to create a new directory (folder).

- **Command**:
  ```bash
  mkdir directory_name
  ```

- **Example**:
  ```bash
  mkdir my_folder
  ```

  This will create a new directory called `my_folder`.

---

## Displaying Text: `echo`

The `echo` command **prints** text to the terminal or a file.

- **Command**:
  ```bash
  echo "Your text here"
  ```

  This will print the text "Your text here" to the terminal.

- **Example**:
  ```bash
  echo "Hello, Year Up!"
  ```

  Output:
  ```
  Hello, Year Up!
  ```

---

## Concatenating Files: `cat`

The `cat` command is used to **concatenate** and display the content of files.

- **Command**:
  ```bash
  cat file_name
  ```

- **Example**:
  ```bash
  cat newfile.txt
  ```

  This displays the contents of `newfile.txt` to the terminal one letter at a time.

---

## Moving or Renaming Files: `mv`

The `mv` command is used to **move** or **rename** files and directories.

- **Command**:
  ```bash
  mv source_file target_file
  ```

- **Example**:
  ```bash
  mv oldfile.txt newfile.txt
  ```

  This renames `oldfile.txt` to `newfile.txt`.

---

## Removing Files: `rm`

The `rm` command is used to **remove** files.

- **Command**:
  ```bash
  rm file_name
  ```

- **Example**:
  ```bash
  rm oldfile.txt
  ```

  This removes `oldfile.txt` from the current directory.

---

## Deleting Directories: `rmdir`

The `rmdir` command is used to **delete an empty directory**.

- **Command**:
  ```bash
  rmdir directory_name
  ```

- **Example**:
  ```bash
  rmdir my_folder
  ```

  This removes the `my_folder` directory if it is empty.

---

## Removing Files and Directories Recursively: `rm -rf`

The `rm -rf` command is used to **remove files and directories recursively and forcefully**.

- **Command**:
  ```bash
  rm -rf directory_name
  ```

- **Example**:
  ```bash
  rm -rf my_folder
  ```

  This removes `my_folder` and all of its contents without prompting for confirmation.

---

## Wildcard Matching: `*`

The asterisk `*` is used as a **wildcard** that matches any pattern in filenames.

- **Command**:
  ```bash
  ls *.txt
  ```

- **Example**:
  ```bash
  ls *
  ```

  This lists all files and directories in the current folder, matching any name.

---

## Redirecting Output: `>` and `>>`

- **`>` (Single Redirect)**:
  Redirects the output of a command to a file, **overwriting** the file if it exists or creating it if it doesn’t.

  - **Command**:
    ```bash
    echo "Some text" > file_name
    ```

    This creates or overwrites `file_name` with the text `Some text`.

  - **Example**:
    ```bash
    echo "Hello, Year Up!" > greetings.txt
    ```

    This creates (or overwrites) `greetings.txt` with "Hello, Year Up!".

- **`>>` (Double Redirect)**:
  Redirects the output of a command to a file, **appending** to the file without overwriting it.

  - **Command**:
    ```bash
    echo "More text" >> file_name
    ```

    This adds the text `More text` to the end of `file_name`.

  - **Example**:
    ```bash
    echo "How are you?" >> greetings.txt
    ```

    This appends "How are you?" to `greetings.txt`.

---

## Summary of Commands

| Command                        | Description                                           |
|--------------------------------|-------------------------------------------------------|
| `ls`                           | Lists files and directories in the current directory  |
| `ls -la`                       | Lists all files (including hidden) in long format     |
| `cd directory_name`            | Changes directory to `directory_name`                 |
| `cd ..`                        | Moves up one directory level (to the parent directory)|
| `touch file_name`              | Creates a new file or updates an existing one         |
| `mkdir directory_name`         | Creates a new directory (folder)                      |
| `echo "text"`                  | Prints `text` to the terminal                        |
| `echo "text" > file`           | Writes `text` to a file, overwriting it if it exists |
| `echo "text" >> file`          | Appends `text` to a file                              |
| `cat file_name`                | Displays the content of `file_name`                   |
| `mv source_file target_file`    | Moves or renames `source_file` to `target_file`      |
| `rm file_name`                 | Removes the specified `file_name`                     |
| `rmdir directory_name`          | Deletes an empty directory                            |
| `rm -rf directory_name`        | Removes `directory_name` and all its contents forcefully |
| `*`                             | Wildcard that matches any pattern in filenames        |

---
