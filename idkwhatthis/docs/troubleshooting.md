# Troubleshooting

| Symptom | Probable Cause | Action |
|---------|----------------|--------|
| Git Bash does not appear in the VS Code terminal profile list | Git for Windows is not installed, or VS Code did not detect Git Bash automatically | Install Git for Windows, then restart VS Code. If it still does not appear, manually add the Git Bash profile in `settings.json`. |
| Git Bash opens in VS Code but does not work correctly | The Git Bash executable path is incorrect | Check that the path points to the correct file, such as `C:\Program Files\Git\bin\bash.exe`. |
| The terminal opens PowerShell instead of Git Bash | Git Bash was not selected as the default terminal profile | Open the terminal profile menu in VS Code and set **Git Bash** as the default profile. |
| `git` is not recognized as a command | Git is not installed or was not added to the system PATH | Reinstall Git for Windows and ensure Git is added to PATH during installation. Restart the terminal afterward. |
| Unable to create a new repository on GitHub | You are not signed in, or the repository name is already in use | Sign in to GitHub and choose a unique repository name. |
| The **New repository** option is missing | You may not be signed in correctly, or you do not have permission in the selected organization | Confirm you are signed in to the correct GitHub account and check organization permissions if applicable. |
| `git init` does not work | The terminal is not opened in the correct project folder | Navigate to the project directory first, then run `git init` again. |
| `git add .` does not stage files | You may be in the wrong folder, or there are no files in the directory | Run `git status` to confirm your current folder and check that your project files are present. |
| `git commit -m "Initial commit"` fails | Git username and email are not configured | Configure Git with `git config --global user.name "Your Name"` and `git config --global user.email "your@email.com"`, then try again. |
| `remote origin already exists` appears | A remote repository has already been linked to the local project | Check existing remotes with `git remote -v`. Update it with `git remote set-url origin <repository-url>` if needed. |
| `git push -u origin main` fails because the branch does not exist | Your local branch may still be named `master` instead of `main` | Run `git branch -M main` and then push again, or use the correct existing branch name. |
| Authentication failed when pushing to GitHub | Your login credentials are incorrect, expired, or GitHub requires a personal access token | Sign in again and use a personal access token if prompted instead of your GitHub password. |
| The repository on GitHub is empty after pushing | The push did not complete successfully, or files were never committed | Run `git status` and `git log` to confirm your files were committed, then push again. |
| `git clone` fails | The repository URL is incorrect, or you do not have permission to access the repository | Copy the repository URL again from GitHub and verify that the repository exists and is accessible to your account. |
| The cloned folder does not appear where expected | The terminal was opened in a different directory before cloning | Run `pwd` to confirm your location, then clone the repository into the correct folder. |
| Downloaded ZIP file does not include version control features | ZIP downloads do not preserve Git history or repository connection | Use `git clone` instead if you need full version control and the ability to pull or push changes. |
| Changes made after downloading a ZIP file cannot be pushed to GitHub | The ZIP method does not connect the project to GitHub automatically | Initialize Git with `git init`, add a remote repository, commit your files, and then push them manually. |