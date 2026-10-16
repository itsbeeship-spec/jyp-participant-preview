# JYP Participant Portal — GitHub Pages ready

This folder hosts **13 static UI demo screens** for the JYP participant portal. `index.html` is the launcher page; every panel is a standalone HTML/CSS/JS file. These are **front-end prototypes**, not a real connected application.

## Publish with GitHub Pages (no command line)

1. Sign in to https://github.com and select **New repository**. For a demonstration, use a name such as `jyp-participant-preview`.
2. Extract `JYP_Participant_GitHub_Pages_Ready.zip` on your computer. **Do not upload the ZIP as a single file**.
3. Inside the newly created repo, select **Add file → Upload files**. Drag **all extracted files**, including `index.html`, into the root of the repository. Choose **Commit changes**.
4. Go to **Settings → Pages → Build and deployment**. Choose **Deploy from a branch**; select branch `main` and directory `/(root)`; click **Save**.
5. After GitHub Pages finishes publishing, open: `https://YOUR-USERNAME.github.io/jyp-participant-preview/` (replace the username and repo name if different).

`index.html` is required at the repository root for the site home page. GitHub Pages is a static host; you don't need to install React/Node or run a build for these HTML demos.

## Limitations and privacy

- The screens contain demo/placeholder data and some browser-local interactions, not a connected database or secure login.
- GitHub Pages should **not** be used for participant-identifying or private data; a Pages site may be publicly accessible even if repo visibility is restricted depending on plan/settings.
- Back-end services, individual authentication and permissions, mentor meetings, data persistence and official document issuance still need to be integrated.
- A navigation launcher is provided so each panel is reachable. The screens are not yet merged into a single shared-data application.

## Optional command-line upload

```bash
git init
git add .
git commit -m "Initial JYP participant portal prototype"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/jyp-participant-preview.git
git push -u origin main
```

## Local preview

Open `index.html` in a browser (basic UI). For more consistent navigation and browser storage, run a local server from the folder: `python -m http.server 8000` and open `http://localhost:8000`.