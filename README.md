# freepo
this is a practice repo for people to mess around with github

# Intro to Git & GitHub Using VS Code

Welcome! This guide will show you how to use Git with GitHub inside [Visual Studio Code (VS Code)](https://code.visualstudio.com/). You don’t need to be a terminal expert—VS Code makes Git much easier! We'll also include basic terminal commands when needed.

---

## 1. Open the Terminal in VS Code

- Open your project folder in VS Code.
- **Open the terminal:**  
  Press <kbd>Ctrl</kbd> + <kbd>`</kbd> (the key above Tab),  
  or from the menu: **View** → **Terminal**.
  There is also a dropdown bar at the top of the program called terminal you can use to open a terminal.

---

## 2. Basic Terminal Commands

You'll use the terminal for navigating your folders:

| Command      | What it does                    | Example                  |
|--------------|---------------------------------|--------------------------|
| `ls`         | Lists files in the current folder| `ls`                     |
| `cd`         | Changes directory               | `cd my-project`          |
| `cd ..`      | Navigate upstream               | `cd ..`                  |
| `pwd`        | Prints your current directory   | `pwd`                    |

---

## 3. Git Basics in VS Code

VS Code has Git built-in! You can use both buttons and the terminal:

### a. Cloning a Repository

**Option 1:** Use the Command Palette (<kbd>F1</kbd> or <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd>), then type "**Git: Clone**". Paste the repository URL.

**Option 2:** Or in the terminal:

```bash
git clone https://github.com/username/repository.git
cd repository
```

Open the folder in VS Code afterward.

### b. Creating a New Branch

**Option 1:**  
In the bottom left (blue bar), click on the branch name and choose "Create new branch".

**Option 2:**  
In the terminal:

```bash
git checkout -b my-feature-branch
```

---

## 4. Tracking and Saving Changes

VS Code’s Source Control tab (left sidebar, the branch icon) shows your changes.

**Or, use the terminal:**

- See changes:  
  ```bash
  git status
  ```

- Stage files for commit:  
  Select files in the Source Control tab, or:  
  ```bash
  git add filename
  # or add all changes:
  git add .
  ```

- Commit staged files:  
  Type a message in the Source Control tab and click the check mark, or:  
  ```bash
  git commit -m "Describe what you changed"
  ```

---

## 5. Push Your Changes to GitHub

When you’re ready to upload:

- In VS Code, click "Sync Changes" (arrow icons) in the Source Control tab,  
  **or** use the terminal:
  ```bash
  git push origin my-feature-branch
  ```

---

## 6. Summary: A Common Workflow

1. **Make a new branch:**  
   - Use VS Code menu or  
   ```bash
   git checkout -b branch-name
   ```
2. **Edit files** (save often!)
3. **See what changed:**  
   - Source Control tab or  
   ```bash
   git status
   ```
4. **Stage files:**  
   - Click "+" or  
   ```bash
   git add .
   ```
5. **Commit:**  
   - Write a message & click ✔, or  
   ```bash
   git commit -m "Message"
   ```
6. **Push:**  
   - Use VS Code "Sync" button, or  
   ```bash
   git push origin branch-name
   ```

---

**Tips:**
- Use the Source Control tab for most operations.
- The terminal is always available if you want more control.
- You can always check `git status` if you’re unsure!

---

### After Pushing

Visit your repository on GitHub.com to open a Pull Request and ask for your changes to be reviewed.

---

Happy learning! 🎉
