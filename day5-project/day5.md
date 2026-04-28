# 📅 Day 5 – DevOps Challenge (CI/CD with GitHub Actions)

## 🎯 Objective

Understand and implement a basic CI (Continuous Integration) pipeline using GitHub Actions to automate tasks on code push.

---

## ⚙️ Environment Used

* Ubuntu (VMware)
* Git (local repository)
* GitHub repository: `devops-challenge`
* GitHub Actions (CI/CD tool)

---

## 🧠 Introduction to CI/CD

* CI (Continuous Integration):

  * Automatically runs tasks (build/test) when code is pushed

* CD (Continuous Deployment):

  * Automatically deploys application after successful build (not implemented yet)

---

## 📁 Workflow Setup

* Created workflow directory:

  * `.github/workflows/`

* Created pipeline file:

  * `ci.yml`

---

## 🔧 CI Pipeline Configuration

* Trigger:

  * Runs on every push to `main` branch

* Defined a job:

  * Job name: `build`
  * Runner: `ubuntu-latest`

---

## ⚙️ Steps Implemented

### 1. Checkout Code

* Action used:

  * `actions/checkout@v3`
* Purpose:

  * Fetch repository code into the runner

---

### 2. List Files

* Command:

  * `ls -la`
* Purpose:

  * View all files in repository

---

### 3. Show Current Directory

* Command:

  * `pwd`
* Purpose:

  * Display working directory path

---

### 4. Print System Information

* Command:

  * `uname -a`
* Purpose:

  * Display system details of runner

---

### 5. Simulate Build

* Command:

  * `echo "Building application..."`
* Purpose:

  * Mimic build step

---

### 6. Simulate Test

* Command:

  * `echo "Running Test..."`
* Purpose:

  * Mimic testing process

---

### 7. Simulate Success

* Command:

  * `echo "Build and Test Successful"`
* Purpose:

  * Indicate successful pipeline execution

---

## 🔄 Pipeline Execution

* Pushed workflow file to GitHub
* Pipeline triggered automatically
* Verified execution in GitHub Actions tab
* Observed step-by-step logs

---

## 💣 Failure Simulation

* Intentionally modified pipeline:

  * Used `exit 1` to simulate failure

* Observed:

  * Pipeline failed (red status)
  * Execution stopped at failure step

* Reverted changes to restore successful pipeline

---

## 🧠 Key Learnings

* CI pipelines automate repetitive tasks
* GitHub Actions uses YAML configuration
* Workflow structure:

  * workflow → jobs → steps
* Each push can trigger automation
* Logs help debug failures
* Even small syntax errors can break pipelines

---

## ✅ Outcome

* Successfully created a CI pipeline
* Automated execution on code push
* Observed and debugged pipeline failure
* Understood workflow structure and execution flow

---

## 🚀 Next Step

Learn Docker and containerization to build and run applications in isolated environments (Day 6)
