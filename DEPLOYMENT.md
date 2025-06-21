# 🚀 Website Deployment Guide

This guide will walk you through deploying Erum Hassan's website to various platforms.

## Option 1: GitHub Pages (Recommended - Free)

### Step 1: Create GitHub Repository
1. Go to [GitHub.com](https://github.com) and sign in
2. Click the "+" icon in the top right → "New repository"
3. Name it: `erum-hassan-website` or `personal-website`
4. Make it **Public** (required for free GitHub Pages)
5. Don't initialize with README (we already have one)
6. Click "Create repository"

### Step 2: Upload Files to GitHub
```bash
# Add all files to git
git add .

# Commit the files
git commit -m "Initial website commit"

# Add your GitHub repository as remote (replace YOUR_USERNAME and REPO_NAME)
git remote add origin https://github.com/YOUR_USERNAME/REPO_NAME.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click "Settings" tab
3. Scroll down to "Pages" section (left sidebar)
4. Under "Source", select "Deploy from a branch"
5. Choose "main" branch and "/ (root)" folder
6. Click "Save"
7. Wait 2-5 minutes for deployment

Your website will be available at: `https://YOUR_USERNAME.github.io/REPO_NAME`

---

## Option 2: Netlify (Free & Drag & Drop)

### Method A: Drag & Drop (Easiest)
1. Go to [Netlify.com](https://netlify.com) and sign up
2. Drag your entire `ErumCV` folder to the Netlify dashboard
3. Wait for deployment (usually 30 seconds)
4. Your site is live! Netlify gives you a random URL like `https://amazing-site-123.netlify.app`

### Method B: Connect to GitHub
1. Sign up for Netlify
2. Click "New site from Git"
3. Connect your GitHub account
4. Select your repository
5. Deploy settings: Build command (leave empty), Publish directory: `/`
6. Click "Deploy site"

---

## Option 3: Vercel (Free & Fast)

1. Go to [Vercel.com](https://vercel.com) and sign up
2. Click "New Project"
3. Import your GitHub repository
4. Vercel auto-detects it's a static site
5. Click "Deploy"
6. Your site is live in seconds!

---

## Option 4: Custom Domain (Optional)

### Step 1: Buy a Domain
- [Namecheap.com](https://namecheap.com) - Good prices
- [GoDaddy.com](https://godaddy.com) - Popular
- [Google Domains](https://domains.google) - Simple

### Step 2: Configure DNS
For GitHub Pages:
1. Go to repository Settings → Pages
2. Add your custom domain
3. Update your domain's DNS settings:
   - Add CNAME record: `YOUR_USERNAME.github.io`
   - Or A records pointing to GitHub's IPs

For Netlify/Vercel:
1. Add custom domain in their dashboard
2. Update DNS as instructed by the platform

---

## Option 5: Local Testing

Before deploying, test locally:

```bash
# Using Python (if installed)
python -m http.server 8000

# Using Node.js
npx http-server

# Using PHP
php -S localhost:8000
```

Then visit `http://localhost:8000`

---

## 🎯 Recommended Deployment Path

**For Erum's website, I recommend:**

1. **Start with GitHub Pages** (free, professional, easy to update)
2. **Add a custom domain** later if desired
3. **Consider Netlify** if you want more features

### Quick GitHub Pages Setup:

```bash
# Run these commands in your terminal:
git add .
git commit -m "Initial website commit"
# Then follow the GitHub repository creation steps above
```

---

## 📊 Post-Deployment Checklist

After deploying, make sure to:

- [ ] Test all links work
- [ ] Check mobile responsiveness
- [ ] Test contact form (if backend is set up)
- [ ] Add Google Analytics (optional)
- [ ] Set up Google Search Console
- [ ] Test loading speed
- [ ] Share the URL with Erum

---

## 🔧 Troubleshooting

### Common Issues:

**GitHub Pages not working:**
- Make sure repository is public
- Check if files are in the main branch
- Wait 5-10 minutes for first deployment

**Images not loading:**
- Check file paths are correct
- Ensure images are committed to repository

**Styling issues:**
- Clear browser cache
- Check CSS file is properly linked

**Mobile menu not working:**
- Test on actual mobile device
- Check JavaScript console for errors

---

## 📈 Analytics Setup (Optional)

### Google Analytics:
1. Go to [Google Analytics](https://analytics.google.com)
2. Create account and property
3. Get tracking code
4. Add to `<head>` section of `index.html`

### Google Search Console:
1. Go to [Search Console](https://search.google.com/search-console)
2. Add your domain
3. Verify ownership
4. Submit sitemap

---

## 🎉 Success!

Once deployed, Erum will have a professional online presence showcasing her:
- Chemical Engineering expertise
- Research achievements
- Professional experience
- Awards and recognition
- Contact information

The website will be accessible worldwide and help her stand out in job applications and networking opportunities! 