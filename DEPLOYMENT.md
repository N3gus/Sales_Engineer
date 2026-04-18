# GitHub Pages Deployment Guide

## Setup Instructions

### 1. Initialize Git Repository

```bash
git init
git add .
git commit -m "Initial Jekyll site setup"
```

### 2. Create GitHub Repository

1. Go to [GitHub](https://github.com) and create a new repository
2. Name it: `N3gus.github.io` (replace with your username)
3. Set it as Public
4. Don't initialize with README (we already have one)

### 3. Push to GitHub

```bash
git remote add origin https://github.com/N3gus/N3gus.github.io.git
git branch -M main
git push -u origin main
```

### 4. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** tab
3. Scroll down to **Pages** section
4. Under "Build and deployment", select **GitHub Actions**
5. Save the settings

### 5. Deploy

The GitHub Actions workflow will automatically:
- Build your Jekyll site
- Deploy it to GitHub Pages
- Make it available at `https://N3gus.github.io`

## What's Been Configured

### GitHub Actions Workflow (`.github/workflows/jekyll.yml`)
- Triggers on push to main branch
- Builds Jekyll site with production settings
- Deploys to GitHub Pages automatically

### Jekyll Configuration (`_config.yml`)
- Configured for GitHub Pages deployment
- URL set to `https://N3gus.github.io`
- Includes GitHub Pages specific plugins

### Dependencies (`Gemfile`)
- Uses `github-pages` gem for compatibility
- Includes all necessary Jekyll plugins

### Optimization Files
- `.nojekyll` file for faster deployment
- Proper asset structure for GitHub Pages

## Troubleshooting

### Build Failures
Check the **Actions** tab in your GitHub repository for build logs.

### Site Not Updating
- Wait a few minutes for deployment to complete
- Check if GitHub Actions completed successfully
- Clear browser cache

### Custom Domain
To use a custom domain, create a `CNAME` file:
```bash
echo "yourdomain.com" > CNAME
git add CNAME
git commit -m "Add custom domain"
git push
```

## Live Site

Once deployed, your site will be available at:
- **Primary**: `https://N3gus.github.io`
- **Custom domain**: (if configured)

The site includes:
- Responsive design
- SEO optimization
- Modern animations
- Contact links
- Professional portfolio layout
