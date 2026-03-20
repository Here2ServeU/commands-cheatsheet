# Git Command Master List (Professional Reference)

## 1. Setup and Configuration
```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
git config --list
git config --global init.defaultBranch main
git config --global core.editor "code --wait"
```

## 2. Repository Initialization and Cloning
```bash
git init
git clone <repo-url>
git clone <repo-url> <folder-name>
```

## 3. Status and History
```bash
git status
git log
git log --oneline
git log --graph --oneline --all
git show <commit-id>
git diff
git diff <file>
git diff <branch1> <branch2>
```

## 4. Staging and Committing
```bash
git add .
git add <file>
git add -A
git commit -m "message"
git commit -am "message"
git commit --amend
```

## 5. Branching and Switching
```bash
git branch
git branch <branch-name>
git checkout <branch-name>
git checkout -b <branch-name>
git switch <branch-name>
git switch -c <branch-name>
git branch -d <branch-name>
```

## 6. Merging and Rebasing
```bash
git merge <branch>
git rebase <branch>
git rebase -i HEAD~3
git merge --abort
git rebase --abort
```

## 7. Remote Repositories
```bash
git remote -v
git remote add origin <url>
git remote remove origin
git remote rename origin new-name
```

## 8. Push and Pull
```bash
git push
git push origin main
git push -u origin main
git pull
git pull origin main
git fetch
git fetch --all
```

## 9. Undo and Reset
```bash
git reset
git reset --soft HEAD~1
git reset --hard HEAD~1
git restore <file>
git checkout -- <file>
git revert <commit-id>
```

## 10. Stashing
```bash
git stash
git stash list
git stash apply
git stash pop
git stash drop
```

## 11. Tagging
```bash
git tag
git tag v1.0
git tag -a v1.0 -m "release"
git push origin v1.0
git push --tags
```

## 12. Inspecting and Debugging
```bash
git blame <file>
git bisect start
git bisect bad
git bisect good
git grep "search-term"
```

## 13. Cleanup
```bash
git clean -f
git clean -fd
git rm <file>
git rm -r <folder>
```

## 14. Submodules
```bash
git submodule add <repo-url>
git submodule update --init --recursive
git submodule update --remote
```

## 15. Advanced Commands
```bash
git cherry-pick <commit-id>
git reflog
git shortlog
git archive
git worktree add ../new-folder branch-name
```

## Core Workflow
```bash
git add .
git commit -m "message"
git push origin main
```

## Feature Workflow
```bash
git checkout -b feature/new-feature
git add .
git commit -m "feature added"
git push origin feature/new-feature
```
