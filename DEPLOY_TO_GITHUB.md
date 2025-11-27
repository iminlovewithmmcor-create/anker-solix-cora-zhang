# 🚀 Deploy to GitHub Pages - Complete Guide

## Step 1: Create GitHub Repository

1. Go to [GitHub.com](https://github.com)
2. Click the **"+"** button in the top right corner
3. Select **"New repository"**
4. Fill in the details:
   - **Repository name**: `anker-solix-cora-zhang`
   - **Description**: `Optimized DTC website for Anker SOLIX power stations`
   - **Visibility**: Choose **Public** (required for free GitHub Pages)
   - **DO NOT** initialize with README, .gitignore, or license (we already have files)
5. Click **"Create repository"**

## Step 2: Push Your Code to GitHub

After creating the repository, GitHub will show you commands. Use these:

```bash
cd ~/anker-solix-cora-zhang

# Add the GitHub remote (replace YOUR-USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR-USERNAME/anker-solix-cora-zhang.git

# Rename branch to main (if needed)
git branch -M main

# Push to GitHub
git push -u origin main
```

**Example:** If your GitHub username is `corazhang`, the command would be:
```bash
git remote add origin https://github.com/corazhang/anker-solix-cora-zhang.git
```

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **"Settings"** tab
3. Click **"Pages"** in the left sidebar
4. Under **"Source"**:
   - Branch: Select **main**
   - Folder: Select **/ (root)**
5. Click **"Save"**

## Step 4: Access Your Live Website

After 1-2 minutes, your website will be live at:

```
https://YOUR-USERNAME.github.io/anker-solix-cora-zhang/
```

**Example:** If your username is `corazhang`:
```
https://corazhang.github.io/anker-solix-cora-zhang/
```

## 🎉 That's It!

Your Anker SOLIX website is now live and publicly accessible!

---

## 📝 Local Files Location

All files are in: `/Users/admin/anker-solix-cora-zhang/`

- `index.html` - Main website file
- `README.md` - Project documentation
- `DEPLOY_TO_GITHUB.md` - This deployment guide

---

## 🔄 Making Updates

To update your website after making changes:

```bash
cd ~/anker-solix-cora-zhang

# Stage changes
git add .

# Commit changes
git commit -m "Update website"

# Push to GitHub
git push
```

The website will automatically update in 1-2 minutes!

---

## 🆘 Troubleshooting

### Problem: "remote origin already exists"
**Solution:**
```bash
git remote remove origin
git remote add origin https://github.com/YOUR-USERNAME/anker-solix-cora-zhang.git
```

### Problem: Website shows 404
**Solutions:**
1. Wait 2-3 minutes - GitHub Pages takes time to deploy
2. Check that GitHub Pages is enabled in Settings → Pages
3. Verify the branch is set to `main`
4. Make sure the file is named `index.html` (not `index.htm` or other)

### Problem: Authentication failed when pushing
**Solutions:**
1. Use a Personal Access Token instead of password
2. Generate token at: [GitHub Settings → Developer settings → Personal access tokens](https://github.com/settings/tokens)
3. Use the token as your password when prompted

---

## 📊 Repository Stats

- **Branch:** main
- **Commits:** 2
- **Files:** 2 (index.html, README.md)
- **Size:** ~90KB

---

**Need help?** Feel free to reach out!

🤖 *Generated with [Claude Code](https://claude.com/claude-code)*
