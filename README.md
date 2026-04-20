# Overions — Landing Page

A static landing page built with plain HTML and CSS. No build tools, no frameworks.

## Editing content

Open `index.html` and find-and-replace every `{{ PLACEHOLDER }}`. That's all your copy.

## Changing colors, fonts, or spacing

Open `styles.css` and look at the `:root` block at the top. Every color, font, and layout value is defined there as a variable — change once, applied everywhere.

Current design direction:
- **Palette:** near-black background (`--bg`) with an amber accent (`--accent`)
- **Display font:** Bricolage Grotesque (headlines)
- **Body font:** Geist (paragraphs, UI)
- **Technical font:** Geist Mono (eyebrows, labels, numbers)

All three fonts load from Google Fonts — no install needed.

## Deploying to GitHub Pages

1. Push `index.html` and `styles.css` to the **root** of your GitHub repo on the `main` branch.
2. In the repo, go to **Settings → Pages**.
3. Under **Source**, choose **Deploy from a branch**.
4. Pick branch `main`, folder `/ (root)`, and click **Save**.
5. Wait 1–2 minutes. Your site will be live at `https://<your-username>.github.io/<repo-name>/`.

## Connecting your Squarespace domain

Once your DNS records have propagated:

1. In your repo, go to **Settings → Pages**.
2. In **Custom domain**, enter your domain (e.g. `overions.com`) and save. GitHub will create a `CNAME` file in your repo automatically.
3. Wait for GitHub to provision an SSL certificate (can take up to an hour).
4. Once available, tick **Enforce HTTPS**.

### DNS records you need (for reference)

In Squarespace's DNS settings, you should have:

- Four `A` records on `@` pointing to GitHub's IPs: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- One `CNAME` record on `www` pointing to `<your-username>.github.io`

## Important: financial disclaimer

The footer contains a placeholder legal disclaimer. Before launch, **have it reviewed by a lawyer familiar with financial services regulation in your jurisdiction** (for the Netherlands/EU this likely means MiFID II and AFM rules). Requirements differ dramatically depending on whether Overions provides advice, executes trades, distributes a product, or only sells software tools.

## Files

| File         | What it does                          |
|--------------|---------------------------------------|
| `index.html` | Page structure and all text content   |
| `styles.css` | All visual styling and layout         |
| `README.md`  | This file                             |
