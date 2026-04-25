Day 3 - Branching practice

# 📅 Day 3 – DevOps Challenge (Git Branching & Workflow)

## 🎯 Objective

Understand and implement Git branching to simulate real-world development workflow without affecting the main codebase.

---

## ⚙️ Environment Used

* Ubuntu (VMware)
* Git (configured)
* GitHub repository: `devops-challenge`

---

## 🌿 Branching Concept

* Learned the importance of branches in Git

* Understood that:

  * `main` branch → stable/production code
  * `feature` branch → development work

* Purpose:

  * To work on new features without breaking the main code

---

## 🔀 Branch Creation

* Checked existing branch:

  * `git branch`

* Created and switched to a new branch:

  * `git checkout -b feature-day3`

* Verified branch switch:

  * `git branch`

---

## 💻 Project Work

* Created a new folder for Day 3:

  * `mkdir day3`

* Created documentation file:

  * `touch day3/DAY3.md`

* Added sample content:

  * `echo "Day 3 - Branching practice" > day3/DAY3.md`

---

## 🔄 Git Workflow Practiced

### Working in Feature Branch

* Added changes:

  * `git add .`

* Committed changes:

  * `git commit -m "Day 3: Practicing Git branching workflow"`

---

### Pushing Feature Branch

* Pushed branch to GitHub:

  * `git push -u origin feature-day3`

---

## 🧠 Key Learnings

* Importance of branching in collaborative development
* Difference between main branch and feature branch
* Safe development without impacting production code
* Real-world workflow: feature → commit → push

---

## ✅ Outcome

* Successfully created and worked in a new branch
* Added and committed new changes in feature branch
* Pushed feature branch to GitHub
* Understood how teams isolate work using branches

---

## 🚀 Next Step

Learn merging branches and Pull Requests to integrate changes into the main branch (Day 4)

