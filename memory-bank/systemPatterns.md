# System Patterns: Academic Project Website Template

## Architecture Overview
```
Browser
    ↓
index.html (Single Page Application)
    ↓
static/
├── css/     # Stylesheets
├── js/      # JavaScript files
└── images/  # Media assets
```

## Core Design Patterns

### Component-Based HTML Structure
- **Purpose**: Organize content into reusable, semantic sections
- **Implementation**: HTML5 semantic elements with CSS classes for styling
- **Example**:
  ```html
  <section class="hero">
    <div class="container">
      <h1>Project Title</h1>
      <p>Description</p>
    </div>
  </section>
  ```
- **Benefits**: Maintainable, accessible, SEO-friendly
- **Trade-offs**: No dynamic component reuse

### Responsive CSS Grid/Flexbox
- **Purpose**: Create mobile-first responsive layouts
- **Implementation**: CSS Grid and Flexbox with media queries
- **Example**:
  ```css
  .container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  }
  ```
- **Benefits**: Flexible layouts that work on all devices
- **Trade-offs**: Browser compatibility considerations

## Component Relationships

### Static Asset Loading
- **Communication**: Direct file references in HTML
- **Data Format**: Standard web formats (JPEG, PNG, MP4, PDF)
- **Error Handling**: Browser handles missing assets gracefully

## Critical Implementation Paths

### Page Load Flow
1. HTML document loads
2. CSS stylesheets apply
3. JavaScript initializes interactive components
4. Images and media load progressively
5. Page becomes fully interactive

### Media Loading Strategy
1. Lazy load images below fold
2. Progressive loading for videos
3. PDF viewer initialization
4. Carousel component setup

## Performance Considerations

### Caching Strategy
- **Browser Cache**: Static assets cached via HTTP headers
- **CDN**: GitHub Pages provides global CDN
- **Invalidation**: Cache busting via file versioning

### Optimization Techniques
- Image compression and responsive images
- Minified CSS and JavaScript
- Lazy loading for media content
- Optimized font loading

### Bottlenecks & Solutions
- **Large Images**: → **Solution**: Compress and use responsive images
- **Slow Loading PDFs**: → **Solution**: Lazy load PDF viewer
- **Heavy JavaScript**: → **Solution**: Defer non-critical scripts

## Security Patterns

### Content Security Policy
- **Method**: None (static site)
- **Storage**: N/A
- **Refresh Strategy**: N/A

### Data Protection
- **Encryption at Rest**: N/A (public content)
- **Encryption in Transit**: HTTPS via GitHub Pages
- **Sensitive Data Handling**: None

## Deployment Architecture

### Environment Structure
- **Development**: Local file system with browser
- **Production**: GitHub Pages hosting

### CI/CD Pipeline
1. Edit files locally
2. Test in browser
3. Commit to Git repository
4. Push to GitHub (triggers Pages deployment)

### Monitoring & Logging
- **Application Logs**: Browser console
- **Performance Metrics**: Browser dev tools
- **Alerts**: Manual monitoring

## Code Organization

### Directory Structure
```
website_nerfies/
├── index.html          # Main page
├── memory-bank/        # Documentation
├── static/
│   ├── css/           # Stylesheets
│   ├── js/            # JavaScript
│   └── images/        # Media assets
├── .git/              # Version control
├── .nojekyll          # GitHub Pages config
└── README.md          # Documentation
```

### Naming Conventions
- **Files**: kebab-case (e.g., project-image.jpg)
- **CSS Classes**: kebab-case (e.g., hero-section)
- **JavaScript**: camelCase for variables/functions
- **IDs**: camelCase for unique elements

### Module Boundaries
- **Core**: index.html and essential styles
- **Features**: Individual sections (hero, abstract, etc.)
- **Shared**: Common utilities and components
