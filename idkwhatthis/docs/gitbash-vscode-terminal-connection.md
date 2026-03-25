# Connecting Git Bash to VS Code Terminal

## Overview

In this section, you will learn how to connect Git Bash to your VS Code terminal.

This documentation uses Git Bash for demonstration. If you are already familiar with using other terminals in VS Code, you may skip this section.

---

## Steps

### 1 Open Visual Studio Code
- Double click on **Visual Studio Code** to open it.

---

### 2 Open the Menu

<p align="center">
  <img src="assets/images/threeDots.png" width="50%">
</p>

- Click on the **three dots** at the top left.

---

### 3 Open Terminal Menu

<p align="center">
  <img src="assets/images/terminal.png" width="50%">
</p>

- Click on the **Terminal** option from the dropdown.

---

### 4 Create New Terminal

<p align="center">
  <img src="assets/images/newTerminal.png" width="50%">
</p>

- Select **New Terminal**.

---

### 5 Locate Terminal Panel
- A terminal window should appear at the bottom of VS Code.

---

### 6 Open Terminal Options

<p align="center">
  <img src="assets/images/terminalWindow.png" width="50%">
</p>

- Click on the terminal menu.

---

### 7 Open Dropdown Options

<p align="center">
  <img src="assets/images/downArrow.png" width="50%">
</p>

- Click the dropdown arrow next to the **+** icon.

---

### 8️ Select Git Bash

<p align="center">
  <img src="assets/images/terminalMenu.png" width="50%">
</p>

- Check if **Git Bash** is listed and select it.

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
