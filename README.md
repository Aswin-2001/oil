# Suprakan Foods

Static storefront for Suprakan Foods.

## Publish with GitHub Pages

1. Create a new repository on GitHub. It can be public or private (private-repository Pages availability depends on your GitHub plan).
2. In the GitHub repository, open **Settings → Pages** and set **Build and deployment → Source** to **GitHub Actions**.
3. Add that repository as this repository's `origin` and push the `main` branch:

   ```sh
   git remote add origin https://github.com/<YOUR-USERNAME>/<YOUR-REPOSITORY>.git
   git add index.html README.md .github/workflows/pages.yml
   git commit -m "Prepare site for GitHub Pages"
   git push -u origin main
   ```

   If `origin` already exists, use `git remote set-url origin ...` instead.
4. The workflow deploys the site on pushes to `main`. Once it completes, the Pages settings show the published URL.

## Important

This is a static, browser-only site. Cart, admin settings, and order data are stored in the visitor's browser; they are not shared with the store or other visitors. GitHub Pages does not provide a backend or secure admin system. Do not treat the built-in admin area as secure or use this as a live order-processing system without adding a suitable backend.
