Git and GitHub – Beginner's Learning Guide

Welcome to the Git and GitHub Learning Repository! 🚀

This repository is designed to help beginners understand Git and GitHub, learn essential commands, and practice version control step by step.

📚 Table of Contents
Introduction
Git vs GitHub
Installation
Basic Git Configuration
Essential Git Commands
Working with Git
Connecting Git to GitHub
Branching and Merging
Working with Remote Repositories
Undoing Changes
Pull Requests
Common Git Commands Cheat Sheet
Hands-On Practice
Learning Resources
📌 Introduction
What is Git?

Git is a distributed version control system that tracks changes in files over time. It helps developers collaborate, manage code, and restore previous versions when needed.

What is GitHub?

GitHub is an online platform that hosts Git repositories. It allows developers to store code, collaborate with others, review changes, and manage projects.

🔍 Git vs GitHub
Git	GitHub
A version control tool	An online hosting platform
Works locally on your computer	Hosts repositories online
Tracks file changes	Enables collaboration and code sharing
Uses commands such as git commit	Provides pull requests, issues, and code reviews
💻 Installation
Install Git

Download Git for your operating system:

Windows: https://git-scm.com/install/windows
macOS: https://git-scm.com/install/mac
Linux: https://git-scm.com/install/linux

Verify the installation:

git --version


Create a free GitHub account:

https://github.com/

⚙️ Basic Git Configuration

Configure your name and email before making commits.

git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"


Check your configuration:

git config --list

🧰 Essential Git Commands
Command	Purpose
git init	Initialize a Git repository
git clone <url>	Copy a remote repository locally
git status	Check the current working tree status
git add <file>	Stage a specific file
git add .	Stage changes in the current directory
git commit -m "message"	Save a snapshot of staged changes
git log	View commit history
git diff	View unstaged changes
git branch	List local branches
git switch <branch>	Switch branches
git merge <branch>	Merge another branch into the current branch
git pull	Fetch and integrate remote changes
git push	Upload local commits to a remote repository
🔄 Working with Git

Follow these steps to create your first local repository.

Step 1: Create a project folder
mkdir git-practice
cd git-practice

Step 2: Initialize Git
git init


This creates a Git repository in the current directory.

Step 3: Create a file

Create a file named README.md and add some text to it.

Step 4: Check the status
git status


Git will show the file as untracked.

Step 5: Stage the file
git add README.md

Step 6: Commit the changes
git commit -m "Add initial README"

Step 7: View commit history
git log --oneline


Congratulations! 🎉 You have created your first Git commit.

☁️ Connecting Git to GitHub
Step 1: Create a GitHub repository
Sign in to GitHub.
Click the New repository option.
Enter a repository name, such as git-practice.
Choose public or private visibility.
Create the repository.

For an existing local project, it is simplest to create the GitHub repository without initializing it with a README, license, or .gitignore.

Step 2: Connect your local repository

Replace YOUR_USERNAME with your GitHub username.

git remote add origin https://github.com/YOUR_USERNAME/git-practice.git


Verify the remote:

git remote -v

Step 3: Rename the branch to main
git branch -M main

Step 4: Push your code to GitHub
git push -u origin main


GitHub may ask you to authenticate. Follow its authentication instructions; your GitHub account password is not accepted for HTTPS Git operations.

Your local project should now be available on GitHub! 🎉

🌿 Branching and Merging

Branches allow you to work on new features without changing the main branch directly.

Create a new branch
git branch feature-login

Switch to the branch
git switch feature-login


Or create and switch in one command:

git switch -c feature-login

Make changes and commit
git add .
git commit -m "Add login feature"

Switch back to main
git switch main

Merge the feature branch
git merge feature-login

Delete the branch after merging
git branch -d feature-login

🌐 Working with Remote Repositories
Clone a repository
git clone https://github.com/USERNAME/REPOSITORY.git

Download and integrate remote changes
git pull origin main

Upload local commits
git push origin main

Download remote information without integrating changes
git fetch origin

View configured remote repositories
git remote -v

↩️ Undoing Changes

Be careful when undoing changes, especially if commits have already been shared with others.

Discard unstaged changes in a file
git restore filename.txt


This discards uncommitted changes in that file.

Unstage a file
git restore --staged filename.txt


The file's changes remain in your working directory.

Undo a commit safely
git revert <commit-hash>


This creates a new commit that reverses the changes introduced by the specified commit.

Amend the latest commit
git commit --amend


Use this to correct the latest commit. Avoid amending commits that others have already based work on.

🤝 Pull Requests

A pull request (PR) lets you propose changes and ask others to review them before merging.

Typical workflow:

Create a feature branch.
Make changes to your files.
Stage and commit your changes.
Push the feature branch to GitHub.
Open a pull request on GitHub.
Review feedback and make any necessary updates.
Merge the pull request when approved.

Example:

git switch -c feature-about-page
git add .
git commit -m "Add about page"
git push -u origin feature-about-page


Then open GitHub and create a pull request from feature-about-page into main.

📝 Common Git Commands Cheat Sheet
# Setup
git config --global user.name "Your Name"
git config --global user.email "you@example.com"

# Start a repository
git init
git clone <repository-url>

# Track changes
git status
git add .
git diff
git commit -m "Your message"

# History
git log
git log --oneline

# Branches
git branch
git switch main
git switch -c new-feature
git merge new-feature

# Remote operations
git remote -v
git fetch origin
git pull origin main
git push origin main

# Undo changes
git restore <file>
git restore --staged <file>
git revert <commit-hash>

🏋️ Hands-On Practice

Complete these exercises to improve your Git and GitHub skills.

Install Git on your computer.
Configure your Git username and email.
Create a new local repository.
Create a README.md file.
Stage and commit your changes.
Create a GitHub repository.
Push your local project to GitHub.
Clone your repository into another folder.
Create a new branch and make a change.
Merge the branch into main.
Create a pull request on GitHub.
Practice undoing a change using git restore.
Explore commit history using git log.
📖 Learning Resources
Git Official Website: https://git-scm.com/
Git Documentation: https://git-scm.com/doc
GitHub Documentation: https://docs.github.com/
GitHub Skills: https://skills.github.com/
Learn Git Branching: https://learngitbranching.js.org/
🎯 Learning Roadmap

Recommended order for learning:

Understand version control and repositories.
Learn init, status, add, and commit.
Practice creating and cloning repositories.
Learn branches, switching, and merging.
Understand fetch, pull, and push.
Practice collaboration using pull requests.
Learn to resolve merge conflicts.
Explore advanced concepts such as rebasing, cherry-picking, and Git workflows.
⭐ Conclusion

Git helps you track and manage code changes, while GitHub helps you store projects online and collaborate with other developers.

Practice regularly, commit meaningful changes, and keep learning!

Happy Coding! 💻🚀
