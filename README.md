# Personal Website

A personal website hosted on GitHub Pages.

## Setup Instructions

1. **Create a GitHub repository** (if you haven't already)
   - Go to GitHub and create a new repository
   - Name it `yourusername.github.io` (replace `yourusername` with your GitHub username)
   - Make it public

2. **Push this code to GitHub**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/yourusername/yourusername.github.io.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to your repository on GitHub
   - Click on "Settings"
   - Scroll down to "Pages" in the left sidebar
   - Under "Source", select "Deploy from a branch"
   - Choose "main" branch and "/ (root)" folder
   - Click "Save"

4. **Configure Custom Domain** (optional)
   - In the same "Pages" settings section
   - Under "Custom domain", enter your domain name
   - Click "Save"
   - Add a `CNAME` file to your repository with your domain name
   - Configure DNS records with your domain provider:
     - Add a CNAME record pointing `www` to `yourusername.github.io`
     - Add an A record for the root domain pointing to GitHub's IPs:
       - 185.199.108.153
       - 185.199.109.153
       - 185.199.110.153
       - 185.199.111.153

Your site should be live at `https://yourusername.github.io` within a few minutes!

