# Publish PostFrame BidPro with GitHub Pages

## Create the repository

1. Sign in at GitHub.
2. Select **New repository**.
3. Name it `postframe-bidpro`.
4. Choose **Public** unless your GitHub plan supports private Pages and you prefer that.
5. Do not add a README, license, or `.gitignore` during repository creation.
6. Select **Create repository**.

## Upload this package

1. Unzip `PostFrame-BidPro-GitHub.zip` on your computer.
2. Open the new GitHub repository.
3. Choose **Add file → Upload files**.
4. Drag every file and folder from inside the unzipped folder into GitHub. Upload the contents, not the outer folder.
5. Confirm that these appear at the repository root:
   - `index.html`
   - `manifest.webmanifest`
   - `service-worker.js`
   - `icons/`
   - `.github/workflows/deploy-pages.yml`
6. Commit the files to the `main` branch.

Note: GitHub’s browser uploader may hide files beginning with a dot in some file pickers. The important hidden items are `.github` and `.nojekyll`. If they do not upload, use GitHub Desktop as described below.

## Enable GitHub Pages

1. Open **Settings → Pages** in the repository.
2. Under **Build and deployment**, set **Source** to **GitHub Actions**.
3. Open the **Actions** tab.
4. Wait for **Deploy PostFrame BidPro to GitHub Pages** to finish successfully.
5. Return to **Settings → Pages** to find the published address.

The address will normally look like:

`https://YOUR-GITHUB-USERNAME.github.io/postframe-bidpro/`

## Easier upload option: GitHub Desktop

GitHub Desktop is the most reliable way to upload hidden workflow files.

1. Install GitHub Desktop and sign in.
2. Clone the empty `postframe-bidpro` repository.
3. Copy all files from this package into the cloned repository folder.
4. In GitHub Desktop, enter a summary such as `Initial PostFrame BidPro PWA`.
5. Select **Commit to main**, then **Push origin**.
6. Enable GitHub Pages using the steps above.

## Install on iPhone

1. Open the published GitHub Pages address in Safari.
2. Tap **Share**.
3. Tap **Add to Home Screen**.
4. Enable **Open as Web App** if displayed.
5. Tap **Add**.

## Install on a computer

- Chrome or Edge: open the site and use the install icon in the address bar or **Menu → Install PostFrame BidPro**.
- Safari on Mac: use **File → Add to Dock**.

## Update the app later

Replace the repository files with the newer version and commit to `main`. GitHub Actions republishes the app automatically at the same address.

Because the PWA uses a service worker, an installed device may briefly show the prior version. Close and reopen the app, or refresh the site in Safari/Chrome after a deployment.
