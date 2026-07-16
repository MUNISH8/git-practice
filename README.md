# Git & GitHub Practice Exercise Report

**Name:** Munish Sarker,
**Student ID:** 24-57375-2,
**Section:** DD

## Introduction

This report documents the hands-on exercise performed to learn the fundamentals of **Git** and **GitHub** as part of the Software Engineering course. The exercise involved creating a GitHub repository, adding a C++ source file, cloning the repository locally, modifying the file, and pushing the updated changes back to GitHub. The purpose of this exercise was to build practical familiarity with the standard Git workflow used in collaborative software development.

## Objective

The main objectives of this exercise were to:

- Create a new repository on GitHub.
- Add and commit an initial file directly through the GitHub web interface.
- Clone the repository to a local machine.
- Modify the file locally and observe the changes using Git commands.
- Stage, commit, and push the changes back to the remote repository.

## Tools Used

- **Git** — version control system used locally.
- **GitHub** — remote hosting platform for the repository.
- **Terminal / Git Bash** — command-line interface used to execute Git commands.
- **Code Editor** — used to modify the `main.cpp` file.

## Procedure

### Step 1: Repository Creation
A new public repository named `git-practice` was created on GitHub.

### Step 2: Adding the Initial File
A file named `main.cpp` was created directly on GitHub containing the provided C++ code, and committed with the message *"Initial commit"*.

### Step 3: Cloning the Repository
The repository was cloned to the local machine using:
```bash
git clone <repository_url>
cd git-practice
```

### Step 4: Checking Repository Status
The status of the repository was verified using:
```bash
git status
```
The output confirmed a clean working tree on the `main` branch.

### Step 5: Modifying the File
The `main.cpp` file was opened locally, and the following fields were updated:

- Name
- Student ID
- Section

An additional field, *[e.g., Favorite Programming Language]*, was also added.

### Step 6: Viewing the Changes
The differences between the original and modified files were viewed using:
```bash
git diff
git status
```
This showed `main.cpp` as a modified file.

### Step 7: Staging the Changes
The modified file was staged for commit using:
```bash
git add main.cpp
```
or, alternatively, to stage all changes:
```bash
git add .
```

### Step 8: Committing the Changes
The staged changes were committed with a descriptive message:
```bash
git commit -m "Updated student information"
```

### Step 9: Pushing the Changes
Finally, the commit was pushed to the remote GitHub repository:
```bash
git push
```
The GitHub repository was refreshed in the browser to confirm that the updated `main.cpp` file was successfully uploaded.

## Git Commands Practiced

| Command | Purpose |
|---|---|
| `git clone` | Copies a remote repository to the local machine |
| `git status` | Displays the current state of the working directory |
| `git diff` | Shows differences between file versions |
| `git add` | Stages changes for the next commit |
| `git commit` | Records staged changes into repository history |
| `git push` | Uploads local commits to the remote repository |

## Observations

- Git tracks file changes at the line level, allowing precise identification of modifications via `git diff`.
- The staging area (`git add`) acts as an intermediate step, giving control over exactly which changes are included in a commit.
- Commit messages are important for maintaining a clear and understandable project history.
- `git push` synchronizes local commits with the remote repository, making changes visible to collaborators.

## Conclusion

This exercise provided practical, hands-on experience with the essential Git and GitHub workflow: creating a repository, cloning it, modifying files locally, and synchronizing changes with the remote repository. Understanding this cycle of `clone → modify → status → diff → add → commit → push` is fundamental to version control and forms the basis of collaborative software development practices used throughout the software industry.
