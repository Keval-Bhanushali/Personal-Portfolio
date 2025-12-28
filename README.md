# Keval Bhanushali — Personal Portfolio

This repository contains a one-page personal portfolio website built with HTML, CSS and a small amount of JavaScript. It's designed to be served from a static web server (for example, XAMPP's Apache) and showcases projects, experience, education, contact details and client logos.

## Key Features
- Responsive, modern one-page layout
- Animated elements using Wow.js / Animate.css
- Client logos strip that auto-centers and scales logos
- Small UX niceties: "Read more" toggle for long paragraphs and an auto-updating footer year

## Tech Stack
- HTML5, CSS3, Bootstrap 5
- Vanilla JavaScript for small UI behaviors
- Libraries: Wow.js, GSAP, Isotope, Magnific Popup, Slick, Remix Icons

## Local Setup (XAMPP / Apache)
1. Copy this folder into your XAMPP `htdocs` directory (already present at `/Applications/XAMPP/xamppfiles/htdocs/Personal-Portfolio`).
2. Start Apache from XAMPP control panel.
3. Visit the site in your browser at:

   http://localhost/Personal-Portfolio/

Note: You can also open `index.html` directly in a browser for static previews, but features relying on server paths or CORS may behave differently.

## Notable Implementation Details
- Footer year: dynamically set via `document.getElementById('currentYear').textContent = new Date().getFullYear()` so the copyright year updates automatically.
- Education paragraph: a CSS clamp + small JS toggle implements a "Read more / Show less" behavior to keep the resume section compact.
- Client logos: the `client-logo-wrap` styles center the logo group and `center-logo` class marks the emphasized logo (adjust sizes in the inline styles or move to `assets/css/style.css`).

## Project Structure
```
Personal-Portfolio/
├─ assets/
│  ├─ css/      # styles (style.css, responsive.css, etc.)
│  ├─ js/       # scripts (script.js and libraries)
│  ├─ images/   # images, logos, profile picture
├─ index.html
├─ README.md
```

## How to edit content
- Open `index.html` in your editor and update sections under `#about`, `#resume`, `#works`, and `#contact`.
- Client logos are located in `assets/images/client-logos/` — add/remove images and, if you want the center emphasis, add the `center-logo` class to the desired `<a class="client-logo-item">` element.

## Contact
- Email: mrbhanushali03@gmail.com
- Phone: +91 7567565368

---

If you want, I can:
- Move the small inline styles/scripts into `assets/css/style.css` and `assets/js/script.js`.
- Update the README with live-deployment instructions (Netlify/Vercel) or add a LICENSE file.