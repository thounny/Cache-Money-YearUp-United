# **Command Line Basics**

- **What is the Command Line?**  
  The Command Line is a text-based interface where you type commands to interact with your computer’s files and programs. It's especially useful for tasks like navigating through folders or running programs, which are faster than using graphical interfaces.

  **Example:**

  ```bash
  $ date   # Outputs the current date and time
  ```

- **Basic Commands**:

  - **pwd (print working directory)**: Shows where you are in the file system.

    ```bash
    $ pwd
    /Users/yourname/Documents
    ```

  - **ls (list)**: Lists the files and folders in your current directory.

    ```bash
    $ ls
    Documents  Downloads  Pictures
    ```

  - **cd (change directory)**: Move between directories.

    ```bash
    $ cd Documents
    ```

  - **mkdir (make directory)**: Create a new folder.

    ```bash
    $ mkdir new_folder
    ```

  - **touch**: Create a new, empty file.

    ```bash
    $ touch file.txt
    ```

  - **rm (remove)**: Delete files, and use `rmdir` to delete folders.
    ```bash
    $ rm file.txt
    $ rmdir empty_folder
    ```

---

### **File Paths**

- **Absolute Path**: Starts from the root directory (e.g., `/Users/yourname/Documents/file.txt`).
- **Relative Path**: Starts from your current location (e.g., `./file.txt`).

---

### **Git Basics**

Git is a version control system that helps track changes in your project over time. You can save "snapshots" of your code called **commits**, which lets you revert back to previous versions if needed.

#### **Key Git Concepts**:

1. **Working Directory**: Where your code resides.
2. **Staging Area**: Where files are prepared for a commit.
3. **Local Repository**: Where the actual commits are stored.

---

### **Basic Git Commands**

- **git init**: Initializes a new Git repository in your project folder. This command is run inside the folder you want Git to track.

  ```bash
  $ git init
  ```

- **git status**: Shows the current state of your project, including which files are modified, added, or removed, but not yet committed.

  ```bash
  $ git status
  ```

- **git add**: Prepares files for the next commit by adding them to the staging area.

  **Examples**:

  - Add a specific file:
    ```bash
    $ git add file.txt
    ```
  - Add all modified, deleted, or newly created files:

    ```bash
    $ git add .
    ```

    **Note:**  
    The `git add .` command stages **all files** (new, modified, and deleted) in the current directory and its subdirectories, preparing them for the next commit. This is useful when you've made multiple changes and want to add everything at once.

---

### **Committing Files**

Once your files are in the staging area, you commit them to the local repository, effectively saving the current state of your project.

- **git commit**: This command commits the staged files with a message describing the changes.
  ```bash
  $ git commit -m "Initial commit with basic project structure"
  ```

---

### **Branching in Git**

- **Branches** in Git allow you to work on different versions of your project at the same time. For example, you might have a `main` branch with stable code and a `feature` branch where you develop a new feature.

- **git branch**: Creates a new branch.

  ```bash
  $ git branch new-feature
  ```

- **git checkout**: Switches between branches.

  ```bash
  $ git checkout new-feature
  ```

- **git merge**: Merges a branch into your current branch (e.g., merging your `new-feature` branch into `main` once the feature is complete).
  ```bash
  $ git merge new-feature
  ```

---

### **Working with Remote Repositories (GitHub)**

Git also allows you to work with **remote repositories** like GitHub, where you can collaborate with others.

- **git clone**: Downloads a remote repository (e.g., from GitHub) to your local machine.

  ```bash
  $ git clone https://github.com/your-repo.git
  ```

- **git push**: Sends your committed changes from your local repository to a remote one.

  ```bash
  $ git push origin main
  ```

- **git pull**: Updates your local project with any changes that have been pushed to the remote repository.
  ```bash
  $ git pull origin main
  ```

---

### **Putting it All Together**

1. **Initialize a Git repository**:

   ```bash
   $ git init
   ```

2. **Check the status of your project**:

   ```bash
   $ git status
   ```

3. **Stage your files** (e.g., add all files using `git add .`):

   ```bash
   $ git add .
   ```

4. **Commit the staged files**:

   ```bash
   $ git commit -m "Added all project files"
   ```

5. **Create and switch to a new branch**:

   ```bash
   $ git branch new-feature
   $ git checkout new-feature
   ```

6. **Push your changes to GitHub**:
   ```bash
   $ git push origin new-feature
   ```

---
