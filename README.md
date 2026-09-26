# Git Branching & Merging — Practical

## 1. Clone Repository

```bash
git clone <repository-url>
cd <repository-name>
```

## 2. Check Current Branch

```bash
git branch
```

## 3. Create a New Branch

```bash
git switch -c feature
```

## 4. Check Branches

```bash
git branch
```

Expected:

```text
* feature
  main
```

## 5. Make Changes

Edit your project files in VS Code.

## 6. Check Changes

```bash
git status
```

## 7. Stage Changes

```bash
git add README.md
```

Or stage all changed files:

```bash
git add .
```

## 8. Commit Changes

```bash
git commit -m "Add feature branch practice"
```

## 9. Push Feature Branch to GitHub

```bash
git push -u origin feature
```

## 10. Create Pull Request

GitHub → `Compare & pull request`

Then:

```text
base: main
compare: feature
```

Click:

**Create pull request → Merge pull request → Confirm merge**

## 11. Switch Back to Main

```bash
git switch main
```

## 12. Get the Updated Main from GitHub

```bash
git pull origin main
```

---

# Important Git Commands

### Push

```bash
git push
```

**Computer → GitHub**

### Pull

```bash
git pull origin main
```

**GitHub → Computer**

### Branch

```bash
git switch -c feature
```

**Create a new branch and switch to it.**

### Merge

```text
feature → main
```

**Combine the feature branch changes into main.**

---

# Simple Workflow

```text
main
  ↓
create feature branch
  ↓
work on feature
  ↓
git add
  ↓
git commit
  ↓
git push
  ↓
Pull Request
  ↓
Merge into main
  ↓
git switch main
  ↓
git pull origin main
```
