# Bonobo Website

Official website for Bonobo - AI Dating Insights app.

## Pages

- **index.html** - Landing page
- **support.html** - Support page with FAQ and contact form
- **privacy.html** - Privacy Policy and Terms of Service

## Setup

### Contact Form Configuration

The contact form uses [Formspree](https://formspree.io) to handle submissions and forward them to your email.

**To activate the form:**

1. Go to https://formspree.io
2. Sign up for free account
3. Create a new form
4. Copy your form endpoint (looks like: `https://formspree.io/f/YOUR_FORM_ID`)
5. In `support.html`, replace `YOUR_FORM_ID` on line 79 with your actual form ID:
   ```html
   <form class="contact-form" action="https://formspree.io/f/YOUR_ACTUAL_ID" method="POST">
   ```
6. Configure Formspree to forward submissions to: `bonobo.app.ai@gmail.com`

### Deploy to GitHub Pages

1. Create a new repository on GitHub called `bonobo-website`
2. Push this code:
   ```bash
   git init
   git add .
   git commit -m "Initial website setup"
   git branch -M main
   git remote add origin https://github.com/bonobo-ai/bonobo-website.git
   git push -u origin main
   ```
3. Go to repository Settings → Pages
4. Source: Deploy from branch `main`, folder `/ (root)`
5. Save

Your website will be live at: `https://bonobo-ai.github.io/bonobo-website/`

### URLs for App Stores

- **Support URL**: `https://bonobo-ai.github.io/bonobo-website/support.html`
- **Privacy Policy**: `https://bonobo-ai.github.io/bonobo-website/privacy.html`
- **Terms of Service**: `https://bonobo-ai.github.io/bonobo-website/privacy.html#terms`

## Customization

### Colors

The site uses your brand colors defined in `styles.css`:
- Primary: `#0091AA`
- Secondary: `#006F85`
- Accent: `#33ABC0`
- Light Background: `#E6F4FE`

### App Store Links

Update the download buttons in `index.html` (lines 24-25) with your actual App Store and Google Play URLs once your apps are published.

## Local Development

Simply open `index.html` in a web browser. No build process required.

## License

© 2025 Bonobo. All rights reserved.
