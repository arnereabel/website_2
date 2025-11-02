# Tech Context: Academic Project Website Template

## Technology Stack

### Frontend
- **Framework**: Vanilla HTML5/CSS3/JavaScript (ES6+)
- **Styling**: Custom CSS with responsive design
- **Build Tool**: None required (static site)
- **Testing**: Manual testing, browser dev tools

### Backend
- **Language**: None (static site)
- **Framework**: None
- **API Type**: None
- **Authentication**: None
- **Testing**: None

### Database
- **Primary DB**: None (static content)
- **Caching**: Browser caching
- **ORM/ODM**: None
- **Migration Tool**: None

### Infrastructure
- **Hosting**: GitHub Pages
- **Container**: None
- **CI/CD**: GitHub Actions (optional)
- **Monitoring**: None

## Development Setup

### Prerequisites
- **Runtime**: Modern web browser
- **Package Manager**: None
- **Database**: None
- **Other Tools**: Text editor, Git

### Installation Steps
1. Clone repository: `git clone https://github.com/arnereabel/website_2`
2. Open index.html in browser or serve locally
3. Edit HTML/CSS/JS files directly
4. Commit and push changes

### Environment Variables
None required - static site

## Development Workflow

### Branch Strategy
- **main/master**: Production-ready code
- **develop**: Integration branch (optional)
- **feature/***: New features
- **customization/***: Site customizations

### Code Standards
- **Linting**: None
- **Formatting**: Manual formatting
- **Pre-commit Hooks**: None
- **Code Review**: Self-review

### Testing Strategy
- **Unit Tests**: None
- **Integration Tests**: Manual browser testing
- **E2E Tests**: Manual testing across devices
- **Performance Tests**: Manual load testing

## Dependencies

### Core Dependencies
None - vanilla web technologies

### Dev Dependencies
None

### Security Considerations
- **Dependency Scanning**: None required
- **Update Policy**: Keep browser compatibility
- **Known Vulnerabilities**: None

## API Documentation

### Endpoints Overview
None - static site

### Authentication
None

### Rate Limiting
None

## Deployment

### Build Process
1. Edit HTML/CSS/JS files
2. Test in browser
3. Commit changes
4. Push to GitHub (auto-deploys via GitHub Pages)

### Deployment Checklist
- [ ] Content updated in index.html
- [ ] Images optimized and in static/ folder
- [ ] Links tested and working
- [ ] Mobile responsiveness verified
- [ ] SEO meta tags updated

### Rollback Procedure
1. Revert commits in Git
2. Push reverted changes
3. GitHub Pages updates automatically

## Troubleshooting

### Common Issues
1. **Issue**: Images not loading
   - **Cause**: Incorrect paths in HTML
   - **Solution**: Use relative paths from index.html

2. **Issue**: Mobile layout broken
   - **Cause**: CSS media queries not working
   - **Solution**: Test with browser dev tools responsive mode

### Debug Tools
- **Logging**: Browser console
- **Debugging**: Browser dev tools
- **Profiling**: Browser performance tab

### Support Contacts
- **Technical Lead**: Template maintainer
- **GitHub Support**: GitHub Pages documentation
