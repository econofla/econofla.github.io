# Silicon Review (Jekyll for GitHub Pages)

A Jekyll site for economic reviews focused on the silicon industry.

## Quick start

```bash
# 1) Install Ruby (3.1+ recommended). On macOS:
brew install ruby

# 2) Install Bundler
gem install bundler

# 3) Install dependencies
bundle install

# 4) Run locally with live reload at http://127.0.0.1:4000
bundle exec jekyll serve --livereload

# 5) Build static site into _site/
bundle exec jekyll build
```

## Creating a new post (as a separate file)

```bash
# Use the helper script:
bin/new_post "Title of your review"
# or manually:
# filename example: _posts/2025-09-04-wafer-prices-q3-2025.md
```

## Deploy to GitHub Pages

1. Create a new GitHub repo and push this project.
2. In **Settings → Pages**, choose **Build and deployment**: *Deploy from a branch*.
3. Select the `main` branch and `/ (root)` path.
4. GitHub will build the site using the `github-pages` gem.
5. Your site will be available at `https://<username>.github.io/<repo>` (for a project site) or `https://<username>.github.io` (for a user/organization site).

> If you prefer Actions: create `.github/workflows/jekyll.yml` with a standard Jekyll Pages workflow.
