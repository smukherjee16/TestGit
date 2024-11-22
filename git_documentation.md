Here’s a comprehensive list of **handy Git commands**, categorized by common use cases, to help you navigate your Git workflow efficiently.

---

### **1. Setup and Configuration**
- Set global username and email:
  ```bash
  git config --global user.name "Your Name"
  git config --global user.email "your.email@example.com"
  ```
- Check current configuration:
  ```bash
  git config --list
  ```
- Set default branch name:
  ```bash
  git config --global init.defaultBranch main
  ```

---

### **2. Repository Initialization and Cloning**
- Initialize a new repository:
  ```bash
  git init
  ```
- Clone an existing repository:
  ```bash
  git clone <repository-url>
  ```

---

### **3. Branch Management**
- List all branches (local and remote):
  ```bash
  git branch -a
  ```
- Create and switch to a new branch:
  ```bash
  git checkout -b <branch-name>
  ```
- Switch to an existing branch:
  ```bash
  git checkout <branch-name>
  ```
- Delete a branch:
  ```bash
  git branch -d <branch-name>  # Safe deletion (only if merged)
  git branch -D <branch-name>  # Force deletion
  ```
- Push a new branch to the remote:
  ```bash
  git push -u origin <branch-name>
  ```

---

### **4. Making Changes**
- Check the status of the repository:
  ```bash
  git status
  ```
- Stage changes:
  ```bash
  git add <file-name>  # Stage specific file
  git add .            # Stage all changes
  ```
- Commit changes:
  ```bash
  git commit -m "Commit message"
  ```
- Amend the last commit:
  ```bash
  git commit --amend -m "Updated commit message"
  ```

---

### **5. Viewing History**
- View commit history:
  ```bash
  git log
  ```
- View commit history in one line:
  ```bash
  git log --oneline
  ```
- View changes in a file:
  ```bash
  git diff <file-name>
  ```
- Compare the working directory with the last commit:
  ```bash
  git diff
  ```

---

### **6. Synchronizing with Remote**
- Fetch latest changes (without merging):
  ```bash
  git fetch
  ```
- Pull latest changes (with merging):
  ```bash
  git pull origin <branch-name>
  ```
- Push changes to the remote:
  ```bash
  git push origin <branch-name>
  ```

---

### **7. Tagging**
- Create a tag:
  ```bash
  git tag <tag-name>
  ```
- List all tags:
  ```bash
  git tag
  ```
- Push a tag to the remote:
  ```bash
  git push origin <tag-name>
  ```

---

### **8. Undoing Changes**
- Unstage changes:
  ```bash
  git reset <file-name>
  ```
- Discard changes in the working directory:
  ```bash
  git checkout -- <file-name>
  ```
- Revert a commit:
  ```bash
  git revert <commit-hash>
  ```
- Reset to a previous commit:
  ```bash
  git reset --hard <commit-hash>
  ```

---

### **9. Stashing**
- Stash current changes:
  ```bash
  git stash
  ```
- List all stashes:
  ```bash
  git stash list
  ```
- Apply the most recent stash:
  ```bash
  git stash apply
  ```
- Drop a stash:
  ```bash
  git stash drop
  ```

---

### **10. Collaboration and Pull Requests**
- Create a pull request via GitHub CLI (if installed):
  ```bash
  gh pr create
  ```
- Link your local branch to a remote branch:
  ```bash
  git branch --set-upstream-to=origin/<branch-name>
  ```

---

### **11. Inspecting and Debugging**
- Show the commit history for a file:
  ```bash
  git log -- <file-name>
  ```
- Show who modified a file (blame):
  ```bash
  git blame <file-name>
  ```

---

### **12. Cleanup**
- Remove untracked files and directories:
  ```bash
  git clean -f
  git clean -fd  # Include directories
  ```
- Prune remote-tracking branches no longer on the remote:
  ```bash
  git fetch --prune
  ```

---

### **13. Advanced Commands**
- Cherry-pick a commit:
  ```bash
  git cherry-pick <commit-hash>
  ```
- Squash multiple commits:
  ```bash
  git rebase -i <base-branch>
  ```
- Merge a branch into the current branch:
  ```bash
  git merge <branch-name>
  ```

---

By mastering these commands, you can handle most Git workflows efficiently! Let me know if you'd like details on any specific command or workflow.