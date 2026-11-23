# Pool wheel

A spinning wheel of pool forfeits that runs in any phone or desktop browser.

Live site: `https://<your-github-username>.github.io/pool-wheel/` once GitHub Pages is switched on (below).

## Put it online with GitHub Pages

1. On github.com, create a new **public** repository called `pool-wheel`.
2. Click **Add file → Upload files**, drag in everything from this folder (including `.nojekyll`), and commit.
3. Go to **Settings → Pages**. Under *Build and deployment*, set **Source: Deploy from a branch**, **Branch: main**, folder **/ (root)**, and save.
4. After a minute or two the page shows your link: `https://<your-github-username>.github.io/pool-wheel/`.

Anyone with the link can use it. On a phone, Share → **Add to Home Screen** gives it an icon and opens it full screen.

## Or from a terminal (GitHub CLI)

```bash
gh repo create pool-wheel --public --source . --push
gh api -X POST repos/{owner}/pool-wheel/pages -f "source[branch]=main" -f "source[path]=/"
```

## Editing

Everything is in `index.html`: the wheel artwork, the rules list and the spin code. Commit a change and the site updates within a couple of minutes.
