# Saurabh Chikhlonde — Portfolio

A responsive, multi-page personal portfolio for an embedded software developer. Built with HTML, CSS, and vanilla JavaScript; no build step or package installation is required.

## Pages

- `index.html` — Animated landing page
- `about.html` — Profile, bio, interests, and dynamically calculated Honeywell experience
- `skills.html` — Embedded development, communication protocols, and tools
- `projects.html` — Selected projects linking to their GitHub repositories
- `experience.html` — Current role and dynamically calculated tenure
- `contact.html` — Contact details, social links, and a Formspree contact form

## Local preview

Open `index.html` in a browser, or serve the project directory locally:

```bash
python -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000).

## Contact form

The form on `contact.html` submits using `POST` to the configured Formspree endpoint. Form delivery depends on that endpoint remaining active and the Formspree account being verified.

## Assets

- `assets/profile.jpg` — About-page profile photo
- `assets/README.md` — Asset guidance

## Deployment

This is a static site. Deploy the repository root to GitHub Pages, Netlify, Vercel, or another static hosting provider. Keep the HTML pages and `assets/` directory together so relative navigation and the profile image continue to work.

## External resources

The pages load Google Fonts and Font Awesome from their CDNs, so those resources require an internet connection.
