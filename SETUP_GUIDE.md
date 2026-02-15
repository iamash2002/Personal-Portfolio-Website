# 🚀 Complete Setup Guide

## Step-by-Step Instructions to Run Your Portfolio

### 1. Prerequisites

Before you begin, make sure you have these installed on your computer:

- **Node.js** (version 16 or higher)
  - Download from: https://nodejs.org/
  - To check if installed, run: `node --version`
  
- **Git** (for GitHub upload)
  - Download from: https://git-scm.com/
  - To check if installed, run: `git --version`

### 2. Download the Project

1. Download the `ashish-portfolio` folder from Claude
2. Extract it to your desired location (e.g., Desktop, Documents)

### 3. Install Dependencies

Open Terminal (Mac/Linux) or Command Prompt (Windows):

```bash
# Navigate to the project folder
cd path/to/ashish-portfolio

# For example:
# cd Desktop/ashish-portfolio

# Install all required packages
npm install
```

This will download all necessary packages (React, Vite, Tailwind CSS, etc.)

### 4. Run the Portfolio Locally

After installation completes:

```bash
# Start the development server
npm run dev
```

You should see output like:
```
VITE v4.3.9  ready in 500 ms

➜  Local:   http://localhost:5173/
➜  Network: use --host to expose
```

**Open your browser and go to:** `http://localhost:5173`

Your portfolio should now be running! 🎉

### 5. Make Changes (Optional)

- To edit content: Open `src/App.jsx` in any code editor (VS Code recommended)
- To change photo: Replace `public/ashish-photo.jpeg` with your photo
- The browser will automatically reload when you save changes

### 6. Build for Production

When you're ready to deploy:

```bash
npm run build
```

This creates an optimized `dist` folder with your production files.

---

## 📤 Upload to GitHub

### First Time Setup

1. **Create a GitHub account** (if you don't have one)
   - Go to: https://github.com/signup

2. **Create a new repository**
   - Go to: https://github.com/new
   - Repository name: `portfolio` or `ashish-portfolio`
   - Description: "My personal portfolio website"
   - Keep it **Public**
   - **DO NOT** check "Add a README file"
   - Click "Create repository"

3. **Upload your project**

Open Terminal in your project folder:

```bash
# Initialize git (only needed first time)
git init

# Add all files
git add .

# Commit your files
git commit -m "Initial commit: Portfolio website"

# Add your GitHub repository as remote
# Replace 'yourusername' with your actual GitHub username
git remote add origin https://github.com/yourusername/portfolio.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Update Your Portfolio (After Making Changes)

Whenever you make changes and want to update GitHub:

```bash
# Add changed files
git add .

# Commit with a message
git commit -m "Update portfolio content"

# Push to GitHub
git push
```

---

## 🌐 Deploy Your Portfolio Online (FREE)

### Option 1: Vercel (Recommended - Easiest)

1. Go to https://vercel.com/
2. Sign up with your GitHub account
3. Click "Add New Project"
4. Select your portfolio repository
5. Click "Deploy"
6. Done! Your site will be live at: `your-portfolio.vercel.app`

**Every time you push to GitHub, Vercel automatically updates your site!**

### Option 2: Netlify

1. Go to https://www.netlify.com/
2. Sign up with your GitHub account
3. Click "Add new site" → "Import an existing project"
4. Select GitHub and choose your repository
5. Build command: `npm run build`
6. Publish directory: `dist`
7. Click "Deploy"
8. Your site will be live at: `your-portfolio.netlify.app`

### Option 3: GitHub Pages

1. Install gh-pages:
   ```bash
   npm install --save-dev gh-pages
   ```

2. Add to `package.json` (in the "scripts" section):
   ```json
   "homepage": "https://yourusername.github.io/portfolio",
   "scripts": {
     "predeploy": "npm run build",
     "deploy": "gh-pages -d dist"
   }
   ```

3. Update `vite.config.js`:
   ```javascript
   export default defineConfig({
     plugins: [react()],
     base: '/portfolio/',  // Add this line (use your repo name)
   })
   ```

4. Deploy:
   ```bash
   npm run deploy
   ```

5. Enable GitHub Pages:
   - Go to your repository on GitHub
   - Settings → Pages
   - Source: Deploy from a branch
   - Branch: `gh-pages` → `/ (root)`
   - Save

Your site will be live at: `https://yourusername.github.io/portfolio`

---

## 🔧 Troubleshooting

### Port Already in Use

If you see "Port 5173 is already in use":
```bash
# Kill the process and try again
npm run dev -- --port 3000
```

### Dependencies Error

If you get errors during `npm install`:
```bash
# Clear cache and reinstall
rm -rf node_modules package-lock.json
npm install
```

### Image Not Loading

- Make sure `ashish-photo.jpeg` is in the `public` folder
- Check the filename matches exactly (case-sensitive)
- Try clearing browser cache (Ctrl+Shift+R or Cmd+Shift+R)

### Build Errors

If `npm run build` fails:
```bash
# Try cleaning and rebuilding
rm -rf dist
npm run build
```

---

## 📞 Need Help?

If you run into issues:

1. Check the error message in the terminal
2. Google the error message
3. Ask on Stack Overflow
4. Check GitHub Issues for similar problems

---

## 🎉 You're All Set!

Your portfolio is now:
- ✅ Running locally
- ✅ Uploaded to GitHub
- ✅ Deployed online (if you chose a hosting option)

**Next Steps:**
- Customize the content to make it yours
- Add more projects as you complete them
- Share your portfolio link on LinkedIn and your resume!

Good luck! 🚀
