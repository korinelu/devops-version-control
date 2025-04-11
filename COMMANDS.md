✅ FULL COMMAND LIST


🟢 Step 1: Initialize Project & Push to GitHub


# Create project folder

mkdir devops-version-control

cd devops-version-control

# Initialize Git

git init

# Create README

echo "# DevOps Version Control Project" > README.md

# Stage and commit initial file

git add README.md

git commit -m "Initial commit"

# Rename branch to main

git branch -M main

# Add remote origin (replace with your GitHub URL)

git remote add origin https://github.com/YOUR_USERNAME/devops-version-control.git

# Push main branch

git push -u origin main

🟡 Step 2: Create Branches

# Create dev branch

git checkout -b dev

git push -u origin dev

# Create feature branch

git checkout -b feature/initial-setup

git push -u origin feature/initial-setup

🔵 Step 3: Add .gitignore File

# Create .gitignore

touch .gitignore

# Open and edit .gitignore (or use echo if scripting)

echo "__pycache__/" >> .gitignore

echo "*.pyc" >> .gitignore

echo "node_modules/" >> .gitignore

echo ".env" >> .gitignore

echo ".DS_Store" >> .gitignore

echo "*.log" >> .gitignore

# Stage and commit

git add .gitignore

git commit -m "Add .gitignore file"

git push

🟣 Step 4: Work on README and Tasks (Feature Branch)

# Add project details to README

echo "## Project Overview" >> README.md

# Create TASKS.md and add logs

touch TASKS.md

echo "# DevOps Version Control Project Tasks" >> TASKS.md

# Stage and commit changes

git add README.md TASKS.md

git commit -m "Add README overview and TASKS log"

git push

🟤 Step 5: Merge via Pull Request (on GitHub)

📌 No CLI command here. You did this on GitHub UI:

Open PR: feature/initial-setup → dev

Review and Merge

⚫ Step 6: Merge dev → main and Tag Release

# Switch to main and merge dev

git checkout main

git pull

git merge dev

git push

# Tag version

git tag v1.0

git push origin v1.0

🟠 Optional Cleanup (Delete local feature branch)

git branch -d feature/initial-setup

git push origin --delete feature/initial-setup  # if you want to remove from GitHub

