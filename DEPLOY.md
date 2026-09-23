# Getting this online, then into Figma

## 1. Upload to GitHub

1. Create a new repository on GitHub. Name it whatever you like — `peterson-linen-site` is fine. Make it **Public** (GitHub Pages needs public on a free plan).
2. On the repo's landing page, click **uploading an existing file**.
3. Unzip this folder on your computer. Open it, select **everything inside it** — `index.html`, the other nine `.html` files, `support.js`, `README.md`, `.nojekyll`, and the `assets` folder — and drag them into the browser window.
   - Drag the **contents**, not the `site` folder itself. If you upload the folder, every page ends up at `/site/index.html` and the images break.
   - The `assets` folder must come along. Images live in it; the pages reference it by relative path.
4. Type a commit message and click **Commit changes**.

## 2. Turn on GitHub Pages

1. In the repo, go to **Settings → Pages**.
2. Under **Build and deployment → Source**, choose **Deploy from a branch**.
3. Branch: `main`. Folder: `/ (root)`. Click **Save**.
4. Wait two or three minutes, then reload the Pages settings screen. Your URL appears at the top:
   `https://YOUR-USERNAME.github.io/peterson-linen-site/`
5. Open it. If images are missing, the `assets` folder did not upload — check step 1.

## 3. Import into Figma

Figma cannot open HTML files directly. You import the **live URL** from step 2 using a plugin.

**html.to.design** (the one most people use)

1. In Figma, open a new design file.
2. Right-click the canvas → **Plugins → Manage plugins**, search **html.to.design**, install it.
3. Run the plugin, paste your GitHub Pages URL, and import. Do each page separately — paste `.../index.html`, then `.../about.html`, and so on.
4. Set the viewport width before importing. Two passes is usually worth it: **1440** for desktop and **390** for mobile, so you have both layouts as frames.

Notes on what you get:
- Text, images, colours and layout come in as editable Figma layers. The Caramella and Libre Franklin type will map correctly if both fonts are installed on your machine or added to your Figma org — otherwise Figma substitutes them.
- Hover states, the Services dropdown and the sticky mobile call bar do not survive the import. They are CSS behaviour, not layout.
- The Google Map on Contact imports as an empty box. That is expected.

**Alternative:** if you only need visual reference rather than editable layers, take full-page screenshots of each URL and drop the PNGs into Figma.

## Page list

| File | Page |
| --- | --- |
| index.html | Home |
| about.html | About / Pamelyn Collins |
| services-personal-events.html | Personal Events |
| services-corporate-events.html | Corporate Events |
| our-linens.html | Our Linens + sizing guide |
| portfolio.html | Portfolio galleries |
| how-it-works.html | How It Works |
| faq.html | FAQ |
| trade.html | Trade & affiliates |
| contact.html | Contact + quote form |
