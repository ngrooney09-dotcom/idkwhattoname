# Connecting Git Bash to VS Code Terminal

## Overview

In this section, you will learn how to configure and use Git Bash as the integrated terminal inside *Visual Studio Code*.

Using Git Bash in VS Code allows you to:

* Use Linux-style commands (ls, cd, etc.)
* Work consistently with Git workflows
* Follow tutorials that use Bash commands

If you are already comfortable using another terminal (e.g., PowerShell or Command Prompt), you may skip this section.

---
## Prerequisites

Before starting, ensure:

- Git is installed on your computer
👉 You can download it from: https://git-scm.com/
- Visual Studio Code is installed

---
## Steps

### 1 Open Visual Studio Code
- Double click on **Visual Studio Code** to open it.

---

### 2 Open the Menu
- Click on the **three dots** at the top left.

![Three dots](assets/images/threeDots.png){ width=50% }

---

### 3 Open Terminal Menu
- Click on the **Terminal** option from the dropdown.

![Terminal dropdown](assets/images/terminal.png){ width=50% }

---

### 4 Create New Terminal
- Select **New Terminal**.

![New Terminal](assets/images/newTerminal.png){ width=50% }

---

### 5 Locate Terminal Panel
- A terminal window should appear at the bottom of VS Code.

---

### 6 Open Terminal Options
- Click on the terminal menu.

![Terminal Window](assets/images/terminalWindow.png){ width=50% }

---

### 7 Open Dropdown Options
- Click the dropdown arrow next to the **+** icon.

![Dropdown arrow](assets/images/downArrow.png){ width=50% }

---

### 8 Select Git Bash
- Check if **Git Bash** is listed and select it.

![Terminal menu](assets/images/terminalMenu.png){ width=50% }

---

## If Git Bash is NOT Listed

### 9️ Open Command Palette
- Press `Ctrl + Shift + P`

---

### 10 Open Settings JSON
- Search:
  ```
  Preferences: Open Settings (JSON)
  ```

---

### 11 Add Configuration

```json
"terminal.integrated.profiles.windows": {
    "Git Bash": {
        "path": "C:\\Program Files\\Git\\bin\\bash.exe"
    }
}
```

---

## ⭐ Set Git Bash as Default

### 12 Select Default Profile
- Go to **Select Default Profile**
- Choose **Git Bash**

---

### 13 Open New Terminal
- Click **New Terminal (+)** again

---

### 14 Done!
- Git Bash should now run inside VS Code 🎉
