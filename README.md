## GitHub Workflow
This repository documents a **complete, hands-on Git and GitHub learning journey**, covering real-world workflows, conflicts, recovery, rebasing, and collaboration.

This cheatsheet is intended for:
- Daily developer reference
- Interview preparation
- Production-safe Git usage
- Debugging and recovery scenarios

---

🔹 Git Configuration

```bash
git --version
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
git config --global init.defaultBranch main
git config --list
git config --global --edit

🔹 Repository Basics
git init
git status
git add .
git commit -m "message"
git log
git log --oneline --graph --all

🔹 Working Tree Operations
git diff
git diff --staged
git checkout -- <file>
git restore <file>

🔹 Branching
git branch
git checkout -b <branch>
git checkout <branch>
git branch -d <branch>

🔹 Merging & Conflicts
git merge <branch>
git merge --abort
Conflict resolution flow:
# edit conflicted file
git add <file>
git commit


🔹 Undo & Recovery
git reset --soft HEAD~1
git reset --hard HEAD~1
git revert <commit>
git reflog
git checkout <commit>


🔹 Commit Fixes
git commit --amend
git commit --amend --author="Name <email>"


🔹 Remote Repositories
git remote -v
git remote add origin <url>
git remote set-url origin <url>
git fetch origin
git pull origin main
git pull --rebase origin main
git push origin main
git push --force-with-lease origin main


🔹 SSH Authentication
ssh-keygen -t ed25519 -C "email"
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
ssh -T git@github.com


🔹 Stash
git stash
git stash push -m "message"
git stash list
git stash apply
git stash pop
git stash drop
git stash clear


🔹 Rebase (Advanced)
git rebase main
git rebase -i HEAD~n
git rebase --continue
git rebase --abort
git rebase --skip


🔹 Bisect (Debugging)
git bisect start
git bisect bad
git bisect good <commit>
git bisect reset
git bisect run <test-command>


🔹 Inspection
git show <commit>
git blame <file>


🔹 Pull Request Workflow
git checkout -b feature-x
git push origin feature-x
# Open PR on GitHub
# Review → Merge
git checkout main
git pull
git branch -d feature-x


🔹 Tags & Releases
git tag v1.0.0
git push origin v1.0.0

Golden Rules
Rebase only local/feature branches
Never force-push to shared branches
Revert in production, reset locally
Always inspect with git diff
Use PRs for collaboration
