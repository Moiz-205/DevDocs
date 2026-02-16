# **Git Commands Documentation**

A guide for **Git commands**.


---

## Repository Initialization and Cloning

- Initialize a New Repository

```bash
git init
```

- Clone an Existing Repository

```bash
git clone <repository-url>
```

---

## Basic Workflow

- Check Repository Status

```bash
git status
```

> Shows modified, staged, and untracked files.


- Stage Files

```bash
git add <file>
```

> To stage a specific file

```bash
git add .
```

> To stage all changes

- Commit Changes

```bash
git commit -m "commit message"
```

To commit staged files

```bash
git commit -am "commit message"
```

> To stage and commit tracked files together

---

## Remote Repository Operations

- Push Changes (First Time)

```bash
git push -u origin main
```

- Push Changes (After First Push)

```bash
git push
```

- Pull Changes

```bash
git pull
```

> Download and merge all remote updates

- Fetch Changes (Without Merge)

```bash
git fetch
```

> Downloads remote updates without modifying local files.

---

## Branching

- List Branches

```bash
git branch
```

- Create a New Branch

```bash
git branch <branch-name>
```

- Switch Branch

```bash
git checkout <branch-name>
```

- Create and Switch Branch

```bash
git checkout -b <branch-name>
```

- Delete a Branch

```bash
git branch -d <branch-name>
```

> Deletes a local branch (safe delete).

---

## Merging and History Control

- Merge a Branch

```bash
git merge <branch-name>
```

> Integrates changes from another branch into the current one.

- Revert a Commit

```bash
git revert <commit-hash>
```

> Creates a new commit that undoes a previous commit.

---

## End of Git Documentation
