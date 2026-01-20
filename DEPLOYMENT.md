# GitHub Setup and Deployment Guide

Follow these steps to create and deploy your website to GitHub Pages.

## Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the **+** icon in the top right corner
3. Select **New repository**
4. Fill in the repository details:
   - **Repository name**: `interactive-llm-verification` (or your preferred name)
   - **Description**: "Official website for 'Improving Human Verification of LLM Reasoning through Interactive Explanation Interfaces'"
   - **Visibility**: Public
   - **DO NOT** initialize with README, .gitignore, or license (we already have these)
5. Click **Create repository**

## Step 2: Upload Your Files

### Option A: Using GitHub Web Interface (Easiest)

1. On your new repository page, click **uploading an existing file**
2. Drag and drop these files:
   - `index.html`
   - `README.md`
   - `LICENSE`
   - `.gitignore`
3. Write a commit message: "Initial commit: Add website files"
4. Click **Commit changes**

### Option B: Using Git Command Line

```bash
# Navigate to the directory containing your files
cd /path/to/your/files

# Initialize git repository
git init

# Add all files
git add index.html README.md LICENSE .gitignore

# Commit the files
git commit -m "Initial commit: Add website files"

# Add your GitHub repository as remote (replace YOUR-USERNAME)
git remote add origin https://github.com/YOUR-USERNAME/interactive-llm-verification.git

# Push to GitHub
git branch -M main
git push -u origin main
```

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (top menu)
3. In the left sidebar, click **Pages**
4. Under **Build and deployment**:
   - **Source**: Select "Deploy from a branch"
   - **Branch**: Select "main"
   - **Folder**: Select "/ (root)"
5. Click **Save**
6. Wait 1-2 minutes for deployment

Your site will be live at:
```
https://YOUR-USERNAME.github.io/interactive-llm-verification/
```

## Step 4: Update URLs in Files

Once your site is live, update the placeholder URLs:

### In `README.md`:
Replace:
```
https://your-username.github.io/interactive-llm-verification/
```
With:
```
https://YOUR-ACTUAL-USERNAME.github.io/interactive-llm-verification/
```

### In `index.html`:
Replace the GitHub link:
```html
<a href="https://github.com/yourusername/interactive-llm-verification" ...>
```
With:
```html
<a href="https://github.com/YOUR-ACTUAL-USERNAME/interactive-llm-verification" ...>
```

And the HuggingFace link (if you have one):
```html
<a href="https://huggingface.co/spaces/your-space" ...>
```

Commit and push these changes:
```bash
git add README.md index.html
git commit -m "Update URLs with actual username"
git push
```

## Step 5: Verify Deployment

1. Visit your site: `https://YOUR-USERNAME.github.io/interactive-llm-verification/`
2. Test all interactive features:
   - Hover cards (iCoT, iPoT, iGraph)
   - Interactive iGraph demo (Previous/Next buttons)
   - All links in the footer
3. Check on mobile devices for responsiveness

## Optional: Custom Domain

If you want to use a custom domain (e.g., `interactive-llm.yoursite.com`):

1. In your repository's **Settings** → **Pages**
2. Under **Custom domain**, enter your domain
3. Click **Save**
4. In your domain registrar's DNS settings, add:
   - Type: `CNAME`
   - Name: `interactive-llm` (or your subdomain)
   - Value: `YOUR-USERNAME.github.io`
5. Wait for DNS propagation (can take up to 24 hours)

## Troubleshooting

### Site not loading?
- Wait 2-3 minutes after enabling GitHub Pages
- Check that `index.html` is in the root directory
- Verify branch is set to "main" in Pages settings

### 404 Error?
- Make sure the repository is public
- Check that the file is named exactly `index.html` (lowercase)
- Clear your browser cache

### Links not working?
- Update all placeholder URLs in `index.html`
- Ensure GitHub username is correct in all links

### Need to make changes?
```bash
# Make your edits to index.html or other files
git add .
git commit -m "Update: description of changes"
git push
```
Changes will appear on your live site within 1-2 minutes.

## Need Help?

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Pages Troubleshooting](https://docs.github.com/en/pages/getting-started-with-github-pages/troubleshooting-404-errors-for-github-pages-sites)
- Open an issue in your repository if you encounter problems

---

**Congratulations!** Your website is now live and accessible to the world! 🎉
