# Smart Measure — GitHub Pages

## Deploy
1. Create a GitHub repository.
2. Upload **all files in this folder** to the repository root.
3. Commit to the branch you want to publish (normally `main`).
4. GitHub → **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select `main` and `/ (root)`, then Save.
7. Open the generated GitHub Pages URL.

## Important
- Keep `index.html`, `manifest.webmanifest`, and `sw.js` together in the published folder.
- This build uses **relative paths** (`./`) so it works with GitHub **project Pages** URLs such as:
  `https://username.github.io/repository-name/`
- No server, Node.js, database, CDN, or API is required.
- The first visit needs internet so GitHub Pages can load the app and the service worker can cache it. After that, previously cached app resources can work offline.
- If an old version remains after an update, close/reopen the site or unregister the old service worker once in browser site settings, then reload.
