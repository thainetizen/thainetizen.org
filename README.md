# Thai Netizen Website

Official website for Thai Netizen - a civil society organization advocating for internet freedom and digital rights in Thailand.

Built with [Zensical](https://zensical.org/), a modern static site generator based on Material for MkDocs.

## Features

- 🌐 **Bilingual**: Available in English and Thai (ไทย)
- 🎨 **Material Design**: Clean, modern interface using Material theme
- 📱 **Responsive**: Mobile-friendly design
- ⚡ **Fast**: Static site generation for optimal performance
- 🔒 **Secure**: Deployed on Cloudflare Pages with HTTPS

## Project Structure

```
thainetizen.org/
├── docs/               # English content
│   ├── index.md       # Homepage
│   ├── about.md       # About page
│   ├── projects.md    # Projects page
│   ├── news.md        # News & updates
│   ├── contact.md     # Contact page
│   └── th/            # Thai translations
│       ├── index.md
│       ├── about.md
│       ├── projects.md
│       ├── news.md
│       └── contact.md
├── zensical.toml      # Site configuration
├── requirements.txt   # Python dependencies
└── .github/
    └── workflows/
        └── deploy.yml # CI/CD workflow
```

## Getting Started

### Prerequisites

- Python 3.x
- pip (Python package manager)

### Local Development

1. **Clone the repository**

   ```bash
   git clone https://github.com/thainetizen/thainetizen.org.git
   cd thainetizen.org
   ```

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Run development server**

   ```bash
   zensical serve
   ```

   The site will be available at `http://localhost:8000` with auto-reload enabled.

## Building the Site

To build the static site:

```bash
zensical build
```

The built site will be output to the `site/` directory.

To build with a clean cache:

```bash
zensical build --clean
```

## Deployment

### Automatic Deployment (Recommended)

The site is automatically deployed to Cloudflare Pages when changes are pushed to the `main` or `master` branch via GitHub Actions.

**Required Secrets:**

Configure these in your GitHub repository settings (Settings → Secrets and variables → Actions):

- `CLOUDFLARE_API_TOKEN`: Your Cloudflare API token with Pages permissions
- `CLOUDFLARE_ACCOUNT_ID`: Your Cloudflare account ID

### Manual Deployment

1. Build the site:
   ```bash
   zensical build --clean
   ```

2. Deploy the `site/` directory to your hosting provider (Cloudflare Pages, GitHub Pages, Netlify, etc.)

### Cloudflare Pages Setup

1. Create a Cloudflare account at https://dash.cloudflare.com/
2. Navigate to Workers & Pages → Create application → Pages → Connect to Git
3. Select your GitHub repository
4. Configure build settings:
   - **Build command**: `pip install -r requirements.txt && zensical build --clean`
   - **Build output directory**: `site`
   - **Environment variables**: None required

## Configuration

### Site Settings

Edit `zensical.toml` to customize:

- Site name, description, and URL
- Navigation structure
- Theme colors and features
- Social media links
- Language settings

### Adding Content

#### English Content

Add or edit Markdown files in the `docs/` directory.

#### Thai Content

Add or edit Markdown files in the `docs/th/` directory, maintaining the same file structure as the English content.

### Markdown Features

Zensical supports advanced Markdown features:

- Admonitions (notes, warnings, tips)
- Code blocks with syntax highlighting
- Content tabs
- Diagrams (Mermaid)
- Icons and emojis
- Task lists
- And more!

See the [Zensical documentation](https://zensical.org/docs/) for details.

## Contributing

Contributions are welcome! Please feel free to submit issues and pull requests.

### Content Guidelines

- Keep content focused on internet freedom and digital rights
- Maintain a professional tone appropriate for a civil society organization
- Ensure Thai translations accurately reflect the English content
- Test your changes locally before submitting

## License

This project is licensed under the terms specified in the [LICENSE](LICENSE) file.

## Contact

- **Website**: https://thainetizen.org
- **Email**: contact@thainetizen.org
- **GitHub**: https://github.com/thainetizen
- **Twitter**: https://twitter.com/thainetizen

## Acknowledgments

- Built with [Zensical](https://zensical.org/)
- Deployed on [Cloudflare Pages](https://pages.cloudflare.com/)
- Theme based on [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)

