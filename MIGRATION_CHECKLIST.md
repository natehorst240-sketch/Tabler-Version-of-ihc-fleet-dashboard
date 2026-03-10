# ✅ GitHub Migration Checklist

Print this page and check off each step as you complete it!

---

## 📋 Pre-Migration

- [ ] Download the `github-migration-package` folder
- [ ] Extract/unzip if needed
- [ ] Have GitHub account ready (create at github.com if needed)
- [ ] Have Git installed (optional, can do everything via web)

---

## 🚀 Step 1: Create Repository (5 minutes)

- [ ] Go to github.com and log in
- [ ] Click `+` icon → New repository
- [ ] Name: `ihc-fleet-dashboard`
- [ ] Set to **Private** ✓
- [ ] ✓ Add a README file
- [ ] Click "Create repository"
- [ ] Repository created ✓

---

## 📤 Step 2: Upload Files (5 minutes)

**Option A: Web Upload (Easier)**
- [ ] In your repo, click "uploading an existing file"
- [ ] Drag entire contents of `github-migration-package` folder
- [ ] Make sure `.github` folder is included!
- [ ] Commit message: "Initial setup"
- [ ] Click "Commit changes"
- [ ] All files uploaded ✓

**Option B: Command Line**
```bash
cd github-migration-package
git init
git add .
git commit -m "Initial setup"
git remote add origin https://github.com/YOUR_USERNAME/ihc-fleet-dashboard.git
git branch -M main
git push -u origin main
```
- [ ] Files pushed to GitHub ✓

---

## ⚙️ Step 3: Configure GitHub (5 minutes)

### Enable GitHub Pages:
- [ ] Go to Settings (top menu)
- [ ] Click "Pages" (left sidebar)
- [ ] Source: **GitHub Actions**
- [ ] Click Save
- [ ] Pages enabled ✓

### Add Secrets (if using SkyRouter API):
- [ ] Settings → Secrets and variables → Actions
- [ ] Click "New repository secret"
- [ ] Name: `SKYROUTER_USER`, Value: [your username]
- [ ] Click "Add secret"
- [ ] Click "New repository secret" again
- [ ] Name: `SKYROUTER_PASS`, Value: [your password]
- [ ] Click "Add secret"
- [ ] Secrets configured ✓

---

## 🧪 Step 4: Test Setup (10 minutes)

### Create Test Data:
- [ ] Navigate to `data/` folder in your repo
- [ ] Click "Add file" → "Create new file"
- [ ] Name it: `test.txt`
- [ ] Content: "test"
- [ ] Commit
- [ ] Check Actions tab → workflow should run
- [ ] Workflow completed successfully ✓

### Or run locally:
```bash
cd ihc-fleet-dashboard
./quick-start.sh
```
- [ ] Test data created ✓
- [ ] Dashboard generated ✓
- [ ] Files committed ✓

### Verify Deployment:
- [ ] Wait 2-3 minutes
- [ ] Visit: `https://YOUR_USERNAME.github.io/ihc-fleet-dashboard/`
- [ ] Dashboard loads! ✓

---

## 📊 Step 5: Upload Real Data (5 minutes)

- [ ] Go to `data/` folder in repo
- [ ] Click "Add file" → "Upload files"
- [ ] Upload `Due-List_Latest.csv`
- [ ] Upload `Due-List_BIG_WEEKLY.csv`
- [ ] Commit changes
- [ ] CSV files uploaded ✓
- [ ] Check Actions tab
- [ ] Workflow runs automatically ✓
- [ ] Wait 2 minutes
- [ ] Refresh dashboard URL
- [ ] Real data showing! ✓

---

## 🔄 Step 6: Set Up Regular Updates

### Automated (Recommended):
- [ ] Workflows are already scheduled (8 AM UTC daily)
- [ ] SkyRouter credentials configured (if applicable)
- [ ] Nothing else needed! ✓

### Manual:
- [ ] Bookmark: Actions → Update Fleet Dashboard
- [ ] Run when you upload new CSV files
- [ ] Manual trigger tested ✓

---

## 👥 Step 7: Share with Team (Optional)

- [ ] Settings → Collaborators → Add people
- [ ] Add team members' GitHub usernames
- [ ] Share dashboard URL: `https://YOUR_USERNAME.github.io/ihc-fleet-dashboard/`
- [ ] Create usage guide (or share SETUP_GUIDE.md)
- [ ] Team has access ✓

---

## 🎯 Post-Setup Verification

- [ ] Dashboard accessible via URL
- [ ] All three tabs working (Maintenance, Flight Hours, Bases)
- [ ] Data is current
- [ ] Automated workflow scheduled
- [ ] Team can access
- [ ] Mobile view works
- [ ] Bookmarked dashboard URL

---

## 📝 Notes / Issues Encountered

Write any problems you ran into and how you solved them:

```
_______________________________________________________________

_______________________________________________________________

_______________________________________________________________

_______________________________________________________________

_______________________________________________________________
```

---

## 🎉 Migration Complete!

**Dashboard URL:** ____________________________________

**Last Updated:** ____________________________________

**Next CSV Upload:** ____________________________________

**Team Members with Access:**
- [ ] ____________________________________
- [ ] ____________________________________
- [ ] ____________________________________

---

## 📞 Quick Reference

| Need | Location |
|------|----------|
| Upload CSV | Repo → data/ folder → Upload files |
| Manual trigger | Actions → Update Fleet Dashboard → Run workflow |
| Check logs | Actions → Click workflow run |
| Add team | Settings → Collaborators |
| Edit scripts | scripts/ folder → Edit file |
| Dashboard URL | https://YOUR_USERNAME.github.io/ihc-fleet-dashboard/ |

---

**Keep this checklist for future reference!**

**Helpful docs:**
- `SETUP_GUIDE.md` - Complete instructions
- `QUICK_REFERENCE.md` - Quick tips
- `README.md` - Project overview
