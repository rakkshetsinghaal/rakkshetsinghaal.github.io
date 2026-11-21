# rakkshet-singhaal website

Two plain HTML pages and one stylesheet. No build step: edit a file, commit, push.

| File | What it holds |
|---|---|
| `index.html` | Home: bio, contact, CV button |
| `research.html` | Publications, Presentations, Additional Research |
| `style.css` | All styling. The six palette colors are at the top, in `:root` |
| `files/Singhaal_CV.pdf` | The CV behind every "CV" link. Replace this file to update it |

**Add a paper or talk:** in `research.html`, copy an existing `<li class="entry"> … </li>` block, paste it where it belongs, and change the text. Abstracts go inside `<details>`. Delete that block for entries without one.

**Change the header or footer:** both pages share the same markup, so edit it in both files. Also update "Last updated" in the footer.

**Preview locally:** double-click `index.html`.

## Publish on GitHub Pages (free)
1. Create a GitHub account, then a **public** repository named exactly `<your-username>.github.io`.
2. From this folder:
   ```
   git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
   git push -u origin main
   ```
3. On GitHub, go to **Settings → Pages**, set Source to *Deploy from a branch*, choose `main` and `/ (root)`, and save. The site goes live at `https://<your-username>.github.io` within a minute or two.

## Optional: custom domain (about $12/year)
Buy a domain (e.g. `rakkshetsinghaal.com`) from any registrar. In **Settings → Pages → Custom domain**, enter it; GitHub adds a `CNAME` file. At the registrar, add the DNS records GitHub lists: four `A` records for the apex domain and a `CNAME` for `www` pointing to `<your-username>.github.io`. Then tick **Enforce HTTPS**.
