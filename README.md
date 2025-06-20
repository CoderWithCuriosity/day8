# day8
---

# ✅ **Git & GitHub Guide for Beginners**

## **What is Git and Why Use It?**

### 1️⃣ **What is Git?**

* Git is a **Version Control System (VCS)**.
* **Purpose:** Track changes in your code, collaborate with others.
* Think of **Google Docs revision history** but for code.

### 2️⃣ **Why Git?**

* Saves every change.
* You can **revert** if something breaks.
* Allows **collaboration** with others on coding projects.

### 3️⃣ **What is GitHub?**

* **GitHub = Online storage for your Git projects.**
* You can share, contribute, or show your projects publicly or privately.

---

## **Setting Up Git**

### ✅ **Install Git:**

* **Windows:** [https://git-scm.com/download/win](https://git-scm.com/download/win)
* **Mac:** `brew install git`
* **Linux:** `sudo apt-get install git`

### ✅ **Check Git Installed:**

```bash
git --version
```

### ✅ **Configure Git:**

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

---

##  **Basic Git Workflow**

### 1️⃣ **Create a New Project Folder**

```bash
mkdir my-first-project
cd my-first-project
```

### 2️⃣ **Initialize Git**

```bash
git init
```

This creates a `.git` folder = starts tracking.

### 3️⃣ **Add Files**

```bash
echo "Hello World" > index.html
```

### 4️⃣ **Track Files**

```bash
git add index.html
```

### 5️⃣ **Commit Changes**

```bash
git commit -m "Initial commit"
```

> 📌 **add** → stage for commit
> 📌 **commit** → save snapshot

---

##  **Git Status, Logs, and Undo**

### ✅ **Check Status**

```bash
git status
```

### ✅ **Check Commit History**

```bash
git log
```

### ✅ **Undo a Mistake**

```bash
git checkout -- index.html
```

### ✅ **Remove File from Staging**

```bash
git reset index.html
```

---

## **Branches in Git**

### ⚡ **Why Branches?**

* Work on **new features** without messing up the main project.

### ✅ **Create Branch**

```bash
git branch new-feature
```

### ✅ **Switch to Branch**

```bash
git checkout new-feature
```

### ✅ **Merge Branch**

```bash
git checkout main
git merge new-feature
```

---

## **GitHub Basics**

### ✅ **Create a GitHub Account**

[https://github.com/](https://github.com/)

### ✅ **Create a Repository on GitHub**

* Click **New** on GitHub
* Name it: `my-first-project`
* Don’t initialize with README

### ✅ **Connect Local Project to GitHub**

```bash
git remote add origin https://github.com/your-username/my-first-project.git
```

### ✅ **Push to GitHub**

```bash
git push -u origin main
```

---

## ** Cloning, Pulling, and Collaboration**

### ✅ **Clone a Repository (Downloading)**

```bash
git clone https://github.com/username/project.git
```

### ✅ **Pull Changes (Update Your Local)**

```bash
git pull
```

### ✅ **Collaboration with Others**

1. Fork the repository (if not yours)
2. Clone it.
3. Push changes to your copy.
4. Open a **Pull Request (PR)** to contribute.

---

## 🗂️ **Summary of Basic Git Commands**

| Command                       | What it Does                     |
| ----------------------------- | -------------------------------- |
| `git init`                    | Start Git in a folder            |
| `git add file`                | Stage file for commit            |
| `git commit -m "msg"`         | Save changes                     |
| `git status`                  | Show changed/staged files        |
| `git log`                     | Show commit history              |
| `git branch`                  | List branches                    |
| `git checkout branch`         | Switch branch                    |
| `git merge branch`            | Merge branch into current branch |
| `git remote add origin <URL>` | Connect local Git to GitHub      |
| `git push`                    | Upload changes to GitHub         |
| `git pull`                    | Download updates from GitHub     |

---

## ✅

Next Level:

* `.gitignore`
* Pull Requests
* Resolving Conflicts
* GitHub Actions (CI/CD)

---