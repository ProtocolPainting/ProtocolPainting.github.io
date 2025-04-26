# Jekyll Theme Updates

## Hero Section Implementation

We've updated the Protocol Painting Jekyll theme to use a consistent hero section across all pages. This update ensures that:

1. **Consistent Design**: All pages now use the same hero section design with rounded buttons
2. **Customizable Content**: Each page can customize the hero title and description through front matter
3. **Centralized Template**: The hero section is now a reusable include file

## Changes Made

### New Files Created:
- `_includes/hero.html`: Centralized hero section template that can be included on any page

### Updated Files:
- `index.html`: Now using the hero include with custom title and description
- `about.html`: Updated to use hero include
- `service.html`: Updated to use hero include
- `contact.html`: Updated to use hero include
- `blog.html`: Updated to use hero include
- `_layouts/post.html`: Blog post layout now uses hero section
- `_layouts/tag.html`: Tag pages now use hero section
- `_layouts/category.html`: Category pages now use hero section

## Hero Section Features

The hero section now has:

1. **Rounded Pill Buttons**: As requested, using the classes `btn-secondary rounded-pill`
2. **Customizable Text**: Hero title and description can be set in each page's front matter
3. **Consistent Styling**: All pages maintain the original hero styling from the template
4. **Mobile Optimization**: Works well on mobile devices with the existing responsive styling

## Usage Instructions

To use the hero section on any page, add these front matter variables:

```yaml
---
layout: default
title: Page Title
hero_title: Custom Hero Title  # Optional, defaults to page.title
hero_description: Custom description for the hero section  # Optional, defaults to original template text
---

{% include hero.html %}

<!-- Rest of the page content -->
```

## Mobile Display

The hero section maintains the mobile-specific styling through the existing `mobile-fixes.css` file, which ensures the text remains visible against the background image on smaller screens.
