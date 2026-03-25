# Working with Existing Code on Github

## Overview

This section demonstrates how to work with existing code from a GitHub repository. There are two common methods:

1. Cloning – the easiest and most efficient method
2. Downloading a ZIP file – a simpler method without version control

## Method 1: Cloning a Repository (Recommended)

## Steps

1. **Navigate** to the desired repository on GitHub using your web browser.
2. Copy the Repository URL
    - **Click** the green “Code” button
    - **Copy** the HTTPS URL

3. Open a Terminal
    - Open Git Bash, or
    - Open Visual Studio Code and launch the terminal

4. Choose a Local Directory
    - Navigate to the folder where you want to store the project:

    ```cd path/to/your/folder
    ```

5. Clone the Repository
    - Run the following command:

    ```git clone https://github.com/username/repo.git
    ```

6. Navigate into the Project Folder

    ```cd repo-name
    ```

7. Verify Files Were Downloaded
    - Check that all project files are present in the directory.

8. Check Repository Status (Optional)

    ```git status
    ```

9. Open the Project in an Editor
    - Open the folder in Visual Studio Code or your preferred IDE.
10. Start Working on the Code
    - Make changes, add features, or fix bugs as needed.
11. Pull Latest Changes (Recommended)
    - Before starting work, ensure your code is up to date:

    ```git pull
    ```

## Method 2: Downloading as a ZIP File

## Steps

1. **Navigate** to the Repository
    - **Open** the repository on GitHub.
2. **Click** the “Code” Button
    - This will open a dropdown menu.
3. **Select** “Download ZIP”
    - The repository will be downloaded as a compressed file.
4. **Locate** the Downloaded File
    - Find the ZIP file in your Downloads folder.
5. **Extract** the ZIP File
    - **Right-click** the file
    - **Select** “Extract All”
6. **Open** the Extracted Folder
    - **Navigate** into the unzipped project directory.
7. **Open** in an Editor
    - **Open** the folder using Visual Studio Code or another IDE.
8. **Review** the Project Files
    - **Ensure** all files are accessible and intact.
9. **Make** Changes Locally
    - **Edit** the code as needed.
10. **Initialize** Git (optional)
    - If you want version control:
