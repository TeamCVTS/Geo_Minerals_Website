Geo Minerals Website - Developer Documentation

Overview
========
Single-page responsive website built with vanilla HTML5, CSS3, and JavaScript. No frameworks or build tools. Optimized for desktop and mobile (responsive navbar with hamburger menu).

File Structure
==============
- index.html          : Main HTML file (all content, sections, JS)
- style.css           : All styles (CSS variables, responsive design)
- CNAME               : Custom domain config (GitHub Pages)
- images/             : Assets (logo, hero bg, section images)

Key Features
============
- Fixed responsive navbar: Desktop horizontal menu, mobile hamburger (≤768px)
- Smooth scrolling sections (#home, #about, etc.)
- Hero with overlay/gradient
- CSS animations (fadeInUp)
- Mobile-first responsive grid/flexbox
- SEO-friendly (meta viewport, title, semantic HTML)

Navbar Responsiveness
=====================
HTML: .navbar > .nav-container (.logo + .hamburger + .nav-menu ul)
CSS: 
  - Desktop: .nav-menu { display: flex; horizontal }
  - @media (max-width: 768px): .hamburger { display: flex }, .nav-menu slides down as overlay
JS: Toggle 'active' class on hamburger click (body click closes)

JavaScript (inline in index.html)
==================================
- DOMContentLoaded event
- Hamburger toggle: .nav-menu.classList.toggle('active'), prevents body close interference

Customization Guide
===================
1. Colors: Edit CSS :root variables (--primary-dark, --accent-gold, etc.)
2. Logo: Replace images/Geo Minerals-2 1.png (60px height)
3. Content: Edit sections in index.html (#about p, #contact phone, etc.)
4. Hero BG: images/hero-mining.png
5. Add section: Copy .section structure, add id/link to nav
6. Media queries: @media (max-width: 768px)/480px/1024px

Sections Structure
==================
- Navbar (fixed)
- #home (hero)
- #about (about + layout)
- #experience (experience)
- #value (features grid)
- #contact
- Footer

Deployment
==========
- Static site: Open index.html or host (GitHub Pages/Netlify)
- Edit & preview: Live Server VSCode extension

Images (optimize before replace):
- hero-mining.png (hero bg)
- mineral-processing.png (about)
- mining-team.png (experience)
- chrome-sand.png (value bg)
- mineral-texture.png (experience bg overlay)

Last Updated: Current version fully responsive, mobile-tested.

