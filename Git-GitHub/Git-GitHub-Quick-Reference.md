# Git & GitHub – Quick Reference
A personal handbook of Git commands, their purpose, and practical use cases.
# First-Time Project Upload to GitHub
Use these commands when uploading a local project to GitHub for the first time.

```
# 1. Initialize Git
git init

# 2. Check current status
git status

# 3. Connect local project to GitHub
git remote add origin https://github.com/USERNAME/REPOSITORY.git

# 4. Verify remote connection
git remote -v

# 5. Stage all files
git add .

# 6. Check staged files
git status

# 7. Create first commit
git commit -m "Initial commit"

# 8. Rename branch to main
git branch -M main

# 9. Push project to GitHub
git push -u origin main
```



Note:
- git init , git remote add origin and git branch -M main – Only once per local project.
- These steps assume the GitHub repository is empty. If it already contains a README or other files, synchronize the histories before pushing.

# Updating an Existing Repository
Use these commands whenever you make changes to an already-uploaded project.
```
# 1. Check modified/new files
git status

# 2. Stage all changes
git add .

# 3. Verify staged changes
git status

# 4. Commit changes
git commit -m "Describe your changes"

# 5. Push changes to GitHub
git push
```




# Important Git Concepts
Concept	Meaning
- Repository	Project tracked by Git
- Working Directory	Where you modify files
- Staging Area	Files prepared for commit
- Commit	Snapshot of changes
- Remote	GitHub repository connected to local Git
- Branch	Separate line of development
- Push	Upload local commits
- Pull	Bring remote changes locally
- Clone	Copy a remote repository locally
- Merge	Combine changes from branches
- Pull Request	Request to merge changes into another branch



Remember:
1. Add → Prepare changes.
2. Commit → Save changes locally.
3. Push → Upload changes to GitHub.


Important: .gitignore prevents untracked files from being added, but it does not remove secrets that were already committed. If a secret is exposed, rotate it immediately.
