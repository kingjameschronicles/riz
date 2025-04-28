# Hosting The King's Library on GitHub

Follow these steps to host your educational game about King James I and Shakespeare on GitHub.

## Step 1: Create a GitHub Account (if you don't have one)

1. Go to [GitHub.com](https://github.com)
2. Sign up for a free account

## Step 2: Create a New Repository

1. Click on the "+" icon in the top right corner of GitHub and select "New repository"
2. Name your repository (e.g., "kings-library")
3. Add a description: "An educational 2D game about King James I's influence on Shakespeare and theater"
4. Choose "Public" visibility
5. Check "Add a README file"
6. Click "Create repository"

## Step 3: Upload Your Files

### Option 1: Upload via GitHub Web Interface

1. In your new repository, click the "Add file" dropdown and select "Upload files"
2. Drag and drop all the files from this project (excluding node_modules folder)
3. Add a commit message like "Initial upload of The King's Library game"
4. Click "Commit changes"

### Option 2: Upload via Git Command Line (Recommended)

1. Install Git on your computer if you haven't already
2. Open a terminal/command prompt
3. Navigate to your project directory
4. Run the following commands:

```bash
git init
git add .
git commit -m "Initial commit of The King's Library game"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/kings-library.git
git push -u origin main
```

Replace `YOUR_USERNAME` with your GitHub username.

## Step 4: Set Up GitHub Pages for Hosting

1. Go to your repository on GitHub
2. Click on "Settings"
3. Scroll down to "Pages" in the left sidebar
4. Under "Source", select "GitHub Actions"
5. Choose a workflow template or use the one already included in this project

The GitHub Actions workflow will automatically build and deploy your project when you push changes to the main branch.

## Step 5: View Your Deployed Game

After the workflow completes (usually takes a few minutes):

1. Go to the "Actions" tab in your repository to see the deployment progress
2. Once complete, your game will be available at: `https://YOUR_USERNAME.github.io/kings-library/`

## Making Updates

When you want to update your game:

1. Make your changes locally
2. Commit and push to GitHub:

```bash
git add .
git commit -m "Description of your changes"
git push
```

The GitHub Actions workflow will automatically rebuild and redeploy your game.

## Customizing the Domain (Optional)

If you want to use a custom domain instead of the default GitHub Pages URL:

1. Go to your repository settings
2. Under "Pages", enter your custom domain
3. Update your domain's DNS settings as instructed by GitHub
4. Add a CNAME file to your repository

## Need Help?

If you encounter any issues with GitHub hosting, refer to the [GitHub Pages documentation](https://docs.github.com/en/pages) or reach out to the GitHub community for assistance.