# RepoSpace — GitHub Portfolio Explorer

A responsive static demo website for showcasing public GitHub repositories. It loads repository metadata using GitHub's public API, and lets visitors search/sort projects, browse files, preview supported text files, open source files on GitHub, and download repository ZIPs or individual files.

## Run locally
Open `index.html` in a modern browser and enter a GitHub username. Internet access is needed because repository data comes from GitHub.

## Publish with GitHub Pages
1. Create a public repository, for example `repospace-portfolio`.
2. Upload `index.html` and `README.md` to the repository root.
3. Open **Settings → Pages**.
4. Choose **Deploy from a branch**, select `main` and `/(root)`, then save.
5. Wait for deployment; GitHub Pages will show the published URL.

For an account-level URL, name the repository `<your-username>.github.io`. A project site normally uses `https://<username>.github.io/<repository-name>/`.

## Default profile
The page automatically loads the public repositories for `ganeshpappala`. To explore another profile, append `?user=OTHER_USERNAME` to the website URL.

## Limitations and safety
- This demo only shows public repositories. It does not access private repositories.
- Unauthenticated GitHub API requests have rate limits; wait and retry if one is reached.
- Very large repositories may return a partial file tree; use the GitHub link to browse all files.
- Binary and large files may not preview, but can be opened/downloaded.
- Never place access tokens, passwords, or private files in a GitHub Pages website. Pages content is public.
- Static GitHub Pages does not provide a secure server-side layer for private repository access.

## Official documentation
- https://docs.github.com/en/pages
- https://docs.github.com/en/rest
