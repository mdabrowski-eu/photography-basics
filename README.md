# Photography Basics Website

This repository contains a Hugo site based on the **Book** theme. It gathers all notes about the basics of photography and splits them into separate chapters.

## Local development

1. Install [Hugo](https://gohugo.io/) with extended support.
2. Fetch the Book theme:

```bash
git submodule add https://github.com/alex-shpak/hugo-book.git site/themes/hugo-book
```

3. Build the site locally:

```bash
hugo server -s site
```

## Deployment

The repository includes a GitHub Actions workflow that builds the Hugo site and publishes it to GitHub Pages. Push changes to the `main` branch and GitHub will deploy the site automatically.
