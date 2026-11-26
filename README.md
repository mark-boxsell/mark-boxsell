# Mark Boxsell — Portfolio

A lightweight, responsive personal portfolio built with plain HTML, CSS, and JavaScript. It has no build step or package dependencies and is published to GitHub Pages by GitHub Actions.

## Preview locally

Open `index.html` in a browser, or start a local static server from the repository root:

```sh
python3 -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000).

## Make it yours

All site content lives in `index.html`. Update the introduction, About copy, project cards, and contact link to reflect your own details. The current external links point to the `mark-boxsell` GitHub profile and repositories; replace them if you change the portfolio owner.

- Edit the page title and description in the document `<head>` for search and sharing previews.
- Update the project names, descriptions, labels, and destinations in the Work section.
- Change the contact button to your preferred public contact method.
- Adjust colors, typography, spacing, and responsive breakpoints in `styles.css`.
- The mobile navigation behavior and automatically updated footer year are in `script.js`.
- Replace `favicon.svg` to use a different browser-tab icon.

The page uses Google Fonts when a network connection is available and falls back to system sans-serif fonts if it is not.

## Deploy to GitHub Pages

The workflow at `.github/workflows/deploy.yml` deploys the repository root whenever a commit is pushed to `main`. It can also be started manually from the repository’s **Actions** tab.

1. Push this repository to GitHub and make sure the branch is named `main`.
2. In the repository, open **Settings → Pages** and set the build and deployment source to **GitHub Actions**.
3. Push a commit to `main`, or run **Deploy to GitHub Pages** from **Actions → Deploy to GitHub Pages → Run workflow**.
4. Follow the workflow run to its deployment step. Once complete, the site URL is shown in the `github-pages` deployment environment and in **Settings → Pages**.

The workflow uses the official Pages actions with read-only repository contents permission, Pages deployment permission, and an OIDC token for deployment. No access token or secret needs to be added.

## Check changes

There is no build or test toolchain to install. Before publishing, preview the page at desktop and mobile widths, follow the navigation and project links, and check the workflow run in **Actions**.
