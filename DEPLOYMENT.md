# Deployment Guide - دليل النشر

## GitHub Pages Deployment

### Step-by-Step Instructions

#### 1. Create GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the "+" icon → "New repository"
3. Name your repository (e.g., `ksar-el-boukhari`)
4. Choose "Public" visibility
5. Don't initialize with README (we already have one)
6. Click "Create repository"

#### 2. Upload Your Code

**Option A: Using Git Command Line**

```bash
# Navigate to your project folder
cd "c:\Users\youba\Downloads\ksar-el-boukhari-app"

# Initialize Git repository
git init

# Add all files
git add .

# Commit files
git commit -m "Initial commit: Ksar El-Boukhari Province website"

# Add remote repository (replace with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/ksar-el-boukhari.git

# Rename branch to main
git branch -M main

# Push to GitHub
git push -u origin main
```

**Option B: Using GitHub Desktop**

1. Download and install [GitHub Desktop](https://desktop.github.com/)
2. Open GitHub Desktop
3. File → Add Local Repository → Choose your folder
4. Click "Publish repository"
5. Choose repository name and click "Publish"

**Option C: Direct Upload**

1. Go to your new repository on GitHub
2. Click "uploading an existing file"
3. Drag and drop all files from your folder
4. Click "Commit changes"

#### 3. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" tab
3. Scroll down and click "Pages" in the left sidebar
4. Under "Source", select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click "Save"
6. Wait 1-2 minutes
7. Your site will be live at: `https://YOUR_USERNAME.github.io/ksar-el-boukhari/`

### Updating Your Website

Whenever you make changes:

```bash
git add .
git commit -m "Description of changes"
git push
```

Changes will be live in 1-2 minutes!

---

## Alternative Deployment Options

### 1. Netlify (Easiest)

1. Go to [Netlify](https://www.netlify.com/)
2. Sign up for free
3. Drag and drop your folder
4. Done! Get instant URL like `your-site.netlify.app`

**Update process**: Just drag & drop again!

### 2. Vercel

1. Go to [Vercel](https://vercel.com/)
2. Sign up with GitHub
3. Import your repository
4. Deploy automatically
5. Get URL like `your-site.vercel.app`

**Update process**: Automatic on every git push!

### 3. Cloudflare Pages

1. Go to [Cloudflare Pages](https://pages.cloudflare.com/)
2. Sign up for free
3. Connect GitHub repository
4. Deploy
5. Get fast CDN-powered hosting

### 4. Firebase Hosting

```bash
# Install Firebase CLI
npm install -g firebase-tools

# Login to Firebase
firebase login

# Initialize project
firebase init hosting

# Deploy
firebase deploy
```

### 5. Any Web Hosting

Just upload these files via FTP:
- `index.html`
- All other files in the folder

---

## Custom Domain Setup

### For GitHub Pages:

1. Buy domain from namecheap, godaddy, etc.
2. In your domain's DNS settings, add:
   - Type: `A` Record
   - Host: `@`
   - Value: GitHub IPs:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - Type: `CNAME`
   - Host: `www`
   - Value: `YOUR_USERNAME.github.io`

3. In GitHub repo Settings → Pages:
   - Add custom domain
   - Enable "Enforce HTTPS"

---

## Performance Optimization

### Optional Improvements:

1. **Minify CSS/JS**: Use [minifier](https://www.minifier.org/)
2. **Compress Images**: If you add images, use [TinyPNG](https://tinypng.com/)
3. **Enable Caching**: Automatic on GitHub Pages
4. **CDN**: Automatic on Netlify/Vercel

---

## Monitoring & Analytics

### Add Google Analytics:

Add before `</head>` in index.html:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=YOUR_GA_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'YOUR_GA_ID');
</script>
```

---

## Troubleshooting

### Site not loading?
- Wait 2-3 minutes after deployment
- Check GitHub Pages settings
- Ensure repository is public

### Styles not working?
- Clear browser cache (Ctrl+F5)
- Check browser console for errors

### Map not showing?
- Check internet connection
- Leaflet CDN might be loading slowly

---

## Support

For issues or questions:
- Open an issue on GitHub
- Check [GitHub Pages documentation](https://docs.github.com/pages)
- Visit [Stack Overflow](https://stackoverflow.com/)

---

**Ready to deploy?** Follow the GitHub Pages instructions above! 🚀
