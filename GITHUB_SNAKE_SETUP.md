# GitHub Snake Setup Guide

Follow these steps to set up your GitHub contribution snake animation:

## Step 1: Create Your GitHub Profile Repository

1. Go to GitHub and create a **new repository**
2. Name it exactly: `phantomexile` (same as your username)
3. Make it **public**
4. Initialize with a README (or use the README.md file I created)

## Step 2: Add the Workflow File

1. In your `phantomexile/phantomexile` repository, create this folder structure:
   ```
   .github/
     workflows/
       generate-snake.yml
   ```

2. Copy the content from `.github/workflows/generate-snake.yml` (I created this file for you in the port2 folder)

3. Commit and push the file to your repository

## Step 3: Enable GitHub Actions

1. Go to your repository settings
2. Navigate to **Actions** → **General**
3. Under "Workflow permissions", select:
   - ✅ **Read and write permissions**
4. Click **Save**

## Step 4: Run the Action

1. Go to the **Actions** tab in your repository
2. Click on "Generate Snake" workflow
3. Click **Run workflow** → **Run workflow**
4. Wait for it to complete (usually takes 1-2 minutes)

## Step 5: Verify

After the action completes successfully:

1. A new branch called `output` will be created
2. Check if these files exist in the `output` branch:
   - `github-contribution-grid-snake.svg`
   - `github-contribution-grid-snake-dark.svg`

## Step 6: Test in Your Portfolio

Your portfolio is already configured to use these files from:
```
https://raw.githubusercontent.com/phantomexile/phantomexile/output/github-contribution-grid-snake.svg
https://raw.githubusercontent.com/phantomexile/phantomexile/output/github-contribution-grid-snake-dark.svg
```

Once the action runs successfully, your portfolio will automatically display your real GitHub contributions!

## Troubleshooting

**If the action fails:**
- Make sure the repository is public
- Check that workflow permissions are set to "Read and write"
- Verify your GitHub token has the necessary permissions

**If images don't load:**
- Wait a few minutes for GitHub's CDN to update
- Clear your browser cache
- Check the `output` branch exists and has the SVG files

## Automatic Updates

The snake will automatically update:
- ✅ Every 24 hours (at midnight UTC)
- ✅ Every time you push to the main branch
- ✅ Manually from the Actions tab

---

Need help? Check the [Platane/snk documentation](https://github.com/Platane/snk)
