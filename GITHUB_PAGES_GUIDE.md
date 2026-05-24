# Step-by-Step Guide: Deploying Your 10-Second Challenge Game to GitHub Pages

Follow these instructions to share your game with the world using GitHub Pages.

## Prerequisites
- A GitHub account (sign up for free at [github.com](https://github.com))
- Git installed on your computer
- Your 10-Second Challenge Game files

## Step 1: Create a GitHub Repository

1. **Sign in to GitHub** at [github.com](https://github.com)
2. **Create a new repository**:
   - Click the "+" icon in the top-right corner
   - Select "New repository"
   - Repository name: `time-challenge-game` (or any name you prefer)
   - Description: "A fun game where you try to stop the timer at exactly 10.000 seconds!"
   - Set visibility to "Public"
   - **Important**: Do NOT initialize with a README file (we'll add our own files)
   - Click "Create repository"

## Step 2: Prepare Your Game Files

1. **Open your project folder** (`time_challenge_game`)
2. **Create a `.gitignore` file** (optional but recommended):
   - Right-click in the folder
   - Select "New file"
   - Name it `.gitignore`
   - Add this content:
   ```
   # Logs
   logs
   *.log
   npm-debug.log*
   yarn-debug.log*
   yarn-error.log*
   
   # Dependencies
   node_modules
   
   # IDE files
   .idea
   .vscode
   *.swp
   *.swo
   
   # OS generated files
   .DS_Store
   Thumbs.db
   ```

## Step 3: Upload Your Files to GitHub

### Option A: Using Git Command Line

1. **Open Terminal** (Mac/Linux) or **Command Prompt** (Windows)
2. **Navigate to your project folder**:
   ```bash
   cd /home/user/vibecoding/workspace/time_challenge_game
   ```
3. **Initialize Git repository**:
   ```bash
   git init
   ```
4. **Add all files**:
   ```bash
   git add .
   ```
5. **Commit the files**:
   ```bash
   git commit -m "Initial commit - 10 Second Challenge Game"
   ```
6. **Link to GitHub repository**:
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/time-challenge-game.git
   ```
   (Replace `YOUR_USERNAME` with your actual GitHub username)
7. **Push files to GitHub**:
   ```bash
   git push -u origin master
   ```
   (You may be prompted to enter your GitHub username and password/Personal Access Token)

### Option B: Using GitHub Desktop (Easier)

1. **Download and install GitHub Desktop** from [desktop.github.com](https://desktop.github.com)
2. **Sign in** with your GitHub account
3. **Click "Add" → "Add Existing Repository"**
4. **Select your project folder** (`time_challenge_game`)
5. **Click "Create a New Repository on GitHub"**
6. **Fill in the details**:
   - Name: `time-challenge-game`
   - Description: "A fun game where you try to stop the timer at exactly 10.000 seconds!"
   - Set to "Public"
7. **Click "Publish Repository"**

### Option C: Upload Files Directly on GitHub (Simplest)

1. **Go to your new repository** on GitHub
2. **Click "Add file" → "Upload files"**
3. **Drag and drop** all files from your `time_challenge_game` folder
4. **Scroll down and click "Commit changes"**

## Step 4: Enable GitHub Pages

1. **Go to your repository** on GitHub
2. **Click "Settings"** (tab near the top)
3. **Scroll down to "Pages"** section in the left sidebar
4. **Under "Source"**:
   - Click the dropdown menu
   - Select `main` or `master` branch
   - Select `/ (root)` folder
   - Click "Save"
5. **Wait a few minutes** for GitHub to build your site
6. **Refresh the page** - you should see a message:
   "Your site is published at https://YOUR_USERNAME.github.io/time-challenge-game/"

## Step 5: Share Your Game!

🎉 **Congratulations!** Your game is now live on the internet.

**Share this URL with anyone**:
`https://YOUR_USERNAME.github.io/time-challenge-game/`

## Troubleshooting

- **Site not loading?** Wait a few minutes - GitHub Pages can take time to build
- **404 Error?** Check that you selected the correct branch and folder in settings
- **Styling issues?** Ensure all CSS files were uploaded correctly
- **Need help?** Check GitHub's documentation at [docs.github.com/en/pages](https://docs.github.com/en/pages)

## Updating Your Game

When you make changes to your game:

### Using Git:
```bash
git add .
git commit -m "Description of your changes"
git push origin master
```

### Using GitHub Desktop:
1. Make your changes
2. GitHub Desktop will detect the changes
3. Add a commit message
4. Click "Commit to master"
5. Click "Push origin"

The changes will automatically appear on your GitHub Pages site within a few minutes.