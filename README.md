# YourBuddy Legal Documents

> Publicly hosted legal documents for the YourBuddy mobile application

This repository contains the Privacy Policy and Terms of Service for [YourBuddy](https://github.com/BrappyTunes/Buddy) - an AI-powered life planner app for journaling, goal tracking, and personal growth.

## 📄 Live Documents

These documents are hosted on GitHub Pages and are publicly accessible:

- **[Privacy Policy](https://brappytunes.github.io/yourbuddy-legal/privacy-policy.html)** - How we collect, use, and protect your data
- **[Terms of Service](https://brappytunes.github.io/yourbuddy-legal/terms-of-service.html)** - Terms and conditions for using YourBuddy
- **[Index Page](https://brappytunes.github.io/yourbuddy-legal/)** - Landing page with links to both documents

## 🎯 Purpose

These legal documents are required for:
- ✅ **App Store Submission** (iOS)
- ✅ **Google Play Submission** (Android)
- ✅ **User Transparency** - Users can review our policies
- ✅ **Legal Compliance** - GDPR, CCPA, and other regulations

## 📁 Repository Structure

```
legal-docs/
├── privacy-policy.html      # Privacy Policy (HTML)
├── terms-of-service.html    # Terms of Service (HTML)
├── index.html              # Landing page
├── convert.js              # Markdown to HTML converter
├── README.md               # This file
├── QUICK_START.md          # Quick deployment guide
└── DEPLOYMENT_GUIDE.md     # Detailed deployment instructions
```

## 🚀 Deployment

This repository is automatically deployed via **GitHub Pages**. The documents are live at:

**Base URL:** `https://brappytunes.github.io/yourbuddy-legal/`

### How It Works

1. HTML files are stored in this repository
2. GitHub Pages serves them as static files
3. Automatic HTTPS/SSL certificates
4. Updates deploy automatically on push

## 🔄 Updating Documents

When the legal documents need to be updated:

1. **Edit source files** in the main [YourBuddy repository](https://github.com/BrappyTunes/Buddy):
   - `PRIVACY_POLICY.md`
   - `TERMS_OF_SERVICE.md`

2. **Convert to HTML:**
   ```bash
   node legal-docs/convert.js
   ```

3. **Commit and push:**
   ```bash
   cd legal-docs
   git add .
   git commit -m "Update legal documents - [reason]"
   git push
   ```

4. **GitHub Pages automatically updates** within 1-2 minutes

## 📋 Document Information

- **Effective Date:** December 11, 2025
- **Last Updated:** December 11, 2025
- **Contact:** yourbuddyai.app@gmail.com

## 🔗 Related Links

- **Main App Repository:** [YourBuddy](https://github.com/BrappyTunes/Buddy)
- **App Store Preparation:** See main repo for submission checklist

## 📝 License

These legal documents are specific to YourBuddy and are not open source. All rights reserved.

## 🤝 Support

For questions about these legal documents, please contact:
- **Email:** yourbuddyai.app@gmail.com

---

**Status:** ✅ Live and accessible  
**Hosting:** GitHub Pages  
**Last Deployed:** See commit history
