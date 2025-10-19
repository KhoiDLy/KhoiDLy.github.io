# KhoiDLy.github.io Brownfield Architecture Document

## Introduction

This document captures the CURRENT STATE of the KhoiDLy.github.io codebase, including technical debt, workarounds, and real-world patterns. It serves as a reference for AI agents working on enhancements to this Jekyll-based academic portfolio website.

### Document Scope

Comprehensive documentation of entire Jekyll-based personal academic website system.

### Change Log

| Date   | Version | Description                 | Author    |
| ------ | ------- | --------------------------- | --------- |
| 2024-12-19 | 1.0     | Initial brownfield analysis | Winston (Architect) |

## Quick Reference - Key Files and Entry Points

### Critical Files for Understanding the System

- **Main Entry**: `index.html` (homepage with research focus)
- **Configuration**: `_config.yml` (site-wide settings and data structure)
- **Layout System**: `_layouts/default.html` (main template)
- **Content Organization**: `_posts/` directory with categorized content
- **Data Management**: `_data/` directory with YAML files for CV content
- **Styling**: `style.css` and `_includes/css/main.css` (custom CSS with Bootstrap)
- **JavaScript**: `_includes/js.html` (jQuery, Bootstrap, custom animations)

## High Level Architecture

### Technical Summary

This is a **Jekyll-based static site generator** configured for GitHub Pages hosting. The site serves as a personal academic portfolio for Dr. Khoi Dang Ly, showcasing research in soft robotics, publications, and professional information.

### Actual Tech Stack

| Category  | Technology | Version | Notes                      |
| --------- | ---------- | ------- | -------------------------- |
| Static Site Generator | Jekyll | 4.x | GitHub Pages compatible |
| CSS Framework | Bootstrap | 4.0.0-beta | Custom modifications |
| JavaScript | jQuery | 3.2.1 | Local copies, not CDN |
| Fonts | Montserrat | Multiple weights | Local font files |
| Markdown | Kramdown | Default | With Rouge syntax highlighting |
| Hosting | GitHub Pages | N/A | Automatic deployment |

### Repository Structure Reality Check

- Type: **Monorepo** (single Jekyll site)
- Package Manager: **None** (static site, no Node.js/npm)
- Notable: **Academic focus** with research project categorization

## Source Tree and Module Organization

### Project Structure (Actual)

```text
KhoiDLy.github.io/
├── _config.yml              # Site configuration and data structure
├── _layouts/
│   └── default.html         # Main layout template
├── _includes/               # Reusable components
│   ├── css/
│   │   ├── bootstrap.min.css # Bootstrap framework
│   │   └── main.css         # Custom styling (1600+ lines)
│   ├── head.html            # HTML head section
│   ├── header.html          # Navigation and header
│   ├── portfolio.html       # Research project display
│   ├── cv.html              # CV/resume layout
│   ├── footer.html          # Site footer
│   └── js.html              # JavaScript includes
├── _data/                   # YAML data files
│   ├── cv-education.yml     # Education history
│   ├── cv-professional.yml  # Professional experience
│   ├── cv-publications.yml  # Research publications
│   ├── cv-skills.yml        # Technical skills
│   └── cv-misc.yml          # Patents, service, teaching
├── _posts/                  # Content organization
│   ├── research/            # Research projects by category
│   │   ├── Embedded power and sensor design/
│   │   ├── Embodied energy system/
│   │   ├── Integrated system and controller design/
│   │   └── Other projects/
│   ├── design/              # Design projects
│   ├── blog/                # Blog posts
│   └── cv/                  # CV-related posts
├── img/                     # Image assets
│   ├── portfolio/           # Research project images
│   ├── fav/                 # Favicon files
│   └── [other images]       # Site images
├── js/                      # JavaScript libraries
├── fonts/                   # Montserrat font family
├── papers/                  # PDF publications
└── [root files]             # HTML pages, PDFs, configs
```

### Key Modules and Their Purpose

- **Content Management**: `_posts/` directory with Jekyll's post system for research projects
- **Data Layer**: `_data/` YAML files for structured CV content
- **Layout System**: `_layouts/default.html` with conditional rendering based on page type
- **Styling System**: Custom CSS with Bootstrap integration and Montserrat fonts
- **Navigation**: Dynamic header with conditional menu items based on page type
- **Research Display**: `_includes/portfolio.html` for categorized project showcase

## Data Models and APIs

### Data Models

The site uses Jekyll's data system with YAML files:

- **CV Education**: See `_data/cv-education.yml`
- **CV Professional**: See `_data/cv-professional.yml` 
- **CV Publications**: See `_data/cv-publications.yml`
- **CV Skills**: See `_data/cv-skills.yml`
- **CV Misc**: See `_data/cv-misc.yml`

### Content Structure

- **Research Posts**: Markdown files in `_posts/research/` with front matter
- **Page Types**: Defined in `_config.yml` defaults (research, design, blog, cv, publications)
- **Subcategories**: Research projects organized by technical focus areas

## Technical Debt and Known Issues

### Critical Technical Debt

1. **Mixed Content Organization**: Research projects split between `_posts/research/` subdirectories and main `_posts/` structure
2. **Hardcoded Navigation**: Navigation logic embedded in `_includes/header.html` with complex conditionals
3. **Font Management**: Local Montserrat fonts with commented-out CDN alternatives
4. **CSS Organization**: Large `main.css` file (1600+ lines) mixing Bootstrap overrides and custom styles
5. **JavaScript Dependencies**: Local copies of jQuery/Bootstrap instead of CDN (performance vs. reliability trade-off)

### Workarounds and Gotchas

- **Page Type Logic**: Complex conditional rendering in `_layouts/default.html` based on `page.type`
- **Print Styles**: Extensive `no-print` and `only-print` classes for CV printing
- **Image Paths**: Hardcoded paths in `_includes/portfolio.html` (`img/portfolio/`)
- **Font Loading**: Custom `@font-face` declarations with specific weight mappings
- **Mobile Navigation**: Custom JavaScript for navbar collapse behavior

## Integration Points and External Dependencies

### External Services

| Service  | Purpose  | Integration Type | Key Files                      |
| -------- | -------- | ---------------- | ------------------------------ |
| GitHub Pages | Hosting | Git-based deployment | Automatic via GitHub |
| Google Analytics | Analytics | JavaScript snippet | `_includes/head.html` |
| Google Fonts | Typography | CSS import | `_includes/head.html` |
| FontAwesome | Icons | CDN | `_includes/head.html` |

### Internal Integration Points

- **Jekyll Processing**: Automatic markdown-to-HTML conversion
- **Liquid Templating**: Data binding between YAML files and HTML templates
- **GitHub Pages**: Automatic site generation and deployment
- **MathJax**: Mathematical equation rendering (conditional loading)

## Development and Deployment

### Local Development Setup

1. **Prerequisites**: Ruby, Jekyll gem
2. **Setup**: `bundle install` (if Gemfile exists) or `gem install jekyll`
3. **Development**: `jekyll serve` for local preview
4. **Known Issues**: Font paths may need adjustment for local development

### Build and Deployment Process

- **Build Command**: Automatic via GitHub Pages (no manual build required)
- **Deployment**: Git push to main branch triggers automatic rebuild
- **Environments**: Single production environment (GitHub Pages)
- **Custom Domain**: Configured via `CNAME` file

## Testing Reality

### Current Test Coverage

- **Unit Tests**: None (static site)
- **Integration Tests**: None
- **E2E Tests**: None
- **Manual Testing**: Primary QA method (visual inspection)

### Content Validation

- **Markdown Validation**: Manual review of post front matter
- **Link Checking**: Manual verification of internal/external links
- **Image Optimization**: Manual image processing and optimization

## Content Management Patterns

### Research Project Organization

- **Categorization**: Projects organized by technical focus areas
- **Front Matter**: Standardized YAML front matter for metadata
- **Image Management**: Thumbnail and full-size images in `img/portfolio/`
- **Publication Integration**: Research projects linked to publications in `_data/cv-publications.yml`

### CV Data Management

- **YAML Structure**: Structured data files for different CV sections
- **Dynamic Rendering**: Liquid templates generate HTML from YAML data
- **Print Optimization**: Special CSS classes for PDF generation
- **Skills Visualization**: Progress bars for technical skills display

## Performance Considerations

### Current Optimizations

- **Local Assets**: JavaScript and CSS files served locally (not CDN)
- **Image Optimization**: Manual image compression and sizing
- **Font Loading**: Local Montserrat fonts with multiple weights
- **Minification**: Bootstrap CSS is minified

### Performance Bottlenecks

- **Large CSS File**: `main.css` is 1600+ lines and not minified
- **Font Loading**: Multiple font weights loaded simultaneously
- **Image Loading**: No lazy loading for portfolio images
- **JavaScript**: Multiple jQuery plugins loaded on every page

## Appendix - Useful Commands and Scripts

### Frequently Used Commands

```bash
# Local development
jekyll serve                    # Start local development server
jekyll build                    # Build site locally
jekyll doctor                    # Check for common issues

# Git operations
git add .                        # Stage changes
git commit -m "message"          # Commit changes
git push origin main             # Deploy to GitHub Pages
```

### Debugging and Troubleshooting

- **Jekyll Issues**: Check `_config.yml` syntax and front matter formatting
- **CSS Problems**: Verify Bootstrap classes and custom CSS overrides
- **Image Issues**: Check file paths in `img/` directory
- **Font Problems**: Verify `@font-face` declarations in `main.css`
- **Navigation Issues**: Check `page.type` logic in templates

### Common Development Tasks

- **Adding Research Project**: Create markdown file in appropriate `_posts/research/` subdirectory
- **Updating CV**: Modify YAML files in `_data/` directory
- **Styling Changes**: Edit `_includes/css/main.css` or `style.css`
- **Navigation Updates**: Modify `_includes/header.html`
- **Content Updates**: Edit markdown files or HTML pages directly
