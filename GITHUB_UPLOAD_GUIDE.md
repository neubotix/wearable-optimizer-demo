# How to Upload to GitHub

Follow these steps to publish your Wearable Optimizer Demo to GitHub:

## Step 1: Create a GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in to your account `neubotix`
2. Click the **"+"** icon (top-right) → **"New repository"**
3. Fill in:
   - **Repository name**: `wearable-optimizer-demo`
   - **Description**: "Interactive 3D web app for wearable comfort engineering and optimization"
   - **Visibility**: Public (so interviewers can access it)
   - **Initialize with README**: ✗ (uncheck — we have our own)
4. Click **"Create repository"**

## Step 2: Prepare Your Local Files

You have all files ready in this folder. The structure is:

```
wearable-optimizer-demo/
├── index.html                    ← Main webapp
├── README.md                     ← Project documentation
├── LICENSE                       ← MIT License
├── .gitignore                    ← Git ignore rules
├── assets/
│   ├── hero.png                  ← Onboarding image
│   └── flame_head_with_ears.ply  ← Face mesh (for regeneration)
└── generator/
    ├── gen_samsung_demo.py       ← Python script to rebuild HTML
    └── requirements.txt          ← Python dependencies
```

## Step 3: Upload via Command Line (Recommended)

Open Terminal/PowerShell and run:

```bash
# Navigate to your project folder
cd /path/to/wearable-optimizer-demo

# Initialize git
git init

# Add all files
git add .

# Create initial commit
git commit -m "Initial commit: Wearable optimizer demo webapp"

# Add GitHub as remote (replace YOUR_USERNAME)
git remote add origin https://github.com/neubotix/wearable-optimizer-demo.git

# Push to GitHub
git branch -M main
git push -u origin main
```

## Step 4: Upload via GitHub Web UI (Alternative)

If command line is unfamiliar:

1. Go to your new repository on GitHub
2. Click **"Add file"** → **"Upload files"**
3. Drag and drop all files (or select them)
4. Write commit message: `Initial commit: Samsung AR glasses comfort demo`
5. Click **"Commit changes"**

Repeat for each folder (assets/, generator/).

## Step 5: Enable GitHub Pages (Optional - for Easy Sharing)

To make the app accessible via a GitHub Pages URL:

1. Go to your repository → **Settings** → **Pages**
2. Under "Build and deployment" → Source: select **main** branch
3. Click **Save**
4. Wait ~1 minute
5. Your app will be live at: `https://neubotix.github.io/wearable-optimizer-demo/`

Now interviewers can simply visit that URL to open the app!

## Step 6: Share with Interviewers

Send them one of these links:

### For Direct File Access:
```
https://github.com/neubotix/wearable-optimizer-demo
```

### For GitHub Pages (Easiest):
```
https://neubotix.github.io/wearable-optimizer-demo/
```

They can either:
- Click the **"index.html"** file and view it in GitHub's preview
- Download the entire repo and open `index.html` locally
- Visit the GitHub Pages link to run it live

## 💡 Pro Tips

- **Update the app**: Just push new commits with `git push`
- **Regenerate HTML**: Modify `generator/gen_samsung_demo.py`, run it to create a new `index.html`, then push
- **Add a badge**: Add this to your README for visual appeal:
  ```markdown
  [![Open Demo](https://img.shields.io/badge/Demo-Live-blue?style=flat-square)](https://neubotix.github.io/wearable-optimizer-demo/)
  ```

## ❓ FAQ

**Q: Do interviewers need to install anything?**
A: No! They just open `index.html` in a browser. It's completely self-contained.

**Q: Can I keep it private?**
A: Yes, set the repo to Private, but then share the link only with specific people (requires GitHub account).

**Q: How large is the app?**
A: ~463 KB for index.html (includes all 3D data embedded). PLY file is ~13 MB but only needed if regenerating.

**Q: What if I change the design?**
A: Edit `gen_samsung_demo.py`, run it, commit the new `index.html`, and push. Done!

---

Once uploaded, your webapp will be instantly accessible to interviewers worldwide. Good luck! 🚀
