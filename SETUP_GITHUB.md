# How to Save to GitHub

Your project is now saved locally with Git version control. To save it to GitHub for backup and sharing:

## Quick Setup (GitHub)

### 1. Create a GitHub Repository

1. Go to [github.com](https://github.com) and log in
2. Click the "+" icon in the top right, select "New repository"
3. Name it: `oktaadversary` or `identity-attack-training`
4. Description: "Security awareness training platform for identity attacks"
5. Choose **Private** (recommended for security tools)
6. **Do NOT** initialize with README, .gitignore, or license
7. Click "Create repository"

### 2. Push to GitHub

After creating the repository, run these commands:

```bash
cd /Users/davidfesperman/Downloads/phishing-training

# Add your GitHub repository as remote
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git

# Push your code
git push -u origin main
```

Replace `YOUR_USERNAME` and `YOUR_REPO_NAME` with your actual values.

### 3. Verify

- Refresh your GitHub repository page
- You should see all your files there

## Alternative: Push to GitLab or Bitbucket

Same process, just use their respective URLs:

**GitLab:**
```bash
git remote add origin https://gitlab.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git push -u origin main
```

**Bitbucket:**
```bash
git remote add origin https://bitbucket.org/YOUR_USERNAME/YOUR_REPO_NAME.git
git push -u origin main
```

## Making Changes Later

When you update your project:

```bash
# Check what changed
git status

# Stage specific files
git add index.html admin.html

# Or stage all changes
git add -A

# Commit with a message
git commit -m "Description of your changes"

# Push to GitHub
git push
```

## Common Git Commands

```bash
# See commit history
git log --oneline

# See what changed in files
git diff

# Create a new branch for features
git checkout -b feature-name

# Switch back to main
git checkout main

# Merge a branch
git merge feature-name
```

## Tips

- ✅ Commit frequently with clear messages
- ✅ Use branches for major new features
- ✅ Keep the repository private (this is a security tool)
- ✅ Never commit real credentials or sensitive data
- ✅ Pull before making changes if working with others: `git pull`

## Backup Without GitHub

If you prefer not to use GitHub, your local Git repository is already a backup:

```bash
# Create a backup
cd /Users/davidfesperman/Downloads
zip -r phishing-training-backup.zip phishing-training/

# Or use tar
tar -czf phishing-training-backup.tar.gz phishing-training/
```

## Project is Ready! 🎉

Your project is now:
- ✅ Version controlled with Git
- ✅ Documented with README and PROJECT_INFO
- ✅ Ready to push to GitHub
- ✅ Easy to backup and share
