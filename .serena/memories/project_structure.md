
# Project Structure

The current project follows a typical HTML template structure:

```
/
├── css/                   # CSS stylesheets
│   ├── bootstrap.min.css  # Bootstrap framework CSS
│   └── style.css          # Custom styles
├── img/                   # Image assets
├── js/                    # JavaScript files
│   └── main.js            # Main JavaScript functionality
├── lib/                   # External libraries
│   ├── easing/            # jQuery easing plugin
│   ├── owlcarousel/       # Owl Carousel for testimonials
│   └── waypoints/         # jQuery waypoints
├── scss/                  # SCSS source files
├── about.html             # About page
├── blog.html              # Blog listings page
├── contact.html           # Contact page
├── detail.html            # Blog detail page
├── index.html             # Homepage
├── service.html           # Services page
├── team.html              # Team page
├── testimonial.html       # Testimonials page
├── LICENSE.txt            # License information
└── READ-ME.txt            # README file
```

To convert to Jekyll, the structure will need to be reorganized as:

```
/
├── _includes/             # Reusable HTML components 
│   ├── header.html
│   ├── footer.html
│   ├── navbar.html
│   └── etc.
├── _layouts/              # Page layouts
│   ├── default.html
│   ├── page.html
│   └── post.html
├── _posts/                # Blog posts (Markdown files)
├── _data/                 # Data files (YAML, JSON, CSV)
├── _sass/                 # SASS partials 
├── assets/                # Static files
│   ├── css/
│   ├── js/
│   ├── img/
│   └── lib/
├── pages/                 # Site pages
├── _config.yml            # Jekyll configuration
├── index.html             # Homepage with front matter
└── Gemfile                # Ruby dependencies
```
