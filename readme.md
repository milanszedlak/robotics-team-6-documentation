# 🚀 Team 6 - Leo Rover Documentation

Welcome to the official documentation repository for **Team 6's Leo Rover Project**. This repository serves as the central hub for all technical guides, system architecture notes, hardware specifications, and project updates related to our Leo Rover build and deployment.

---

## 🛠️ Git & GitHub Workflow Guide

To keep our documentation organized and prevent merge conflicts, please follow our team's standard Git workflow whenever you update or add content.

### 📌 Branch Naming Convention

Always create a new branch for your work. Branches must follow this standard format:

```text
[YOUR_NAME]/[ACTION_THAT_YOU_ARE_DOING]
```

**Examples:**
- `milan/add-teleop-guide`
- `keara/update-wiring-diagram`

---

## 💡 Key Git Commands Reference

Here are the essential commands you will need during development:

| Command | Description |
| :--- | :--- |
| `git fetch origin` | Fetches updates from the remote repository without merging them. |
| `git pull origin main` | Pulls and merges the latest changes from the main branch into your current branch. |
| `git checkout -b <branch-name>` | Creates a new local branch and switches to it. |
| `git checkout <branch-name>` | Switches to an existing branch. |
| `git status` | Displays the status of working directory files (modified, untracked, staged). |
| `git add <file-path>` | Stages specific files for the next commit (use `git add .` to stage all changes). |
| `git commit -m "Your descriptive message"` | Commits staged changes with a clear description. |
| `git push origin <branch-name>` | Pushes your local branch and commits to GitHub. |

---

## 📖 Step-by-Step Example Workflow: Adding a New Document

Here is a full walkthrough showing how to add a new document (e.g., `camera_setup.md`) and open a Pull Request (PR).

### Step 1: Get the Latest Main Branch
Before starting new work, make sure your local `main` branch is up to date:
```bash
git checkout main
git fetch origin
git pull origin main
```

### Step 2: Create a New Branch
Create and switch to your feature branch using the required naming convention:
```bash
git checkout -b alex/add-camera-setup-guide
```

### Step 3: Add Your Content
Create your new file inside the `docs/` directory:
```bash
# Example: Create and write your document in docs/camera_setup.md
```

### Step 4: Stage and Commit Your Changes
Check what files were modified, stage them, and write a clear commit message:
```bash
git status
git add docs/camera_setup.md
git commit -m "docs: add setup and configuration guide for Leo Rover camera"
```

### Step 5: Push Your Branch to GitHub
Push your local branch to the remote GitHub repository:
```bash
git push origin alex/add-camera-setup-guide
```

### Step 6: Create a Pull Request (PR)
1. Go to the repository on **GitHub**.
2. You will see a banner prompting you to **"Compare & pull request"** for your recently pushed branch. Click it.
3. Fill out the PR details:
   - **Title**: Provide a brief title describing the change (e.g., `Add Leo Rover Camera Setup Guide`).
   - **Description**: Briefly explain what document was added or modified.
4. Select at least **one teammate from Team 6** as a reviewer.
5. Click **Create pull request**.
6. Once reviewed and approved by a team member, merge the PR into `main` and delete the feature branch.

---

## 🤝 Team 6 Best Practices
- Keep commit messages concise and informative.
- Never commit directly to the `main` branch.
- Always review your changes locally before opening a pull request.