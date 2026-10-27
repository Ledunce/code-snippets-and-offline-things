https://drive.google.com/file/d/1cgj7yeYOf0tubP8VkhOtZkpGE4LeOW3E/view?usp=sharing

https://github.com/vahid-kazemi/W3Schools_offline

https://git-scm.com/install/windows?utm_source=chatgpt.com

Install Git itself first, then configure it once. For Windows:

1. Download the installer while online

Get Git for Windows. Save the installer on your laptop or USB so you can install it offline later. A portable version is also available. git-scm.com

2. Install, then restart VS Code and its terminal

Check:
git --version

If Git isn’t recognized, open a new terminal after installation.

3. Initialize your project

Open the terminal inside your project folder. For a new repository:
git init -b main

If the project already has Git history, use git status and keep that existing repository.

4. Set your commit identity

For an assessment/shared computer, configure it for this project:
git config user.name "Peter Gabriel Rosales"
git config user.email "your-email@example.com"

Replace the email with your actual email. On your own computer, adding --global applies the identity to all your repositories.

5. Check .gitignore before adding files

Keep any existing rules and ensure these are included:
node_modules/
dist/
.env
.env.*
!.env.example

Your .env.example should contain public configuration or placeholders.

6. Create your first commit
git add .
git diff --cached --stat
git commit -m "Initial project setup"
git status

Inspect the staged file list before committing.

Git commits work offline. GitHub access is needed only when communicating with a remote repository.

If the computer is already offline, you’ll need a previously downloaded installer or portable Git copy transferred by USB.
