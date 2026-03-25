# Pushing an Existing Project to GitHub

## Overview
This guide walks you through pushing an existing local project to a GitHub repository for version control and collaboration.

---

## Steps

### 1️ Open Your Project Folder
- Navigate to your existing project directory on your computer.

---

### 2️ Open a Terminal
Choose one of the following:
- Right-click inside the folder → **Git Bash**
- Open **VS Code** → Press `Ctrl + \`` to open the terminal

---

### 3️ Initialize Git
Start tracking your project:

```bash
git init
```

---

### 4️ Check Status *(Optional)*
See which files are untracked:

```bash
git status
```

---

### 5️ Stage Files
Add all files to staging:

```bash
git add .
```

---

### 6️ Commit Changes
Save your files with a message:

```bash
git commit -m "Initial commit"
```

---

### 7️ Create a GitHub Repository
- Go to GitHub
- Click **New Repository**
- ⚠️ Do **NOT** initialize with a README if your project already has files

!!! warning
    Do not initialize the repository with a README, .gitignore, or license if you already have a local project.

---

### 8️ Copy Repository URL
Example:

```
https://github.com/username/repo.git
```

---

### 9️ Add Remote Origin
Link your local project to GitHub:

```bash
git remote add origin https://github.com/username/repo.git
```

---

###  10 Verify Remote *(Optional)*

```bash
git remote -v
```

---

###  11 Push to GitHub

```bash
git push -u origin main
```

> 💡 Use `master` instead of `main` if your branch uses that name.

!!! tip
    You can check your branch name using:
    ```bash
    git branch
    ```

---

###  12 Confirm Upload
- Refresh your GitHub repository page
- Ensure all files have been uploaded successfully

---

##  Done!
Your project is now successfully pushed to GitHub and ready for collaboration 🚀
