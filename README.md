# TaaPlay Landing Page — Setup Guide

## 📂 File Map
/
├── index.html # Main landing page
├── style.css # Shared theme & layout styles
├── script.js # Behaviour (smooth scroll, nav, FAQ, Kit integration)
├── thanks.html # Post-subscription confirmation & download page
├── assets/
│ ├── brand/ # Logos, icons, OG images
│ └── taaplay-starter-pack.zip # Placeholder downloadable pack

---

## 🌐 Hosting on GitHub Pages
1. **Repository Setup**
   - Commit all files to a public GitHub repository.
   - Ensure `index.html` is at the root of the default branch (`main` or `master`).

2. **Enable Pages**
   - Go to **Settings → Pages** in your repo.
   - Set **Source** to `Deploy from a branch` and select your branch + root folder.
   - Save. Your site will be live at `https://<username>.github.io/<repo>/`.

3. **Asset Paths**
   - Use relative paths (`assets/...`) so the site works locally and on GitHub Pages.

---

## 🔌 Adding the Real Kit (ConvertKit) Embed
In **`script.js`**, find the `initKitForm` function:

```js
// STEP 2: Inject the provider script (PLACEHOLDER SRC)
kitScript.src = 'https://TODO.example.com/your-kit-embed.js'; // <-- TODO: replace
