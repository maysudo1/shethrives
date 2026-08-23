# She Thrives Coaching — Website

A single-page site for She Thrives Coaching (Relationship & Marriage Coaching). Self-contained — no build step required.

## What's in this folder

| File | Purpose |
|---|---|
| `index.html` | The entire site (HTML, CSS, and JS in one file) |
| `404.html` | Custom "page not found" page GitHub Pages will show for broken links |
| `.nojekyll` | Tells GitHub Pages to skip Jekyll processing and serve files as-is (required since this isn't a Jekyll site) |
| `README.md` | This file |

Fonts load from Google Fonts' CDN and the "Book a call" button links to Calendly — both require an internet connection to work, which is fine for a live site.

## Deploy to GitHub Pages (step by step)

### 1. Create a repository
Go to [github.com/new](https://github.com/new) and create a new repository (public repos get free GitHub Pages hosting). Name it whatever you like — for a **user/organization site** name it exactly `<your-username>.github.io`; for a **project site** any name works and your site will be served at `<your-username>.github.io/<repo-name>`.

### 2. Upload these files
**Easiest — no command line needed:**
- Open your new repo on GitHub → click **"Add file" → "Upload files"**
- Drag in `index.html`, `404.html`, and `.nojekyll` (you may need to show hidden files in your file explorer to see `.nojekyll`)
- Commit the changes

**Or, using git from the command line:**
```bash
cd path/to/this/folder
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

### 3. Turn on GitHub Pages
- In your repo, go to **Settings → Pages**
- Under **Source**, select **Deploy from a branch**
- Branch: `main`, folder: `/ (root)` → **Save**

### 4. Visit your site
GitHub will show a message like *"Your site is live at..."* — it can take a minute or two the first time. Your URL will be:
- `https://<your-username>.github.io/` (if you named the repo `<your-username>.github.io`), or
- `https://<your-username>.github.io/<repo-name>/` (for any other repo name)

### 5. (Optional) Custom domain
If you own a domain, add a `CNAME` file to this folder containing just your domain (e.g. `shethrivescoaching.com`), then point your domain's DNS at GitHub Pages following [GitHub's custom domain guide](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).

## Updating the site later
Just edit `index.html` and push/upload the change again — GitHub Pages redeploys automatically within a minute or so.
