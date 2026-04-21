# Push to GitHub Guide

## ✅ Local Git Setup Complete

Your local repository is ready with:
- ✅ Git initialized
- ✅ All files committed
- ✅ Ready to push to GitHub

---

## 🚀 Step 1: Create GitHub Repository (2 minutes)

1. **Go to GitHub**: https://github.com/new

2. **Repository Settings**:
   - **Repository name**: `wellness-initiative` (or your preferred name)
   - **Description**: "Team Wellbeing Initiative wellness poster with Monday.com feedback integration"
   - **Visibility**: 
     - ✅ **Public** (recommended for GitHub Pages)
     - ⚠️ Private (requires GitHub Pro for Pages)
   - **Initialize**: 
     - ❌ Do NOT add README
     - ❌ Do NOT add .gitignore
     - ❌ Do NOT add license
     (We already have these files)

3. **Click**: "Create repository"

---

## 🔗 Step 2: Push Your Code (30 seconds)

After creating the repository, GitHub will show you commands. Use these:

### Copy Your Repository URL
GitHub will show something like:
```
https://github.com/YOUR_USERNAME/wellness-initiative.git
```

### Run These Commands

```bash
cd "Work_Documentation/01_Active_Projects/Team_Wellbeing_Initiative/wellness-project"

# Add GitHub as remote
git remote add origin https://github.com/YOUR_USERNAME/wellness-initiative.git

# Push to GitHub
git branch -M main
git push -u origin main
```

**Replace `YOUR_USERNAME` with your actual GitHub username!**

---

## 🌐 Step 3: Enable GitHub Pages (1 minute)

1. **Go to your repository** on GitHub

2. **Click**: Settings (top right)

3. **Scroll to**: "Pages" (left sidebar)

4. **Configure**:
   - **Source**: Deploy from a branch
   - **Branch**: `main`
   - **Folder**: `/ (root)`

5. **Click**: Save

6. **Wait 1-2 minutes** for deployment

7. **Your site will be live at**:
   ```
   https://YOUR_USERNAME.github.io/wellness-initiative/
   ```

---

## 📝 Step 4: Update Monday.com Form URL

1. **Create form** in Monday.com (follow QUICK_FORM_CREATION.md)

2. **Get form URL** from Monday.com

3. **Edit `index.html`**:
   - Find line ~330: `YOUR_MONDAY_FORM_URL_HERE`
   - Replace with your actual form URL

4. **Commit and push**:
   ```bash
   git add index.html
   git commit -m "Add Monday.com form URL"
   git push
   ```

---

## ✨ You're Done!

Your wellness poster will be live at:
```
https://YOUR_USERNAME.github.io/wellness-initiative/
```

Share this URL with your team! 🎉

---

## 🔧 Troubleshooting

### If push fails with authentication error:

**Option 1: Use Personal Access Token**
1. Go to: https://github.com/settings/tokens
2. Generate new token (classic)
3. Select scopes: `repo`, `workflow`
4. Copy token
5. When pushing, use token as password

**Option 2: Use SSH**
1. Set up SSH key: https://docs.github.com/en/authentication/connecting-to-github-with-ssh
2. Change remote URL:
   ```bash
   git remote set-url origin git@github.com:YOUR_USERNAME/wellness-initiative.git
   ```

### If GitHub Pages doesn't work:
- Ensure repository is **Public**
- Wait 2-3 minutes after enabling Pages
- Check Settings > Pages for deployment status
- Look for green checkmark ✅

---

## 📞 Need Help?

If you encounter any issues, let me know and I'll help troubleshoot!