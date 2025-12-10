# Quick Deployment Guide for GitHub Pages

## 🚀 Fastest Way to Deploy

### Step 1: Create GitHub Repository

1. Go to [github.com](https://github.com) and sign in
2. Click the "+" icon → "New repository"
3. Name it (e.g., `myhomepage`)
4. Make it **Public** (required for free GitHub Pages)
5. **Don't** initialize with README, .gitignore, or license
6. Click "Create repository"

### Step 2: Upload Files

**Option A: Using GitHub Web Interface (Easiest)**

1. In your new repository, click "uploading an existing file"
2. Drag and drop ALL files from `myhomepage-static` folder:
   - `index.html`
   - `styles.css`
   - `script.js`
   - `cv.pdf`
   - `README.md`
   - `.gitignore`
3. Scroll down, add commit message: "Initial commit"
4. Click "Commit changes"

**Option B: Using Git (Recommended for updates)**

```bash
cd /Users/yanhe/Downloads/myhomepage-static

# Initialize git
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit - Static homepage"

# Add your GitHub repository (replace YOUR_USERNAME and REPO_NAME)
git remote add origin https://github.com/YOUR_USERNAME/REPO_NAME.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (top menu)
3. Scroll down to **Pages** (left sidebar)
4. Under **Source**:
   - Select **"Deploy from a branch"**
   - Branch: **main**
   - Folder: **/ (root)**
5. Click **Save**

### Step 4: Access Your Site

- Your site will be live at: `https://YOUR_USERNAME.github.io/REPO_NAME/`
- It may take 1-5 minutes to deploy
- GitHub will show the URL in the Pages settings

## ✅ Verification Checklist

- [ ] All files uploaded to GitHub
- [ ] Repository is Public
- [ ] GitHub Pages enabled in Settings
- [ ] Site URL is accessible
- [ ] Matrix rain animation works
- [ ] Typewriter effect works
- [ ] Navigation links work
- [ ] CV download works

## 🔄 Updating Your Site

After making changes:

**Using Git:**
```bash
git add .
git commit -m "Update homepage"
git push
```

**Using Web Interface:**
- Edit files directly on GitHub
- Or upload new versions

Changes will be live in 1-5 minutes.

## 🎨 Custom Domain (Optional)

1. In GitHub Pages settings, add your custom domain
2. Update DNS records at your domain provider:
   - Type: `CNAME`
   - Name: `www` (or `@`)
   - Value: `YOUR_USERNAME.github.io`
3. Wait for DNS propagation (can take up to 24 hours)

## 🐛 Troubleshooting

**Site not loading?**
- Check if repository is Public
- Verify GitHub Pages is enabled
- Wait a few minutes for deployment
- Check repository name matches URL

**Styles not working?**
- Verify `styles.css` is in root directory
- Check browser console for errors
- Ensure file paths are correct

**JavaScript not working?**
- Verify `script.js` is in root directory
- Check browser console for errors
- Ensure JavaScript is enabled in browser

## 📝 Notes

- GitHub Pages serves files from the root directory
- File names are case-sensitive
- Use relative paths (e.g., `cv.pdf` not `/cv.pdf`)
- Maximum repository size: 1GB
- Maximum file size: 100MB

---

**Need help?** Check the main README.md or open an issue on GitHub.

