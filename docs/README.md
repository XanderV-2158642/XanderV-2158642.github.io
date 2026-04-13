# Xander Vaes Blog

Personal portfolio and blog site built with Jekyll, hosted on GitHub Pages.

## Overview

- **Author**: Xander Vaes
- **Domain**: xanderv-2158642.github.io
- **Tech Stack**: Jekyll, Sass, GitHub Pages

## Site Structure

```
├── _config.yml          # Site configuration
├── _layouts/            # Page layouts
├── _includes/           # Reusable components
├── _sass/               # Sass stylesheets
├── _projects/           # Project pages (jekyll collections)
├── assets/              # Images, fonts, CSS
├── docs/                # Documentation
├── index.md             # Home page
├── about.md             # About page
└── projects.md          # Projects listing
```

## Configuration

Key settings in `_config.yml`:
- `title`: Site author name
- `url`: Production domain
- `domain`: GitHub Pages domain
- `collections.projects`: Project collection with permalink `/projects/:name/`

## Running Locally

```bash
bundle install
bundle exec jekyll serve
```

## Projects

| Project | Description |
|---------|-------------|
| SOLDAR | Collaborative robot + AR for PCB prototyping |
| WhatTheFund | LLM ETF explaining platform |
| ZupaSlica | STL slicer for 3D printing |

## Social Links

- GitHub
- LinkedIn
- Orcid