# GitHub Pages Deployment Guide

## Quick Setup (5 minutes)

### Option 1: Create New Repository (Recommended)

1. **Create a new GitHub repository:**
   - Go to [github.com/new](https://github.com/new)
   - Name it: `yourbuddy-legal` (or any name you prefer)
   - Make it **Public** (required for free GitHub Pages)
   - Don't initialize with README (we already have files)

2. **Push the legal-docs folder:**
   ```bash
   cd legal-docs
   git init
   git add .
   git commit -m "Initial commit: Legal documents"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/yourbuddy-legal.git
   git push -u origin main
   ```

3. **Enable GitHub Pages:**
   - Go to your repository on GitHub
   - Click **Settings** → **Pages** (left sidebar)
   - Under "Source", select:
     - Branch: `main`
     - Folder: `/ (root)`
   - Click **Save**

4. **Get your URLs:**
   - Your site will be live at: `https://YOUR_USERNAME.github.io/yourbuddy-legal/`
   - Privacy Policy: `https://YOUR_USERNAME.github.io/yourbuddy-legal/privacy-policy.html`
   - Terms of Service: `https://YOUR_USERNAME.github.io/yourbuddy-legal/terms-of-service.html`

### Option 2: Add to Existing Repository

If you want to add this to your main Buddy repository:

1. **Create a `docs` folder in your main repo:**
   ```bash
   mkdir docs
   cp legal-docs/*.html docs/
   ```

2. **Enable GitHub Pages:**
   - Go to repository Settings → Pages
   - Source: "Deploy from a branch"
   - Branch: `main`
   - Folder: `/docs`
   - Save

3. **Your URLs will be:**
   - `https://YOUR_USERNAME.github.io/buddy/privacy-policy.html`

## Custom Domain (Optional)

If you have a domain from Railway or elsewhere:

1. **Add CNAME file:**
   ```bash
   echo "legal.yourdomain.com" > legal-docs/CNAME
   git add legal-docs/CNAME
   git commit -m "Add custom domain"
   git push
   ```

2. **Configure DNS:**
   - Add a CNAME record in your domain provider:
     - Name: `legal` (or `www.legal`)
     - Value: `YOUR_USERNAME.github.io`

3. **Update GitHub Pages settings:**
   - Go to Settings → Pages
   - Enter your custom domain
   - GitHub will provide SSL certificate automatically

## Testing Locally

Before deploying, test locally:

```bash
# Using Python (if installed)
cd legal-docs
python -m http.server 8000

# Or using Node.js http-server
npx http-server legal-docs -p 8000
```

Then visit: `http://localhost:8000`

## Updating Documents

When you need to update the legal documents:

1. Edit the markdown files in the main repo (`PRIVACY_POLICY.md`, `TERMS_OF_SERVICE.md`)
2. Run the conversion script:
   ```bash
   node legal-docs/convert.js
   ```
3. Commit and push:
   ```bash
   cd legal-docs
   git add .
   git commit -m "Update legal documents"
   git push
   ```

GitHub Pages will automatically update within a few minutes.

## Advantages of GitHub Pages

✅ **Free** - No cost  
✅ **Reliable** - 99.9% uptime  
✅ **HTTPS** - Automatic SSL certificates  
✅ **Version Control** - Track changes to legal docs  
✅ **Easy Updates** - Just push changes  
✅ **Professional** - Clean URLs  
✅ **Fast** - CDN-backed  

## Next Steps

After deployment:

1. ✅ Test the URLs work
2. ✅ Update App Store Connect with Privacy Policy URL
3. ✅ Update Google Play Console with Privacy Policy URL
4. ✅ Add URLs to your app's settings/about screen (optional)

---

**Need help?** Check GitHub Pages documentation: https://docs.github.com/en/pages

