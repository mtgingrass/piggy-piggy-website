# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static marketing website for the Piggy-Piggy iOS app - a financial tracking app designed to help you manage your savings goals and track your spending habits. The website is built with pure HTML/CSS and deployed on Netlify.

## Technology Stack

- **Frontend**: Pure HTML5 and CSS3 (no JavaScript frameworks)
- **Fonts**: Google Fonts (Inter font family)
- **Deployment**: Netlify static hosting
- **No build process**: Direct HTML/CSS files served statically

## Key Files and Structure

- `index.html` - Main landing page with hero section, features, screenshot gallery, and app details
- `privacy.html` - Privacy policy page 
- `styles.css` - Complete styling (638 lines) with modern CSS features (Grid, Flexbox, custom properties)
- `netlify.toml` - Deployment configuration with security headers, cache rules, and URL redirects
- `images/iOS Phones 6.9/` - Contains 3 app screenshots (01.png, 02.png, 03.png)

## Development Workflow

### Local Development
```bash
# No build process needed - simply open in browser
open index.html
```

### Testing Changes
- Open `index.html` in browser to view changes
- Test responsive design across different screen sizes
- Verify all links work correctly (developer website, privacy policy)

### Deployment
- Automatic deployment via Netlify when pushing to main branch
- No build command needed (static site)
- Security headers and cache optimization configured in `netlify.toml`

## Code Architecture

### HTML Structure
- Semantic HTML5 markup
- SEO-optimized with proper meta tags
- Responsive design with mobile-first approach
- App Store integration placeholder (app not yet published)

### CSS Organization
- Single `styles.css` file contains all styling
- CSS custom properties for consistent theming
- Modern layout techniques (CSS Grid for feature sections, Flexbox for components)
- Smooth animations and hover effects
- Horizontal scrolling screenshot gallery

### Key Design Patterns
- **Hero Section**: App branding with download CTA
- **Feature Grid**: 2x2 grid layout showcasing app features
- **Screenshot Gallery**: Horizontal scrolling with CSS scroll-snap
- **Responsive Design**: Mobile-first with breakpoints for tablet/desktop

## Important Configuration

### Netlify Redirects
- `/app-store` → Placeholder (app not yet published)
- `/developer` → Developer website (301 redirect)

### Security Headers
- X-Frame-Options: DENY
- X-XSS-Protection: 1; mode=block
- X-Content-Type-Options: nosniff
- Referrer-Policy: strict-origin-when-cross-origin

### Cache Control
- Static assets (CSS, JS, images) cached for 1 year
- HTML files use default cache settings

## App Information Context

When making changes, keep in mind this promotes:
- **App Name**: Piggy-Piggy
- **Platform**: iOS (requires iOS 15.0+)
- **Purpose**: Financial tracking app for managing savings goals and spending habits
- **Key Features**: Track daily expenses, visual tracking, savings goals, simple design
- **Target Audience**: Parents managing children's money, individuals tracking personal expenses
- **Developer**: Mark Gingrass
- **Status**: In development (not yet published to App Store)

## Editing Guidelines

- Maintain the clean, professional design aesthetic
- Keep content focused on the app's financial tracking value proposition
- Ensure all changes are responsive across devices
- Test placeholder links after any URL changes
- Preserve the horizontal screenshot gallery functionality (currently shows 3 screenshots)
- Maintain SEO optimization with proper meta tags
- Update App Store links once the app is published