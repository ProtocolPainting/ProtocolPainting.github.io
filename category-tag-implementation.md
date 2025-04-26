# Category and Tag Pages Implementation

In Jekyll, there are two main approaches to handling category and tag pages:

## Option 1: Using Jekyll Plugins (jekyll-archives)

This approach automatically generates pages for categories and tags:

1. Add to `Gemfile`:
```ruby
gem 'jekyll-archives'
```

2. Configure in `_config.yml`:
```yaml
plugins:
  - jekyll-archives

jekyll-archives:
  enabled:
    - categories
    - tags
  layouts:
    category: category
    tag: tag
  permalinks:
    category: /categories/:name/
    tag: /tags/:name/
```

**Note**: This approach doesn't work on GitHub Pages due to plugin restrictions.

## Option 2: Manual Approach (what we've implemented)

This approach uses a manual file for each category/tag:

1. Create layouts: 
   - `_layouts/category.html`
   - `_layouts/tag.html`

2. Create individual files for each category/tag:
   - `categories/category-name.md`
   - `tags/tag-name.md`

3. Set front matter in each file:
```yaml
---
layout: category
category: "Category Name"
permalink: /categories/category-name/
---
```

## Usage in Blog Posts

Categories and tags are defined in each post's front matter:

```yaml
---
layout: post
title: "Post Title"
categories: [Category1, Category2]
tags: [tag1, tag2, tag3]
---
```

## Adding New Categories or Tags

When adding new categories or tags, follow these steps:

1. For a new category "Home Decor":
```yaml
# File: categories/home-decor.md
---
layout: category
category: "Home Decor"
permalink: /categories/home-decor/
---
```

2. For a new tag "painting techniques":
```yaml
# File: tags/painting-techniques.md
---
layout: tag
tag: "painting techniques"
permalink: /tags/painting-techniques/
---
```

## Recommendation

The manual approach is most reliable for GitHub Pages and other Jekyll hosting platforms with restricted plugin access.