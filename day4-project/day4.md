# 📅 Day 4 – DevOps Challenge (Pull Requests, Multi-Branch Workflow & Conflict Resolution)

## 🎯 Objective

Implement real-world Git workflow including multiple feature branches, Pull Requests (PR), merging, and handling merge conflicts using both local Git and GitHub.

---

## ⚙️ Environment Used

* Ubuntu (VMware)
* Git (local repository)
* GitHub repository: `devops-challenge`

---

## 🌿 Branching & Parallel Development

* Created multiple feature branches to simulate team development:

  * `feature-login`
  * `feature-dashboard`
  * `feature-A`
  * `feature-B`

* Each branch represents independent work similar to multiple developers working in parallel.

---

## 💻 Feature Development

### Feature 1: Login

* Created branch: `feature-login`
* Added file: `login.txt`
* Committed changes:

  * `git commit -m "Added login feature"`
* Pushed branch to GitHub

---

### Feature 2: Dashboard

* Created branch: `feature-dashboard`
* Added file: `dashboard.txt`
* Committed changes:

  * `git commit -m "Added dashboard feature"`
* Pushed branch to GitHub

---

## 🔀 Pull Request & Merge Workflow

### PR 1: feature-login → main

* Created Pull Request
* Reviewed changes
* Successfully merged into main

---

### PR 2: feature-dashboard → main

* Created Pull Request after merging feature-login
* Successfully merged into main

---

## 💣 Merge Conflict Simulation

To simulate real-world conflicts:

* Created two branches modifying the same file:

  * `feature-A`
  * `feature-B`

* File used: `conflict.txt`

---

## ⚠️ Conflict Scenario 1 (feature-A → main)

* Modified same file differently
* Created PR: `feature-A` → `main`
* GitHub showed:

  * “Can’t automatically merge”

### Resolution:

* Used GitHub UI → Resolve conflicts
* Selected: **Accept Both Changes**

### Output after merge:

Feature A line
Original line

---

## ⚠️ Conflict Scenario 2 (feature-B → main)

* Created PR: `feature-B` → `main`
* Again encountered merge conflict

### Resolution:

* Used GitHub UI → Resolve conflicts
* Selected: **Accept Both Changes**

### Final Output:

Feature B line

Feature A line
Original line

---

## 🔧 Conflict Resolution Understanding

* Learned conflict markers:

  * `<<<<<<< HEAD`
  * `=======`
  * `>>>>>>> branch-name`

* Learned resolution options:

  * Accept Current Change (main branch)
  * Accept Incoming Change (feature branch)
  * Accept Both Changes

* Understood that conflicts occur when:

  * Same file + same line + different changes

---

## 🧠 Key Learnings

* Real-world development involves multiple branches
* Pull Requests are used for controlled merging
* GitHub can auto-merge only when no conflicts exist
* Merge conflicts are normal and expected in team environments
* Conflict resolution requires understanding of code changes
* Git workflow:

  * feature → commit → push → PR → merge → resolve conflicts

---

## ✅ Outcome

* Successfully created and managed multiple branches
* Simulated parallel development workflow
* Created and merged multiple Pull Requests
* Experienced and resolved merge conflicts (twice)
* Understood real-world Git collaboration process

---

## 🚀 Next Step

Learn CI/CD pipeline basics using GitHub Actions (Day 5)
