# Spotty — GitHub Pages Deployment Package 🎵

This folder contains the pre-built, production-ready files configured for **GitHub Pages** (or any static hosting service like Netlify, Vercel, or Cloudflare Pages).

---

## 🚀 How to Put Spotty on GitHub Pages (2 Minutes)

You have **two easy methods** to deploy:

---

### Option 1: Drag & Drop Upload (No Git terminal needed)

1. **Go to GitHub**:
   - Head to [github.com/new](https://github.com/new) and log in.
   - Name your repository (for example: `spotty` or `spotty-music`).
   - Keep it **Public** (required for free GitHub Pages).
   - Click **Create repository**.

2. **Upload these files**:
   - On the new repository page, click the link that says **"uploading an existing file"**.
   - Drag and drop **all files and the `assets` folder** from this `github-pages-ready` directory directly into GitHub in your browser.
   - Click **Commit changes** (green button at the bottom).

3. **Activate GitHub Pages**:
   - In your repository, click **Settings** (tab at the top right).
   - In the left sidebar, click **Pages**.
   - Under **Build and deployment**:
     - **Source**: Select `Deploy from a branch`.
     - **Branch**: Choose `main` (or `master`) and folder `/ (root)`.
     - Click **Save**.

4. **Done! 🎉**:
   - Wait 30–60 seconds, then refresh the page.
   - GitHub will display your live link:
     ```
     https://<your-username>.github.io/<repository-name>/
     ```
   - Open that link on your PC or iPhone Safari to enjoy Spotty!

---

### Option 2: Push with Git & Auto-Deploy via GitHub Actions

If you prefer using the Git command line:

1. In the project root (`Spotty`), initialize and push:
   ```bash
   git init
   git add .
   git commit -m "Initial Spotty PWA release"
   git branch -M main
   git remote add origin https://github.com/<your-username>/spotty.git
   git push -u origin main
   ```

2. Turn on GitHub Pages via Actions:
   - Go to your repository on GitHub -> **Settings** -> **Pages**.
   - Under **Build and deployment > Source**, select **GitHub Actions**.
   - Spotty already includes `.github/workflows/deploy.yml`! GitHub will automatically build and deploy every time you push changes!

---

## 📱 Installing on iOS (iPhone / iPad)

Once your GitHub Pages link is live:
1. Open your GitHub Pages link (e.g. `https://<your-username>.github.io/spotty/`) in **Safari** on your iPhone.
2. Tap the **Share** button (box with an arrow pointing up at the bottom).
3. Scroll down and tap **"Add to Home Screen"** (`Tilføj til hjemmeskærm`).
4. Tap **Add** (`Tilføj`).
5. Spotty will appear on your iPhone home screen with its official icon, full-screen playback, lock-screen controls, and equalizer!

---

## 🌐 Custom Domain (Optional)

If you own a custom domain (e.g. `music.mywebsite.com`):
1. In your GitHub repo -> **Settings** -> **Pages**.
2. Under **Custom domain**, enter your domain name and click **Save**.
3. Create a `CNAME` DNS record in your domain registrar pointing to `<your-username>.github.io`.
