# nalako-src

Sources for nalako.de, built with Hugo using the Parsa theme and deployed automatically via GitHub Actions.

## Overview

This repository contains the source code for the Nalako.de personal blog, built with:

- **[Hugo](https://gohugo.io/)** - Fast and flexible static site generator
- **[Parsa Theme](https://github.com/gethugothemes/parsa-hugo)** - Beautiful, responsive blog theme
- **GitHub Actions** - Automated building and deployment
- **GitHub Pages** - Static site hosting

## Local Development

### Prerequisites

- [Hugo](https://gohugo.io/getting-started/installing/) (v0.121.1 or later)
- Git

### Setup

1. Clone the repository with submodules:
   ```bash
   git clone --recurse-submodules https://github.com/nalako-de/nalako-src.git
   cd nalako-src
   ```

2. Start the development server:
   ```bash
   hugo server --buildDrafts
   ```

3. Open your browser to http://localhost:1313/nalako-src/

### Creating Content

- Create a new blog post: `hugo new posts/my-post.md`
- Create a new page: `hugo new my-page.md`
- All content is written in Markdown format

## Deployment

The site is automatically built and deployed to GitHub Pages when changes are pushed to the `main` branch. The deployment process:

1. GitHub Actions triggers on push to main
2. Hugo builds the static site
3. The built site is deployed to the `gh-pages` branch
4. GitHub Pages serves the site from the `gh-pages` branch

## Theme

This site uses the [Parsa Hugo theme](https://github.com/gethugothemes/parsa-hugo) as a git submodule. The theme provides:

- Responsive design
- Blog functionality
- Search functionality
- Social media integration
- Contact forms
- Multiple layout options

## Configuration

The main site configuration is in `hugo.toml`. Additional configuration files are in the `config/_default/` directory:

- `menus.en.toml` - Site navigation
- Other theme-specific configurations

## License

The content of this project is licensed under the [MIT License](LICENSE), and the underlying source code used to format and display that content is also licensed under the [MIT License](LICENSE).
