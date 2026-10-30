# Portfolio Deployment Guide (Lecture 13 & 15)

This guide documents the exact Git commands, security checks, and Vercel deployment steps used for the Portfolio project.

---

## Part 1: Git Repository Setup & Initial Commit (Lecture 13)
Inside the `portfolio/` directory:
```bash
# 1. Initialize git repository
git init

# 2. Check initial untracked files
git status

# 3. Stage all project files
git add .

# 4. Create initial commit
git commit -m "Initial portfolio commit"

# 5. Connect to GitHub remote and set main branch
git branch -M main
git remote add origin https://github.com/krishnagupta/portfolio.git
git push -u origin main
```

---

## Part 2: Vercel Deployment Workflow (Lecture 13)
1. Sign in to [Vercel](https://vercel.com) using GitHub account.
2. Click **New Project** -> **Import Git Repository**.
3. Locate `portfolio` and click **Import**.
4. Keep default framework preset (`Other`) and root directory as `./`.
5. Click **Deploy**.
6. Deployment builds immediately and provides production URL: `https://krishnagupta-portfolio.vercel.app`.

---

## Part 3: Secure Chatbot Deployment (Lecture 15)
When adding Groq Chatbot:
1. Verify `config.js` is ignored by Git to avoid leaking API credentials:
   ```bash
   git status
   git check-ignore config.js
   ```
2. Commit and push only safe files:
   ```bash
   git add index.html chatbot.css chatbot.js .gitignore
   git status
   git commit -m "Add portfolio chatbot interface"
   git push origin main
   ```
3. Vercel automatically redeploys from the latest commit on `main`.
