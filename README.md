# Experiment 1: Version Control & Hosting Documentation

**Student Name:** Harsh Kumar  
**Specialization:** B.Tech CSE (Data Science)  
**GitHub Profile:** [https://github.com/Harshrana00101](https://github.com/Harshrana00101)  

---

## Objective
Set up a clean Git repository for web development experiments, practice branch creation, merge feature branches into `main`, commit code with meaningful messages, push the repository to GitHub, and deploy it statically using GitHub Pages.

---

## Sequential Step-by-Step Commands

### Step 1: Initialize Git Repository
```bash
# Inside the root project folder
git init
```

### Step 2: Configure Git User Identity (if not already set)
```bash
git config user.name "Harsh Kumar"
git config user.email "harshrana00101@example.com"
```

### Step 3: Stage and Commit Initial Files on `main` Branch
```bash
git checkout -b main
git add .
git commit -m "feat: initial commit with experiments 1 to 6 and root directory showcase"
```

### Step 4: Practice Branching Workflow (Feature Branch & Merge)
```bash
# Create and switch to a development feature branch
git checkout -b feature/portfolio-updates

# Make any update or add documentation
git add experiment-1/
git commit -m "docs(exp-1): add version control and deployment documentation"

# Switch back to main and merge the feature branch
git checkout main
git merge feature/portfolio-updates

# Optionally delete the feature branch after merging
git branch -d feature/portfolio-updates
```

### Step 5: Connect Remote GitHub Repository and Push
```bash
# Link the local repository to your GitHub remote
# (Ensure the repository is created on your GitHub account)
git remote add origin https://github.com/Harshrana00101/web-development-experiments.git

# Push changes to GitHub
git push -u origin main
```

---

## GitHub Pages Deployment Steps

1. Open your repository on GitHub:  
   `https://github.com/Harshrana00101/web-development-experiments`
2. Navigate to **Settings** > **Pages** (under the "Code and automation" section in the left sidebar).
3. Under **Build and deployment**:
   - **Source**: Select `Deploy from a branch`.
   - **Branch**: Select `main` and leave the folder set to `/ (root)`.
   - Click **Save**.
4. Within 1–2 minutes, GitHub Actions will build and deploy your site.
5. Your live deployed URL will be:  
   **`https://harshrana00101.github.io/web-development-experiments/`**

Visiting this live URL opens the root portal, allowing anyone to preview all individual experiments directly!
