# 🚀 Deploy to GitHub Pages - Step by Step

This guide shows you exactly how to get your Arcade Zone website live on GitHub Pages.

## Prerequisites

- GitHub account (free at github.com)
- Git installed on your computer
- Your Arcade Zone files ready

## Method 1: Deploy Using GitHub Pages (Easiest)

### Step 1: Create a New Repository on GitHub

1. Go to [github.com](https://github.com) and sign in
2. Click the **+** icon in top right → **New repository**
3. Name your repository one of these:
   - `yourusername.github.io` (for a user/organization site) → **Most Popular**
   - `Arcade` (for a project site)
4. Choose **Public** (so it's visible to everyone)
5. Click **Create repository**

### Step 2: Push Your Code to GitHub

Open PowerShell in your `Arcade` folder and run:

```powershell
# Initialize git
git init

# Add all files
git add .

# Create initial commit
git commit -m "Initial commit: Arcade Zone retro gaming website"

# Add remote repository (replace YOUR_USERNAME and REPO_NAME)
git remote add origin https://github.com/YOUR_USERNAME/REPO_NAME.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (top right)
3. Click **Pages** (left sidebar, under "Code and automation")
4. Under "Build and deployment":
   - **Source**: Select `Deploy from a branch`
   - **Branch**: Select `main` and folder `/root`
   - Click **Save**

### Step 4: Visit Your Site!

- If you used `yourusername.github.io` → Visit `https://yourusername.github.io`
- If you used `Arcade` → Visit `https://yourusername.github.io/Arcade`

✅ **Done! Your arcade website is live!**

---

## Method 2: Using GitHub CLI (Alternative)

If you have GitHub CLI installed:

```powershell
# Login to GitHub
gh auth login

# Create new repository and push
gh repo create Arcade --public --source=. --remote=origin --push
```

Then follow **Step 3** above to enable Pages.

---

## Method 3: Update Your Site

After you make changes locally:

```powershell
# Add your changes
git add .

# Commit with a message
git commit -m "Update: Added new features"

# Push to GitHub
git push origin main
```

Your site updates automatically within seconds!

---

## Tips & Tricks

### Custom Domain
Want to use your own domain instead of `github.io`?

1. Buy a domain (namecheap.com, godaddy.com, etc.)
2. Go to your repo **Settings → Pages**
3. Under "Custom domain", enter your domain
4. Configure DNS at your domain provider (they have instructions)

### Add a Favicon
1. Create a 32×32 icon file named `favicon.ico`
2. Add to your repository root
3. Add this to `index.html` `<head>`:
```html
<link rel="icon" type="image/x-icon" href="favicon.ico">
```

### Faster Loading
Your site is already optimized! But you can:
- Minimize `index.html` if needed (though it works fine as-is)
- Use a CDN for images (already using Google Fonts CDN)

### Track Visitors (Optional)
Add Google Analytics, Vercel Analytics, or GitHub Insights (all free).

---

## Troubleshooting

**"Repository not found"?**
- Make sure you pushed to the correct repository
- Check that the repository name matches in the git remote command

**"Website showing 404"?**
- Wait 1-2 minutes for GitHub Pages to deploy
- Go to Settings → Pages and check "Actions" tab for deployment status
- Clear browser cache (Ctrl+Shift+Delete)

**Changes not showing?**
- Hard refresh browser (Ctrl+F5)
- Wait up to 30 seconds for GitHub Pages to update
- Check Actions tab to see if build succeeded

**Custom domain not working?**
- DNS can take up to 24 hours to propagate
- Double-check your DNS settings match your domain provider's docs

---

## Share Your Arcade!

Once it's live:

- Share the link: `https://yourusername.github.io/Arcade`
- Add to your portfolio
- Tweet it: **"Check out my retro arcade website! 🕹️ Built with vanilla HTML/CSS/JS. No backend needed!"**
- Post on Reddit: r/webdev, r/retrogaming, r/portfolios

---

## Next Steps

- Customize the colors and fonts in `index.html`
- Add more games (edit the `GAMES` object in the script)
- Add your own favicon
- Write a blog post about building it

---

**Questions?** Check the main README.md or open an issue on GitHub!
