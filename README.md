***************************
README.md file
***************************
1. you can create directly while creating the repository
2. create README.md to your local repository and then upload using git commands
3. 

# Github notes
## Github highlights
``` this is test notes ````

# Github notes
## Github highlights
``` this is test notes ````

# 📘 Git & GitHub – Complete Beginner Notes

This README contains **end‑to‑end Git & GitHub notes** for beginners. It covers everything from basic commands to branching, conflicts, and pushing code to GitHub.

---

## 📌 What is Git?

Git is a **Distributed Version Control System (DVCS)** used to track changes in source code and collaborate with multiple developers.

### Why Git?

* Track code history
* Work in parallel using branches
* Easy rollback of mistakes
* Team collaboration

---

## 📌 What is GitHub?

GitHub is a **cloud-based hosting service** for Git repositories.

### Git vs GitHub

| Git                  | GitHub                  |
| -------------------- | ----------------------- |
| Version control tool | Online hosting platform |
| Works locally        | Works on cloud          |
| Tracks code changes  | Stores & shares code    |

---

## 📁 Git Areas (Very Important)

```
Working Directory → Staging Area → Repository (Snapshot)
        git add        git commit
```

---

## 🛠️ Basic Git Bash Commands

### File & Folder Commands

```bash
ls        # list files
pwd       # current directory
cd folder # move into folder
cd ..     # move back
mkdir dir # create folder
touch f   # create file
rm f      # delete file
```

---

## 🔧 Git Configuration

### Check Git Version

```bash
git --version
```

### Set Username & Email

```bash
git config --global user.name "Your Name"
git config --global user.email "you@email.com"
```

### View Config

```bash
git config --list
```

---

## 🚀 Initialize Repository

```bash
git init
```

Creates a `.git` folder and turns directory into a Git repo.

---

## 📄 Git Status

```bash
git status
```

Shows:

* Untracked files
* Staged files
* Modified files

---

## ➕ git add (Staging)

### Add single file

```bash
git add file1.txt
```

### Add all files

```bash
git add .
```

---

## 📸 git commit (Snapshot)

```bash
git commit -m "commit message"
```

Saves staged changes permanently in Git history.

---

## 📜 View Commit History

```bash
git log
git log --oneline
```

---

## 🔄 Remove Files from Staging

### Unstage single file

```bash
git reset file1.txt
```

### Unstage all files

```bash
git reset
```

---

## ⏪ Undo Commits

| Command                    | Meaning                    |
| -------------------------- | -------------------------- |
| `git reset --soft HEAD~1`  | Remove commit, keep staged |
| `git reset --mixed HEAD~1` | Remove commit, keep files  |
| `git reset --hard HEAD~1`  | Remove commit & files      |
| `git revert HEAD`          | Safe undo with new commit  |

---

## 🌿 Branches

### What is a Branch?

A branch is an **independent line of development**.

### List branches

```bash
git branch
```

### Create branch

```bash
git branch feature1
```

### Switch branch

```bash
git switch feature1
```

### Create & switch

```bash
git switch -c feature1
```

### Delete branch

```bash
git branch -d feature1
```

---

## 🔀 Merge Branch

```bash
git checkout main
git merge feature1
```

---

## ⚔️ Git Conflict

### What is Conflict?

Occurs when **same file & same line** are modified in different branches.

### Conflict Markers

```text
Main branch code
```

### Resolve Conflict Steps

1. Edit file manually
2. Remove conflict markers
3. `git add file`
4. `git commit`

---

## 🌍 Upload Local Code to GitHub

### Steps

```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/username/repo.git
git branch -M main
git push -u origin main
```

---

## 🔐 Authentication Note

GitHub no longer supports passwords.
Use **Personal Access Token (PAT)** as password.

---

## 🔄 Daily Git Workflow

```bash
git status
git add .
git commit -m "message"
git push
```

---

## 🎯 Interview Quick Answers

* **git add** → staging
* **git commit** → snapshot
* **branch** → parallel work
* **merge** → combine branches
* **conflict** → same file, same line

---

## ✅ Conclusion

These notes cover **complete Git & GitHub fundamentals** required for:

* Beginners
* Interviews
* Real‑world projects

Happy Learning 🚀