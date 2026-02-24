# Git Branching & Workflow

Commonly used commands for managing local branches and syncing with remote repositories.

---

### Update Local Main
Always ensure your local environment is up to date before starting new work.
```bash title="Sync with Remote"
git pull origin main
```
### Update Local Main
Use this to checkout a new branch
```bash title="Checkout"
git checkout -b "feature/your-branch-name"
```

### Stage All Changes
Use this to checkout a new branch
```bash title="Stage"
git add -A
```

### Commit All Changes
Use this to checkout a new branch
```bash title="Commit"
git commit -m "description of commit"
```

### Push and link to remote
Use this to checkout a new branch
```bash title="Push"
git push --set-upstream origin feature/your-branch-name
```