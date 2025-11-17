# 🚀 Portfolio Website

A modern, responsive, and fully customizable portfolio website built with HTML, CSS (Tailwind), and vanilla JavaScript. Perfect for developers, designers, and creative professionals.

## ✨ Features

- 🎨 **Modern Design** - Clean, professional, and eye-catching
- 💾 **Embedded System Theme** - Hexadecimal rain, binary streams, oscilloscope waves
- 🖥️ **Terminal Interface** - Authentic boot sequence and system status
- 📊 **Matrix Effects** - Falling hex code, scanlines, glowing borders
- 📱 **Fully Responsive** - Works perfectly on all devices
- ⚡ **Fast Performance** - Optimized for speed and SEO
- 🎭 **Smooth Animations** - Processor split, door opening, bus signals
- 📧 **Contact Form** - Ready-to-integrate contact functionality
- 🚀 **Easy Deploy** - Works on GitHub Pages, Netlify, Vercel, etc.
- ♿ **Accessible** - Built with accessibility in mind
- 🎯 **No Build Required** - Uses CDN, no complex setup needed
- ⌨️ **Keyboard Support** - Press ENTER to boot the system

## 📋 Sections

1. **Hero/Landing** - Eye-catching introduction with CTA buttons
2. **About Me** - Personal background and stats
3. **Skills** - Visual representation of your tech stack
4. **Projects** - Showcase your best work with links
5. **Experience** - Timeline of your career journey
6. **Contact** - Contact form and social links
7. **Footer** - Quick links and copyright

## 🛠️ Tech Stack

- **HTML5** - Semantic markup
- **CSS3** - Custom animations and styles
- **Tailwind CSS** - Utility-first CSS framework (via CDN)
- **JavaScript** - Vanilla JS for interactivity
- **Font Awesome** - Icons
- **Google Fonts** - Inter & Poppins fonts

## 📦 Getting Started

### 1. Customize Your Content

Open `index.html` and replace the placeholder content with your information:

- **Line 13-14**: Update meta description and keywords
- **Line 18**: Change page title
- **Line 43**: Your name/logo
- **Line 79**: Your name and title
- **Line 82**: Your tagline/subtitle
- **Line 93-100**: Update social links
- **Line 131-151**: Add your photo and bio
- **Line 204-268**: Update your skills
- **Line 280-370**: Replace with your actual projects
- **Line 432-490**: Add your work experience
- **Line 522-547**: Update contact information
- **Line 588**: Update footer text

### 2. Add Your Resume

Create a folder named `assets` and add your resume:
```
Portfolio_Website/
├── assets/
│   └── resume.pdf
├── index.html
├── styles.css
└── main.js
```

### 3. Add Project Screenshots

For project images, replace the placeholder divs:
```html
<!-- Replace this: -->
<div class="h-48 bg-gradient-to-br from-blue-500 to-purple-600">
    <!-- Placeholder -->
</div>

<!-- With this: -->
<img src="assets/project1.jpg" alt="Project Name" class="h-48 w-full object-cover">
```

### 4. Test Locally

Simply open `index.html` in your browser. No server required!

Or use a simple local server:
```bash
# Python 3
python -m http.server 8000

# Node.js (with npx)
npx serve

# VS Code - Install "Live Server" extension and click "Go Live"
```

Visit: `http://localhost:8000`

## 🌐 Deployment

### GitHub Pages (Recommended)

1. Create a new repository on GitHub
2. Push your code:
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/yourusername/portfolio.git
git push -u origin main
```

3. Go to Settings → Pages
4. Select `main` branch → `/ (root)` → Save
5. Your site will be live at: `https://yourusername.github.io/portfolio/`

### Netlify

1. Sign up at [netlify.com](https://netlify.com)
2. Drag and drop your project folder
3. Done! Your site is live with auto-deploy on updates

**Or use Git:**
```bash
# Install Netlify CLI
npm install -g netlify-cli

# Deploy
netlify deploy --prod
```

### Vercel

1. Sign up at [vercel.com](https://vercel.com)
2. Import your GitHub repository
3. Deploy with one click

**Or use CLI:**
```bash
# Install Vercel CLI
npm install -g vercel

# Deploy
vercel --prod
```

### Cloudflare Pages

1. Sign up at [pages.cloudflare.com](https://pages.cloudflare.com)
2. Connect your GitHub repository
3. Deploy automatically

## 📧 Contact Form Setup

The contact form needs a backend to work. Here are your options:

### Option 1: Web3Forms (Free, Recommended)
1. Get free API key from [web3forms.com](https://web3forms.com)
2. Add hidden input to form:
```html
<input type="hidden" name="access_key" value="YOUR_ACCESS_KEY">
```
3. Update form action:
```html
<form action="https://api.web3forms.com/submit" method="POST">
```

### Option 2: Formspree (Free)
1. Sign up at [formspree.io](https://formspree.io)
2. Update form:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

### Option 3: EmailJS
1. Sign up at [emailjs.com](https://emailjs.com)
2. Follow their JavaScript integration guide
3. Update `main.js` with EmailJS code

### Option 4: Simple mailto (Temporary)
Replace the form submission handler in `main.js`:
```javascript
const mailtoLink = `mailto:your@email.com?subject=${data.subject}&body=${data.message}`;
window.location.href = mailtoLink;
```

## 🎨 Customization Guide

### Change Color Scheme

Edit the gradient colors in `index.html`:
```html
<!-- Blue-Purple (default) -->
from-blue-500 to-purple-600

<!-- Change to other combinations: -->
from-green-500 to-teal-600
from-orange-500 to-red-600
from-pink-500 to-purple-600
```

### Add More Projects

Copy a project card div and modify:
```html
<div class="project-card bg-gray-900 rounded-xl...">
    <!-- Your project details -->
</div>
```

### Modify Animations

Edit `styles.css` to change animation speed:
```css
.animate-blob {
    animation: blob 7s infinite; /* Change 7s to your preference */
}
```

### Change Fonts

Replace Google Fonts link in `index.html`:
```html
<link href="https://fonts.googleapis.com/css2?family=YourFont&display=swap">
```

Update font-family in HTML classes:
```html
font-['YourFont']
```

## 📱 Responsive Breakpoints

- **Mobile**: < 768px
- **Tablet**: 768px - 1024px
- **Desktop**: > 1024px

## ♿ Accessibility Features

- Semantic HTML5 elements
- ARIA labels where needed
- Keyboard navigation support
- Focus visible indicators
- Reduced motion support
- High contrast mode support
- Screen reader friendly

## 🚀 Performance Tips

1. **Optimize Images**:
   - Use WebP format
   - Compress with [TinyPNG](https://tinypng.com)
   - Use lazy loading (already implemented)

2. **Minify Files** (for production):
   ```bash
   # Install minifiers
   npm install -g html-minifier clean-css-cli terser
   
   # Minify
   html-minifier --collapse-whitespace --remove-comments index.html -o index.min.html
   cleancss -o styles.min.css styles.css
   terser main.js -o main.min.js -c -m
   ```

3. **Use CDN for libraries** (already implemented)
4. **Enable caching** (automatic on most hosting platforms)

## 🔧 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Opera (latest)

## 📝 SEO Optimization

Already included:
- Meta tags for description and keywords
- Open Graph tags for social sharing
- Semantic HTML structure
- Fast loading time

**To improve further:**
1. Add `sitemap.xml`
2. Add `robots.txt`
3. Submit to Google Search Console
4. Add structured data (JSON-LD)

## 🐛 Troubleshooting

**Tailwind styles not loading?**
- Check internet connection (CDN requires internet)
- Verify the CDN link is correct

**Icons not showing?**
- Check Font Awesome CDN link
- Verify icon class names

**Animations not working?**
- Check if `styles.css` is linked correctly
- Clear browser cache

**Form not submitting?**
- Set up a form backend service (see Contact Form Setup)
- Check browser console for errors

## 📄 License

Free to use for personal and commercial projects. Attribution appreciated but not required.

## 🤝 Contributing

Feel free to fork, customize, and make it your own!

## 📞 Support

If you need help customizing this template:
- Open an issue on GitHub
- Check existing documentation
- Reach out via the contact form

## 🌟 Show Your Support

If you like this template, give it a ⭐️ on GitHub!

---

**Made with ❤️ by Your Name**

*Last updated: November 2025*
