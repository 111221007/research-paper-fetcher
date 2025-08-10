# 🚀 Development & Deployment Guide

## Quick Reference for Updating & Deploying Your Research Paper Fetcher

### 📍 Current Setup
- **Local Project**: `/Users/reddy/2025/paper-fetcher-web/`
- **GitHub Repo**: `https://github.com/111221007/research-paper-fetcher`
- **Live Site**: `https://research-paper-fetcher-111221007.vercel.app` (or your custom Vercel URL)

---

## 🔄 Step-by-Step Update & Deploy Process

### Step 1: Navigate to Project Directory
```bash
cd /Users/reddy/2025/paper-fetcher-web
```

### Step 2: Make Your Changes
Edit any files you want to update:
- `index.html` - Main application
- `README.md` - Documentation
- `vercel.json` - Deployment config
- `package.json` - Project metadata

### Step 3: Check What Changed
```bash
git status
```
This shows which files you modified.

### Step 4: Add Changes to Git
```bash
# Add specific files
git add index.html
git add README.md

# OR add all changes at once
git add .
```

### Step 5: Commit Your Changes
```bash
git commit -m "Your descriptive commit message here"

# Examples:
git commit -m "Add new search filters to UI"
git commit -m "Fix mobile responsiveness issue"
git commit -m "Update styling and improve UX"
```

### Step 6: Push to GitHub
```bash
git push
```

### Step 7: Automatic Deployment ⚡
- **Vercel automatically detects** the GitHub push
- **Builds and deploys** your changes (30-60 seconds)
- **Your live site updates** automatically!

### Step 8: Verify Changes Live
Visit your live URL to see the changes:
`https://research-paper-fetcher-knqa.vercel.app/`

---

## 🎯 Quick Commands Reference

### Check Status
```bash
git status                    # See what files changed
git log --oneline -5          # See recent commits
```

### Make Changes Live (All-in-One)
```bash
git add .
git commit -m "Description of changes"
git push
```

### View Live Deployment Status
- Visit: `https://vercel.com/dashboard`
- See real-time build logs and deployment status

---

## 🔧 Common Update Scenarios

### Scenario 1: UI/Design Changes
1. Edit `index.html` (CSS/HTML sections)
2. `git add index.html`
3. `git commit -m "Update UI design"`
4. `git push`
5. Check live site in 30-60 seconds

### Scenario 2: New Features
1. Edit `index.html` (JavaScript sections)
2. Test locally by opening `index.html` in browser
3. `git add index.html`
4. `git commit -m "Add new feature: [feature name] "`
5. `git push`

### Scenario 3: Fix Bugs
1. Identify and fix the issue in `index.html`
2. `git add index.html`
3. `git commit -m "Fix: [bug description]"`
4. `git push`

### Scenario 4: Update Documentation
1. Edit `README.md`
2. `git add README.md`
3. `git commit -m "Update documentation"`
4. `git push`

---

## 🚨 Troubleshooting

### If Vercel Build Fails:
1. Check Vercel dashboard for error logs
2. Common issues:
   - Syntax errors in HTML/JavaScript
   - Invalid `vercel.json` configuration
3. Fix the issue locally
4. Push the fix: `git add . && git commit -m "Fix build error" && git push`

### If Changes Don't Appear:
1. Hard refresh browser: `Cmd + Shift + R` (Mac) / `Ctrl + Shift + R` (Windows)
2. Check Vercel dashboard to confirm deployment completed
3. Try incognito/private browsing mode

### If Git Push Fails:
```bash
git pull                      # Pull any remote changes first
git push                      # Try pushing again
```

---

## ✨ Pro Tips

### 1. Test Locally First
- Open `index.html` in your browser before pushing
- Make sure everything works as expected

### 2. Use Descriptive Commit Messages
- ✅ Good: `"Add year range validation to search form"`
- ❌ Bad: `"update"`

### 3. Check Live Site After Each Push
- Always verify your changes worked as expected
- Test on both desktop and mobile

### 4. Keep Commits Small
- Make frequent, small commits rather than large ones
- Easier to track and rollback if needed

---

## 📱 Mobile Testing

### Test Responsiveness:
1. Open live site on your phone
2. OR use browser dev tools:
   - Press `F12`
   - Click device icon (phone/tablet)
   - Test different screen sizes

---

## 🆘 Emergency Rollback

### If Something Breaks:
```bash
git log --oneline -10         # See recent commits
git revert COMMIT_HASH        # Revert specific commit
git push                      # Deploy the rollback
```

---

## 📞 Quick Help

- **Vercel Dashboard**: https://vercel.com/dashboard
- **GitHub Repo**: https://github.com/111221007/research-paper-fetcher
- **Live Site**: [Your Vercel URL]

---

**💡 Remember**: Every `git push` = Automatic deployment to live site!

**🚀 Typical workflow**: Edit → Test locally → `git add .` → `git commit -m "message"` → `git push` → Check live site
