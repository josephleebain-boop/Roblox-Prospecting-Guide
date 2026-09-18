# Prospecting Build Guide

A Vue 3 + TypeScript reference site for Roblox Prospecting. It includes stage-based Luck, Size and Sell builds, museum targets, and an Ore Finder with the top farming locations and estimated Luck targets.

## Publish using only your browser

You do **not** need Node.js, Git, VS Code or a terminal.

1. Download and extract the ZIP provided by ChatGPT.
2. Sign in to [GitHub](https://github.com) and create a new repository.
3. Name it something like `prospecting-build-guide` and make it **Public**.
4. Open the empty repository and choose **uploading an existing file**.
5. Drag **all files and folders inside** the extracted project into GitHub. Include the hidden `.github` folder.
6. Commit the files to the `main` branch.
7. Open **Settings → Pages**.
8. Under **Build and deployment → Source**, select **GitHub Actions**.
9. Open the **Actions** tab and wait for “Deploy to GitHub Pages” to finish.

Your public URL will normally be:

`https://YOUR-USERNAME.github.io/REPOSITORY-NAME/`

## Editing without development tools

- Build information: `src/data/builds.ts`
- Ore data: `src/data/ore-data.json`
- Main interface: `src/App.vue`
- Styling: `src/style.css`

On GitHub, open a file and press the pencil icon to edit it. Committing to `main` automatically republishes the site.

## Optional local development later

```bash
npm install
npm run dev
```

## Data notes

Ore locations and chances were collected from the Official Prospecting Wiki in September 2026. Recommended Luck estimates a 50% cumulative chance using the best listed base location and the Wiki's reroll description. Individual minerals may weaken or ignore Luck, so the estimate is a comparison target rather than a guarantee.
