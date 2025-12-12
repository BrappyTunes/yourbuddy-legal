# Quick Start - GitHub Pages Deployment

## 🚀 Deploy in 3 Steps

### Step 1: Create GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. Repository name: `yourbuddy-legal` (or any name)
3. Make it **Public** ✅ (required for free GitHub Pages)
4. Click "Create repository"

### Step 2: Push Files

```bash
cd legal-docs
git init
git add .
git commit -m "Add legal documents"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/yourbuddy-legal.git
git push -u origin main
```

Replace `YOUR_USERNAME` with your GitHub username.

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages** (left sidebar)
3. Under "Source":
   - Branch: `main`
   - Folder: `/ (root)`
4. Click **Save**

## ✅ Done!

Your legal documents are now live at:

- **Privacy Policy:** `https://YOUR_USERNAME.github.io/yourbuddy-legal/privacy-policy.html`
- **Terms of Service:** `https://YOUR_USERNAME.github.io/yourbuddy-legal/terms-of-service.html`
- **Index:** `https://YOUR_USERNAME.github.io/yourbuddy-legal/`

## 📝 Next Steps

1. ✅ Test the URLs work in your browser
2. ✅ Copy the Privacy Policy URL
3. ✅ Use it in App Store Connect and Google Play Console
4. ✅ You're ready to submit! 🎉

## 🔄 Updating Documents

When you need to update:

1. Edit `PRIVACY_POLICY.md` or `TERMS_OF_SERVICE.md` in main repo
2. Run: `node legal-docs/convert.js`
3. Commit and push:
   ```bash
   cd legal-docs
   git add .
   git commit -m "Update legal documents"
   git push
   ```

GitHub Pages updates automatically within a few minutes!

---

**Need help?** See `DEPLOYMENT_GUIDE.md` for detailed instructions.

