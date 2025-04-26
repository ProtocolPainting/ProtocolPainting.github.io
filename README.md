# Protocol Painting - Jekyll Website

This repository contains the Jekyll-based website for Protocol Painting, a professional painting company.

## Getting Started

### Prerequisites

Before you can run this Jekyll site locally, you need to have Ruby and Jekyll installed:

```bash
# Install Ruby (if not already installed)
# For Windows, use RubyInstaller: https://rubyinstaller.org/

# Install Jekyll and Bundler
gem install jekyll bundler
```

### Installation

1. Clone this repository:
```bash
git clone https://github.com/yourusername/protocol-painting.git
cd protocol-painting
```

2. Install dependencies:
```bash
bundle install
```

3. Run the site locally:
```bash
bundle exec jekyll serve
```

4. Open your browser and visit `http://localhost:4000`

## Site Structure

- `_config.yml` - Site configuration
- `_includes/` - Reusable HTML components
- `_layouts/` - Page templates
- `_posts/` - Blog posts
- `_data/` - Data files for services, team members, etc.
- `_services/` - Service collection pages
- `_team/` - Team member collection pages
- `assets/` - Static files (CSS, JS, images)

## Adding Content

### Blog Posts

To add a new blog post, create a new file in the `_posts` directory following the naming convention `YYYY-MM-DD-title.md`. Add the following front matter:

```markdown
---
layout: post
title: "Your Post Title"
date: YYYY-MM-DD
author: Author Name
image: img/blog/your-image.jpg
categories: [Category1, Category2]
tags: [tag1, tag2, tag3]
---

Your content here...
```

### Services

To add a new service:

1. Add the service details to `_data/services.yml`
2. Create a new file in the `_services` directory with appropriate front matter

### Team Members

To add a new team member, add their details to `_data/team.yml`.

## License Information

This site uses the "PAINTER" template from HTML Codex, which is licensed under a Creative Commons Attribution 4.0 International License. 

**Important**: The footer attribution links must be preserved unless a Credit Removal License has been purchased from HTML Codex.

## Development Guidelines

- Follow Jekyll best practices for templating and content organization
- Use Liquid templating language for dynamic content
- Keep configuration settings in `_config.yml`
- Follow BEM methodology for CSS class naming
- Test all changes locally before deployment

## Deployment

The site can be deployed to any static hosting platform like GitHub Pages, Netlify, or Vercel.

For GitHub Pages:

```bash
bundle exec jekyll build
# Commit and push the changes to your repository
```

For other platforms, follow their respective deployment instructions.
