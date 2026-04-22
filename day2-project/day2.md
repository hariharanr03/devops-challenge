# 📅 Day 2 – DevOps Challenge (GitHub Integration & Remote Workflow)

## 🎯 Objective

Understand and implement Git remote workflow by connecting local repository to GitHub and pushing code.

---

## ⚙️ Environment Used

* Ubuntu (VMware)
* Git (installed and configured)
* GitHub account

---

## 🌐 GitHub Setup

* Created a new repository named: `devops-challenge`
* Repository visibility: Public
* No README file added during creation

---

## 🔗 Git Remote Configuration

* Connected local repository to GitHub using:

  * `git remote add origin https://github.com/hariharanr03/devops-challenge.git`

* Verified remote connection:

  * `git remote -v`

---

## 🔄 Git Workflow Practiced

### Initial Push

* Renamed branch to main:

  * `git branch -M main`

* Pushed local code to GitHub:

  * `git push -u origin main`

* Used Personal Access Token (PAT) for authentication

---

### Updating Existing Code

* Modified file:

  * Added new content to `app.txt`

* Tracked changes:

  * `git add .`

* Committed changes:

  * `git commit -m "Day 2 update"`

* Pushed updates:

  * `git push`

---

## ⚠️ Issues Faced & Fixes

### Issue 1: Authentication Error

* Error: Password authentication not supported
* Fix: Used GitHub Personal Access Token instead of password

### Issue 2: No Remote Configured

* Error: `fatal: No configured push destination`
* Fix: Added remote using `git remote add origin <repo-url>`

---

## 🧠 Key Learnings

* Difference between local and remote repositories
* Importance of GitHub in DevOps workflow
* Authentication using Personal Access Token
* Complete Git workflow: add → commit → push

---

## ✅ Outcome

* Successfully connected local repository to GitHub
* Pushed project files to remote repository
* Performed multiple commits and updates
* Understood real-world Git workflow

---

## 🚀 Next Step

Learn Git branching and collaboration workflow (Day 3)

