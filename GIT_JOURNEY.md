# 🧩 My Git Mastery Challenge Journey

## 👨‍💻 Student Information
- **Name:** Siva Sai Prasanna Rameswari Bojja  
- **Student ID:** 23a91a05e5  
- **Repository:** [https://github.com/prasannnna/git-solved-23a91a05e5](https://github.com/prasannnna/git-solved-23a91a05e5)  
- **Date Started:** October 27, 2025  
- **Date Completed:** October 27, 2025  

---

## 🧾 Task Summary
Cloned the instructor’s repository containing multiple pre-built conflicts and successfully resolved all merge conflicts across **main**, **dev**, and **conflict-simulator** branches using proper Git workflows.  
Practiced advanced Git operations such as **cherry-pick**, **revert**, **reset**, and **reflog recovery**.

---

## ⚙️ Commands Used

| Command | Times Used | Purpose |
|----------|-------------|----------|
| `git clone` | 1 | Clone instructor’s repository |
| `git checkout` | 25+ | Switch between branches |
| `git branch` | 10+ | View and manage branches |
| `git merge` | 3 | Merge `dev` and `conflict-simulator` into `main` |
| `git add` | 35+ | Stage resolved conflicts |
| `git commit` | 18+ | Commit resolved and merged changes |
| `git push` | 12+ | Push local changes to GitHub |
| `git fetch` | 2 | Fetch updates from instructor repo |
| `git pull` | 1 | Pull remote updates |
| `git stash` | 2 | Temporarily save uncommitted work |
| `git cherry-pick` | 1 | Copy specific commit (`02011a5`) |
| `git rebase` | 1 | Rebase feature branch onto main |
| `git reset` | 3 | Undo commits (soft/mixed/hard) |
| `git revert` | 1 | Safely undo a bad commit |
| `git reflog` | 2 | Recover lost commit references |
| `git tag` | 2 | Create version tags |
| `git status` | 60+ | Check repo state |
| `git log` | 30+ | View commit history |
| `git diff` | 25+ | Compare code changes |

---

## ⚔️ Conflicts Resolved

### 🧩 Merge 1: `main` + `dev` (6 files)

#### 1️⃣ config/app-config.yaml
- **Issue:** Production used port 8080, development used 3000  
- **Resolution:** Unified config using environment variable `APP_ENV`  
- **Strategy:** Default = production, dev optional  
- **Difficulty:** Medium  
- **Time:** 15 minutes  

#### 2️⃣ config/database-config.json
- **Issue:** Different DB hosts and SSL configs  
- **Resolution:** Added “profiles” for production and development  
- **Strategy:** Maintained production as default  
- **Difficulty:** Medium  
- **Time:** 10 minutes  

#### 3️⃣ scripts/deploy.sh
- **Issue:** Completely different deployment logic  
- **Resolution:** Added `DEPLOY_ENV` flag for conditional deployment  
- **Strategy:** Unified both strategies dynamically  
- **Difficulty:** Hard  
- **Time:** 20 minutes  

#### 4️⃣ scripts/monitor.js
- **Issue:** Different logging intervals and monitoring logic  
- **Resolution:** Used `process.env.NODE_ENV` to switch configs  
- **Difficulty:** Medium  
- **Time:** 15 minutes  

#### 5️⃣ docs/architecture.md
- **Issue:** Overlapping architectural explanations  
- **Resolution:** Merged both into one comprehensive document  
- **Difficulty:** Easy  
- **Time:** 10 minutes  

#### 6️⃣ README.md
- **Issue:** Different feature lists and setup instructions  
- **Resolution:** Combined both with proper formatting and clarity  
- **Difficulty:** Easy  
- **Time:** 10 minutes  

---

### 🧩 Merge 2: `main` + `conflict-simulator` (6 files)

| File | Issue | Resolution | Difficulty | Time |
|------|--------|-------------|-------------|------|
| `scripts/deploy.sh` | Merge simulation conflicts | Manually merged and validated logic | Medium | 15 min |
| `README.md` | Duplicate information | Unified and formatted cleanly | Easy | 10 min |
| `config/app-config.yaml` | Conflicting settings | Reused unified environment-based config | Medium | 10 min |
| `scripts/test.sh` | Different testing commands | Combined as environment-based | Medium | 15 min |
| `logs/README.md` | Missing section | Re-added with proper formatting | Easy | 5 min |
| `package.json` | Version mismatch | Kept updated version with all dependencies | Medium | 10 min |

---

## 💡 Most Challenging Parts

1. **Handling Multiple Conflicts** — Managing the same files across multiple branches required patience.  
2. **Understanding Merge Markers** — Learned how `<<<<<<<`, `=======`, and `>>>>>>>` indicate branch conflicts.  
3. **Recovering Lost Commits** — Used `git reflog` and `git cherry-pick` to restore lost changes after a reset.  
4. **Push Errors** — Faced “fetch first” issues; fixed using `git pull --rebase` and `git push --force`.  
5. **Bad Commit Practice** — Created a deliberate bug and reverted using `git revert HEAD`.  

---

## 🚀 Key Learnings

### 🧠 Technical Skills
- Confidently resolve merge conflicts  
- Practiced `revert`, `rebase`, `cherry-pick`, and `reset`  
- Understood recovery using `reflog`  
- Learned difference between **merge** and **rebase**

### 🧩 Best Practices
- Always check `git status` and `git diff`  
- Commit small, clear changes  
- Test before committing after conflict resolution  
- Write meaningful commit messages  
- Don’t panic — `git reflog` saves the day 😄  

### 🔁 Workflow Insights
- Conflicts are normal during collaboration  
- Always understand both code versions before merging  
- Keep your main branch stable  
- Rebase helps maintain a clean history  

---

## 🪶 Reflection
This Git Mastery Challenge gave me real experience with resolving conflicts, merging branches, and fixing mistakes safely.  
I learned that **conflicts aren’t errors — they’re opportunities to understand code better**.  

I can now confidently handle merges, resolve conflicts, and use advanced Git tools like `revert`, `reset`, and `cherry-pick` without fear.  
This challenge made me ready for real-world collaborative development.

---

