# Category and Tag System Implementation

I've standardized the category and tag system in the Jekyll theme to ensure consistent functionality across all pages.

## Changes Made:

### Directory Structure:
1. Created `categories/` directory for category pages using `.md` files
2. Renamed `tag/` to `tags/` and updated to use `.md` files for consistency

### File Formatting:
1. Standardized permalink structure:
   - Categories: `/categories/category-name/`
   - Tags: `/tags/tag-name/`

2. Used proper front matter:
```yaml
---
layout: category
category: "Category Name"
permalink: /categories/category-name/
---
```

### Link Updates:
1. Updated all category links to point to:
   - `/categories/[category-name]/`

2. Updated all tag links to point to:
   - `/tags/[tag-name]/`

3. Added proper URL slugify filter to convert spaces and special characters in URLs:
   - `{{ tag | downcase | slugify }}`

### Template Updates:
1. Updated all layouts to use the new URL structure:
   - `blog.html`
   - `_layouts/post.html`
   - `_layouts/category.html`
   - `_layouts/tag.html`

## Benefits:

1. **Consistency** - All category and tag pages now use the same URL structure
2. **Better URL Formatting** - URLs are properly slugified for better SEO and compatibility
3. **Maintainability** - Standard approach makes it easier to add new categories and tags
4. **Better Organization** - Files organized in logical directories

## How to Add New Categories/Tags:

When creating a new blog post with a new category or tag, simply add a corresponding file:

1. For a new category "Home Decor":
```yaml
---
layout: category
category: "Home Decor"
permalink: /categories/home-decor/
---
```

2. For a new tag "painting techniques":
```yaml
---
layout: tag
tag: "painting techniques"
permalink: /tags/painting-techniques/
---
```

These files ensure that clicking on the category or tag links will take users to a properly formatted page with relevant posts.
