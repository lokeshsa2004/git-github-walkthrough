
---

```md
#  Git & GitHub – Learning Progress & Technical Report

##  Objective

To gain **practical, production-grade understanding of Git and GitHub**, beyond basic commands, including conflict handling, history rewriting, debugging, and safe collaboration.

---

##  Learning Approach

- Hands-on execution (not theory-only)
- Intentional creation of mistakes
- Conflict simulation and recovery
- Real GitHub interaction (SSH, PRs, remotes)
- Repetition of industry workflows

---

##  Topics Covered

### 1. Git Fundamentals
- Repository initialization
- Working tree vs staging vs commits
- Commit creation and inspection
- File tracking and ignoring

### 2. Configuration & Identity
- Global vs repo-level config
- Author correction using `commit --amend`
- Default branch configuration

---

### 3. Branching Strategy
- Feature branching
- Safe deletion of merged branches
- Branch isolation for experimentation

---

### 4. Merging & Conflict Resolution
- Fast-forward merges
- Manual merge conflict resolution
- Conflict markers and resolution flow
- Merge abort and recovery

---

### 5. Undo & History Management
- Soft vs hard resets
- Undoing commits safely
- Reverting commits in shared history
- Using `reflog` as a recovery mechanism

---

### 6. Remote Repositories & GitHub
- HTTPS vs SSH authentication
- SSH key generation and setup
- Remote URL management
- Push rejections and resolution
- Force-with-lease usage and safety

---

### 7. Pull Request Workflow
- Feature branch PRs
- Review and merge strategies
- Branch cleanup
- Syncing local with remote

---

### 8. Rebase (Advanced Topic)
- Rebase vs merge conceptual differences
- Rebase on feature branches
- Rebase with conflicts
- Commit-by-commit conflict resolution
- Abort, skip, and continue during rebase
- Detached HEAD understanding

---

### 9. Debugging with Git
- `git bisect` for regression identification
- Good/bad commit marking
- Automated bisect concepts

---

### 10. Inspection & Accountability
- `git blame` for line-level ownership
- `git show` for commit-level diffs
- Understanding merge commits deeply

---

##  Key Challenges Faced

- Rebase conflicts occurring multiple times
- Authentication failures with HTTPS
- Push rejections due to divergent histories
- Editor issues during rebase (`nano` / `vi`)
- Managing detached HEAD states

---

##  Key Learnings

- Git is about **state transitions**, not commands
- History rewriting must be treated with care
- Rebase is safe when scoped correctly
- Force push is not dangerous if used correctly
- Git provides recovery tools for almost every mistake

---

##  Production-Safe Practices Adopted

- No force push on shared branches
- PR-based development
- Revert instead of reset in shared repos
- Clean commit history before merging
- SSH-based authentication

---

##  Outcome

By the end of this exercise:
- All core and advanced Git commands were executed
- Real-world workflows were simulated
- Confidence gained in resolving complex Git states
- Ability to explain Git behavior clearly in interviews
- Readiness to use Git safely in production environments



---

## ✅ Conclusion

This repository represents a **complete Git learning lifecycle**, emphasizing correctness, safety, and real-world applicability rather than memorization.

---
