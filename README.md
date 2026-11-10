# EST Internship Hub + Survival Guide

One password-protected website with two sides: the **Internship Hub** (companies and vacancies) and the **Survival Guide** (first-internship help). Use the two big buttons at the top to switch.

Files:
- `index.html` is the website (design and password lock). The page content is encrypted inside it.
- `content.json` is the written content of the **Survival Guide**.
- `companies.json` is the **Internship Hub** data: dates in `settings`, and one block per company in `companies` (quota, filled, address, email, roles).
- `.nojekyll` is an empty helper file for GitHub Pages. Keep it.

## Put it online with GitHub Pages (free)

1. Create a new **public** repository on GitHub, for example `est-hub`.
2. Upload all five files and click **Commit changes**.
3. Open **Settings → Pages**, choose **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
4. After 1–2 minutes the site is at `https://YOUR-USERNAME.github.io/est-hub/`.

## Edit

Open `content.json` or `companies.json` on GitHub, click the pencil icon, change the text between the quotation marks, then **Commit changes**. To add a company, copy a whole `{ ... }` block (comma between blocks) and give it a new unique `id`. "Places left" is quota minus filled.
A missing comma or quotation mark breaks the file; if the site shows old text after you edit, check the JSON in an online validator. If a JSON file is broken or missing, the site uses the built-in copy.

## Password

The site asks for a password before opening. `index.html` is encrypted, so the text inside it cannot be read from the page source. A new password needs a rebuilt `index.html`.
Important: `content.json` and `companies.json` are ordinary files in a public repository, so anyone who knows their address can read them. Do not put private information in them.
