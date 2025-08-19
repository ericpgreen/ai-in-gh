# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static website for a Duke University FOCUS Program course called "AI in Global Health." The repository contains a single-page HTML website that serves as the course syllabus and information portal.

## Project Structure

```
/
├── README.md                # Basic project identifier  
├── index.html              # Main course website (self-contained)
├── dghi-logo.png           # Duke Global Health Institute logo
└── dghi-logo-white.png     # White version of DGHI logo
```

## Technology Stack

- **Frontend**: Pure HTML5 with embedded CSS and JavaScript
- **Styling**: CSS Grid, Flexbox, CSS custom properties (CSS variables)
- **JavaScript**: Vanilla JS for interactive elements
- **Deployment**: Static hosting (GitHub Pages based on git commits)

## Key Features

The website includes:
- Responsive course syllabus with Duke University branding
- Interactive timeline with modal popups for detailed weekly schedules
- Animated hero section with floating blob effects
- Mobile-responsive navigation with hamburger menu
- Scroll-triggered reveal animations
- Course information, grading breakdown, and tool showcase

## Development Workflow

### Making Changes

1. **Direct editing**: Modify `index.html` directly for content updates
2. **Testing**: Open `index.html` in a web browser to preview changes
3. **Images**: Replace logo files as needed (maintain aspect ratios)

### Common Tasks

**Updating course content:**
- Edit text content directly in the HTML
- Modify the `weekDetails` JavaScript object for schedule changes
- Update CSS custom properties in `:root` for color scheme changes

**Content sections to update:**
- Course details and dates (lines ~1170-1180)
- Weekly schedule content (JavaScript object starting ~1445)
- Assignment percentages and descriptions (lines ~1265-1310)
- Tool showcase items (lines ~1378-1410)

### Deployment

The site is deployed via GitHub Pages. Changes pushed to the main branch will automatically update the live site.

### Styling Notes

- Uses Duke University brand colors defined as CSS custom properties
- Responsive breakpoints: 1024px, 768px, 480px
- Key color variables: `--duke-navy`, `--duke-royal`, `--eno`, `--persimmon`
- Animation classes: `.reveal` for scroll-triggered animations

### Browser Compatibility

The site uses modern CSS features (Grid, Flexbox, custom properties) and should work in all current browsers. No build process or transpilation required.