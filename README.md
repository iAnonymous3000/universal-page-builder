# 🧰 Universal Page Builder (JavaScript-Free)

*Inspired by [Science & Design's Page Builder](https://github.com/scidsg/page-builder)*

A modern, accessible landing page template with dark mode, SEO optimization, and responsive design - all without a single line of JavaScript. This template helps you quickly create accessible, lightweight, and privacy-first single-page websites.

## ✨ Features

- **🚫 No JavaScript Required**: Full functionality using pure HTML and CSS
- **🌗 Dark Mode Support**: Dark mode enabled by default, with automatic system preference detection
- **♿ Fully Accessible**: WCAG 2.1 AA compliant with keyboard navigation and semantic HTML
- **🔒 100% Privacy-Respecting**: No client-side scripts means no tracking possibilities
- **🔍 SEO Optimized**: Built-in meta tags and structured data
- **📱 Responsive Design**: Adapts beautifully to all screen sizes with CSS-only mobile menu
- **⚡ Ultra-Fast Performance**: Minimal code, no script loading/parsing, instant page loads
- **🖨️ Print-friendly**: Special styling for print media
- **⌨️ Keyboard Accessible**: Full keyboard navigation support with enhanced focus states
- **👁️ Reduced Motion**: Respects user preferences for reduced motion

## 🚀 Getting Started

### Quick Start

1. Fork this repository
2. Clone your repository to your local machine
3. Edit the content in `index.html` to match your needs
4. Customize colors and styles in `styles.css` as desired
5. Deploy to GitHub Pages or your preferred hosting platform

### Deployment with GitHub Pages

1. Go to your repository settings
2. Navigate to "Pages" in the sidebar
3. Under "Source", select "Deploy from a branch"
4. Choose "main" branch and "/ (root)" folder
5. Click "Save"
6. Your site will be published at https://yourusername.github.io/universal-page-builder/

## 🎨 Customization

### Colors and Theme

The template uses CSS variables for easy color customization. Edit these in the `:root` section of `styles.css`:

```css
:root {
    /* Dark mode by default */
    --bg-primary: #121212;
    --bg-secondary: #1e1e1e;
    --text-primary: #f0f0f0;
    --text-secondary: #b0b0b0;
    --accent-color: #738bff;
    /* ...more variables... */
}
```

### Content

Replace the placeholder content in `index.html` with your own:

- Update headings, paragraphs, and button text
- Replace SVG placeholders with your own images
- Modify meta tags and structured data with your information
- Update links and navigation items

## 🔄 How the JavaScript-Free Approach Works

This template implements advanced features without JavaScript:

### Dark Mode

The template uses dark mode by default and responds to system preferences:
```css
/* Dark mode by default */
:root {
    --bg-primary: #121212;
    /* Other dark mode variables... */
}

/* Light mode using media query (if needed) */
@media (prefers-color-scheme: light) {
    :root {
        --bg-primary: #ffffff;
        /* Other light mode variables... */
    }
}
```

### Mobile Menu

Implements the hamburger menu using CSS `:checked` pseudo-class:
```html
<label for="menu-toggle" class="menu-icon">
    <span class="hamburger"></span>
</label>
<input type="checkbox" id="menu-toggle" class="menu-checkbox">
<ul id="main-menu" class="main-menu"><!-- Menu items --></ul>

<!-- CSS shows/hides menu based on checkbox state -->
#menu-toggle:checked ~ .main-menu {
    display: flex;
}
```

## 📋 Accessibility Features

This template follows WCAG 2.1 AA guidelines and includes:

- Semantic HTML structure with proper landmarks
- Proper heading hierarchy
- Skip-to-content link
- Keyboard navigation support
- Focus indicators
- Color contrast compliance
- Reduced motion support
- ARIA attributes where needed

See [ACCESSIBILITY.md](https://github.com/iAnonymous3000/universal-page-builder/blob/main/ACCESSIBILITY.md) for more details.

## 🔒 Privacy Features

This template provides maximum privacy:

- No JavaScript = no tracking scripts, cookies, fingerprinting, or analytics
- No third-party requests
- Content loads directly from your server with no external dependencies
- No local storage or client-side state
- No possibility of XSS attacks via JavaScript

See [PRIVACY.md](https://github.com/iAnonymous3000/universal-page-builder/blob/main/PRIVACY.md) for more details on our privacy-first approach.


## 📄 License

This project is released under the AGPL-3.0 License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

Made with ♥ by [Sooraj Sathyanarayanan](https://github.com/iAnonymous3000)
