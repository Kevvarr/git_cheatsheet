# 🌱 Git Command Cheat Sheet

---

## ⚙️ Git Setup

| Command | Description |
|--------|-------------|
| `git config --global user.name "Your Name"` | Set global username |
| `git config --global user.email "you@example.com"` | Set global email |
| `git config --list` | View current Git configuration |
| `git init` | Initialize a new Git repository |

---

## 📦 Basic Workflow

| Command | Description |
|--------|-------------|
| `git clone <repo-url>` | Clone remote repository |
| `git status` | Show working tree status |
| `git add <file>` | Stage a specific file |
| `git add .` | Stage all modified files |
| `git commit -m "message"` | Commit staged changes |
| `git push` | Push local commits to remote |
| `git pull` | Fetch and merge latest changes |
| `git log` | View commit history |
| `git diff` | Show file differences not yet staged |

---

## 🌿 Branching

| Command | Description |
|--------|-------------|
| `git branch` | List all local branches |
| `git branch <name>` | Create a new branch |
| `git checkout <name>` | Switch to a branch |
| `git checkout -b <name>` | Create and switch to a new branch |
| `git merge <branch>` | Merge another branch into current one |
| `git branch -d <name>` | Delete a local branch |
| `git push origin --delete <name>` | Delete a remote branch |

---

## 🤝 Remote Collaboration

| Command | Description |
|--------|-------------|
| `git remote -v` | Show current remotes |
| `git remote add origin <url>` | Add a remote repository |
| `git push -u origin <branch>` | Push a branch and set upstream |
| `git pull origin <branch>` | Pull updates from a remote branch |
| `git fetch` | Download objects from remote, no merge |

---

## 🔄 Rebasing & Syncing

| Command | Description |
|--------|-------------|
| `git pull --rebase` | Rebase instead of merge for cleaner history |
| `git rebase <branch>` | Reapply commits on top of another branch |
| `git rebase -i <commit>` | Interactive rebase to squash/edit commits |

> 💡 **Example:**  
> Keeping your feature branch up to date:  
> `git checkout feature/ui`  
> `git pull --rebase origin main`

---

## 📥 Stash & Apply

| Command | Description |
|--------|-------------|
| `git stash` | Temporarily store uncommitted changes |
| `git stash pop` | Reapply stashed changes |
| `git stash list` | List all stashes |
| `git stash drop` | Remove a specific stash |

---

## 🎯 Cherry-Pick & Revert

| Command | Description |
|--------|-------------|
| `git cherry-pick <commit>` | Apply a specific commit from another branch |
| `git revert <commit>` | Revert a commit with a new commit |
| `git reset --hard <commit>` | Reset HEAD to a specific commit (destructive) |

> 💡 **Example:**  
> Apply a hotfix commit to another branch:  
> `git checkout develop`  
> `git cherry-pick <commit-hash>`

---

## 🧼 Cleanup & Recovery

| Command | Description |
|--------|-------------|
| `git clean -fd` | Remove untracked files and directories |
| `git reset --hard` | Discard all local changes |
| `git reflog` | Show history of HEAD changes |
| `git gc` | Run garbage collection on repo |

---
