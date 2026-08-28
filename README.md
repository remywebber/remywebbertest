# Remy Webber — Portfolio

Static site, no build step required.

## Structure
```
index.html          → remywebber.com
work/index.html      → remywebber.com/work
contact/index.html   → remywebber.com/contact
CNAME                 → tells GitHub Pages to serve this at remywebber.com
```

## Deploy to GitHub Pages

1. Create a new GitHub repository and push the contents of this folder to it
   (the files should sit at the repo root, not inside a subfolder).
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to `Deploy from a branch`,
   branch `main`, folder `/ (root)`.
4. Under **Custom domain**, enter `remywebber.com` and save
   (this matches the included `CNAME` file — GitHub will detect it automatically).
5. At your domain registrar, point `remywebber.com` to GitHub Pages:
   - Add an **A record** for the root domain to GitHub's IPs:
     `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - If you also want `www.remywebber.com` to work, add a **CNAME record**
     for `www` pointing to `<your-github-username>.github.io`.
6. Back in GitHub Pages settings, tick **Enforce HTTPS** once the domain
   verifies (can take a few minutes to a few hours).

That's it — no build tools, frameworks, or dependencies involved.
