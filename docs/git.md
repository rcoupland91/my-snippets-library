# Git Branching & Workflow

Commonly used commands for managing local branches and syncing with remote repositories.

---

### Update Local Main
Always ensure your local environment is up to date before starting new work.
```bash title="Sync with Remote"
git pull origin main
```

### Create a New Branch
Use this to create and switch to a new feature branch.
```bash title="Checkout"
git checkout -b "feature/your-branch-name"
```

### Stage All Changes
Stage all modified and new files ready for commit.
```bash title="Stage"
git add -A
```

### Commit All Changes
Commit staged changes with a descriptive message.
```bash title="Commit"
git commit -m "description of commit"
```

### Push and Link to Remote
Push your branch and set the upstream tracking reference.
```bash title="Push"
git push --set-upstream origin feature/your-branch-name
```
