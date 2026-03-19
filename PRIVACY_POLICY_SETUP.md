# Privacy Policy Setup – CuriaAngels/Labs

**Main repo:** https://github.com/CuriaAngels/Labs

Instructions for hosting the CardNest privacy policy in the Labs repo.

---

## 1. Add the privacy policy via GitHub web UI

1. Go to **https://github.com/CuriaAngels/Labs**
2. Click **Add file** → **Create new file**
3. In the filename box, type: `index.html`
4. Paste the content below into the editor
5. Click **Commit changes** → **Commit changes**

---

## 2. File content (paste into the editor)

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Privacy Policy – CardNest</title>
    <style>
        body { font-family: system-ui, sans-serif; max-width: 640px; margin: 2rem auto; padding: 0 1rem; line-height: 1.6; color: #333; }
        h1 { font-size: 1.5rem; margin-bottom: 0.5rem; }
        .updated { color: #666; font-size: 0.9rem; margin-bottom: 1.5rem; }
        h2 { font-size: 1.1rem; margin-top: 1.5rem; }
        p { margin: 0.5rem 0; }
    </style>
</head>
<body>
    <h1>Privacy Policy</h1>
    <p class="updated">CardNest · Last updated: March 2025</p>

    <p>CardNest is a privacy-focused app for storing and displaying loyalty and benefit cards.</p>

    <h2>Data storage</h2>
    <p>All data (card images, barcodes, notes) is stored <strong>only on your device</strong>. Nothing is sent to our servers or any third party.</p>

    <h2>Data collection</h2>
    <p>We do not collect personal information. The app does not require an account or login.</p>

    <h2>Data sharing</h2>
    <p>We do not share any data with third parties. Your cards stay on your device.</p>

    <h2>Data security</h2>
    <p>Card data is stored locally using encrypted storage (SQLCipher).</p>

    <h2>Data deletion</h2>
    <p>You can delete cards at any time in the app. Uninstalling the app removes all stored data from your device.</p>

    <h2>Ads and tracking</h2>
    <p>CardNest contains no ads and does not use tracking or analytics.</p>

    <h2>Contact</h2>
    <p>Curia Angels Labs · <a href="mailto:curia.angels.labs@gmail.com">curia.angels.labs@gmail.com</a></p>
</body>
</html>
```

---

## 3. Enable GitHub Pages

1. Go to **https://github.com/CuriaAngels/Labs**
2. **Settings** → **Pages** (under Code and automation)
3. **Build and deployment:**
   - **Source:** Deploy from a branch
   - **Branch:** `main`
   - **Folder:** `/ (root)`
4. Click **Save**
5. Wait 1–2 minutes for deployment

---

## 4. Privacy policy URL

**Main link (repo):** https://github.com/CuriaAngels/Labs

**Hosted page (after deployment):** https://curiaangels.github.io/Labs/  
*(Only works after you add `index.html` and enable GitHub Pages.)*

For Google Play Console, use the hosted page URL once it’s live.

---

## 5. Add to Play Console

1. Play Console → **Set privacy policy**
2. Paste: `https://curiaangels.github.io/Labs/` (or `https://github.com/CuriaAngels/Labs` until Pages is deployed)
3. Save
