# Zoë B Cullen - Academic Website

Personal academic website for Zoë B Cullen, Associate Professor at Harvard Business School.

## Overview

This is a static website hosted on GitHub Pages showcasing academic research, publications, and professional information.

**Live Site:** [https://zcullen.github.io](https://zcullen.github.io)

## Structure

```
├── index.html          # Main landing page with bio and contact info
├── research/           # Research publications page
│   └── index.html      # Research papers with collapsible abstracts
├── assets/             # Static assets
│   ├── css/           # Stylesheets
│   ├── docs/          # PDF files for papers and CV
│   └── img/           # Images
└── README.md          # This file
```

## Features

- **Responsive Design**: Built with Tailwind CSS for mobile and desktop viewing
- **Research Page**: Publications organized by status (published, forthcoming, working papers)
- **Collapsible Abstracts**: All paper abstracts use native HTML `<details>` elements for clean, compact presentation
- **Google Analytics**: Integrated tracking (ID: G-268BMM7D5G)

## Technology Stack

- HTML5
- Tailwind CSS
- GitHub Pages for hosting
- No build process required - pure static HTML

## Making Updates

### Adding a New Paper

1. Open `research/index.html`
2. Add a new paper entry following the existing structure:

```html
<div class="lg:static">
  <div class="mb-8 text-base">
    <div class="mb-6">
      <div class="mb-2">
        <a class="text-blue-600 font-medium text-lg" href="/assets/docs/paper.pdf">Paper Title</a>
        <p class="italic">with Co-authors</p>
      </div>
      <div>
        <div class="text-teal-600 text-base mb-2">
          <p><a class="italic"/>Journal Name</a></p>
        </div>
        <details>
          <summary class="cursor-pointer text-gray-900 font-medium">Abstract</summary>
          <p class="mt-2">Abstract text here...</p>
        </details>
      </div>
    </div>
  </div>
</div>
```

3. Upload the paper PDF to `assets/docs/`
4. Commit and push changes

### Updating CV

1. Upload new CV PDF to `assets/docs/`
2. Update the CV link in both `index.html` and `research/index.html`

## Deployment

The site automatically deploys to GitHub Pages when changes are pushed to the `main` branch.

## Local Development

Since this is a static site, you can simply open `index.html` in a browser to preview changes locally:

```bash
open index.html
```

Or use a local server:

```bash
python3 -m http.server 8000
# Visit http://localhost:8000
```

## Analytics

The site uses Google Analytics to track visitor data. The tracking ID is configured in the `<head>` section of each HTML file.

## License

All rights reserved. Content copyright © Zoë B Cullen.
