# Razo Beckett’s Blog

A personal blog built with [Hugo](https://gohugo.io/), using the [Terminal theme](https://github.com/panr/hugo-theme-terminal). Fast, minimal, and highly customizable.

## Features

- **Terminal theme**: Retro, minimal, and fully responsive.
- **Custom color schemes**: Easily tweak via [Terminal.css](https://panr.github.io/terminal-css/).
- **Syntax highlighting**: Powered by Chroma.
- **Fira Code font**: Beautiful monospaced font for code.
- **Comments**: Integrated via [Giscus](https://giscus.app/).
- **Easy content management**: Write posts in Markdown.
- **SEO-friendly**: Sitemap, robots.txt, and meta tags.
- **Git-based workflow**: Version control for all content and configuration.

## Project Structure

```
.
├── archetypes/         # Content templates
├── content/            # Blog posts and pages
│   └── posts/
├── layouts/            # Custom HTML templates
├── static/             # Static assets (images, CSS, favicon, etc.)
├── themes/terminal/    # Hugo Terminal theme
├── hugo.toml           # Site configuration
└── README.md           # This file
```

## Getting Started

### Prerequisites

- [Hugo Extended](https://gohugo.io/getting-started/installing/) v0.90.x or newer
- [Git](https://git-scm.com/)

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/razobeckett/blog.git
   cd blog
   ```

2. **Install Hugo Terminal theme:**
   ```bash
   git submodule update --init --recursive
   # or manually clone to themes/terminal
   ```

3. **Install dependencies (if any):**
   ```bash
   npm install
   # or
   yarn install
   ```

### Running Locally

Start the development server:

```bash
hugo server -t terminal
```

Visit [http://localhost:1313](http://localhost:1313) in your browser.

### Building for Production

```bash
hugo
```

The static site will be generated in the `public/` directory.

## Customization

- **Config:** Edit `hugo.toml` for site settings, theme options, and menu.
- **Content:** Add Markdown files to `content/posts/` for new blog posts.
- **Assets:** Place images, CSS, and other static files in `static/`.
- **Theme:** Customize the theme in `themes/terminal/` or override styles in `static/style.css`.
- **Comments:** Giscus is configured in `hugo.toml` under `[params.giscus]`.

## Contribution

Contributions, suggestions, and bug reports are welcome! Please open an issue or pull request.

## License

[![CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

Content on this blog is licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
You must give appropriate credit to Razo Beckett and [https://blog.razobeckett.xyz](https://blog.razobeckett.xyz), provide a link to the license, and indicate if changes were made.

The site code and theme are licensed under the MIT License. The Terminal theme is © 2019-2025 Radek Kozieł ([panr](https://rkoziel.com/)), also MIT.

## Credits

- [Hugo](https://gohugo.io/)
- [Terminal Theme](https://github.com/panr/hugo-theme-terminal)
- [Fira Code](https://github.com/tonsky/FiraCode)
- [Giscus](https://giscus.app/)
