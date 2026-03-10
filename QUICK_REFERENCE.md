# 🎯 GitHub Migration - Quick Reference Card

## ⚡ 3-Minute Setup

1. **Create repo on GitHub** → Name: `ihc-fleet-dashboard` (Private)
2. **Upload all files** from `github-migration-package` folder
3. **Enable GitHub Pages** → Settings → Pages → Source: GitHub Actions
4. **Done!** Dashboard at: `https://YOUR_USERNAME.github.io/ihc-fleet-dashboard/`

---

## 📥 Daily Workflow

**Upload new CSV:**
1. GitHub → `data/` folder → Upload files
2. Wait 2 minutes
3. Dashboard auto-updates!

---

## 🔐 Add SkyRouter Credentials

Settings → Secrets → Actions → New secret:
- `SKYROUTER_USER` = your username
- `SKYROUTER_PASS` = your password

---

## 🤖 Automation

**Runs automatically:**
- Every day at 8 AM UTC (1 AM MST)
- When you upload CSV files

**Manual trigger:**
- Actions tab → Update Fleet Dashboard → Run workflow

---

## 📂 What Goes Where

```
ihc-fleet-dashboard/
├── data/
│   ├── Due-List_Latest.csv      ← Upload here
│   └── Due-List_BIG_WEEKLY.csv  ← Upload here
├── scripts/                      ← Don't touch
├── public/
│   └── index.html                ← Auto-generated
└── .github/workflows/            ← Auto-runs daily
```

---

## 🐛 Quick Fixes

| Problem | Fix |
|---------|-----|
| Dashboard not updating | Check Actions tab for errors |
| 404 error | Enable GitHub Pages in Settings |
| No data showing | Upload CSV files to data/ folder |
| SkyRouter not working | Add secrets in Settings |

---

## 📖 Full Instructions

**See:** `SETUP_GUIDE.md` (complete step-by-step guide)

---

## ✅ Checklist

- [ ] Create GitHub repository
- [ ] Upload all files
- [ ] Enable GitHub Pages
- [ ] Add SkyRouter secrets (if applicable)
- [ ] Test with sample data
- [ ] Upload real CSV files
- [ ] Verify dashboard loads
- [ ] Share URL with team

---

**Dashboard URL:** `https://YOUR_USERNAME.github.io/ihc-fleet-dashboard/`

**Need help?** Check SETUP_GUIDE.md → Troubleshooting section
