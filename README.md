# Academic Website

A minimal academic portfolio website built with Hugo, styled with a mid-century sci-fi inspired theme.

## Architecture

- Static website built with Hugo
- Custom layouts and templates
- Single CSS stylesheet for theming
- Markdown content for pages

## Directory Structure

```
hawc2.github.io/
├── content/              # Markdown content
├── layouts/              # Hugo templates
├── static/               # Static assets (CSS, images)
├── .github/workflows/    # GitHub Actions deploy
├── hugo.toml             # Hugo configuration
├── netlify.toml          # Netlify deployment config
└── README.md             # Project documentation
```

## Key Files

- `hugo.toml` - Site configuration, menus, base URL
- `layouts/_default/baseof.html` - Base template
- `layouts/index.html` - Home page template
- `layouts/partials/header.html` - Header and navigation
- `layouts/partials/footer.html` - Footer
- `static/css/style.css` - Main theme stylesheet

## Local Development

### Prerequisites

- Hugo Extended v0.152.0 or later

### Running Locally

```bash
# Navigate to the site directory
cd hawc2.github.io

# Start the Hugo development server
hugo server -D

# View the site at http://localhost:1313
```

## Customization

### Update Site Information

Edit `hugo.toml` to update:
- Site title
- Base URL (for deployment)
- Author name
- Navigation menu items

### Content

- **Home page**: Edit `layouts/index.html`
- **CV**: Edit `content/cv/_index.md`
- **Projects**: Edit `content/projects/_index.md`

### Styling

All styles are in `static/css/style.css`. The theme uses:
- Custom color variables for muted accents
- Retro-styled typography from Google Fonts
- Subtle entrance animations

## External Dependencies

- Hugo Extended v0.152.0+
- Google Fonts: Bebas Neue, Fira Sans Condensed, IBM Plex Serif

## Resources

- Hugo documentation: https://gohugo.io/documentation/
- Hugo templates: https://gohugo.io/templates/introduction/
- GitHub Pages hosting: https://gohugo.io/hosting-and-deployment/hosting-on-github/
- Netlify hosting: https://gohugo.io/hosting-and-deployment/hosting-on-netlify/

## Deployment

### GitHub Pages

1. Push your code to a GitHub repository
2. Go to Settings > Pages
3. Set source to "GitHub Actions"
4. The `.github/workflows/hugo.yml` file will automatically build and deploy

Ensure `hugo.toml` uses the correct baseURL:
```
baseURL = 'https://hawc2.github.io/'
```

### Netlify

1. Connect your repository to Netlify
2. Netlify will automatically detect the `netlify.toml` configuration
3. Deploy settings are pre-configured

Or use the Netlify CLI:
```bash
netlify deploy --prod
```

## License

Feel free to use this template for your own academic website.
