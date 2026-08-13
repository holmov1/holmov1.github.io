# Ali Kholmovaia — personal site

## Structure

```
site/
├── index.html          ← main page (about, publications list, cv, links)
├── style.css           ← shared styles
└── README.md
```

## How to add creature icons

Replace any `<div class="icon-placeholder">icon</div>` with:

```html
<img src="images/your-creature.png" alt="creature">
```

Put your images in an `images/` folder (or wherever you want, just match the path).

## Deploy to GitHub Pages

1. Create a new repo on GitHub (e.g. `my-site` or `yourusername.github.io`)
2. Push this folder:

```bash
cd site
git init
git add .
git commit -m "first entry"
git remote add origin git@github.com:YOURUSERNAME/REPONAME.git
git push -u origin main
```

3. Go to repo **Settings → Pages**
4. Under "Source", pick **Deploy from a branch** → **main** → **/ (root)**
5. Hit Save

Your site will be live at `https://YOURUSERNAME.github.io/REPONAME/` within a minute or two.

If you name the repo `yourusername.github.io`, it'll be at `https://yourusername.github.io/` directly.

## Custom domain (optional)

If you buy a domain:
1. Add a file called `CNAME` containing just your domain (e.g. `ali.cool`)
2. Point your domain's DNS to GitHub Pages (their docs explain this)
