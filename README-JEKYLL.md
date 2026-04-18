# Mweetwa Mweembo Nketani - Jekyll Portfolio

A modern, responsive portfolio website built with Jekyll, featuring a clean design with smooth animations and professional styling.

## Features

- **Jekyll Static Site Generator** for fast, secure hosting
- **Responsive Design** that works on all devices
- **Modern CSS** with custom properties and animations
- **SEO Optimized** with proper meta tags and structured data
- **Accessibility** focused with semantic HTML and ARIA labels
- **Dark Mode Support** for system preference
- **Performance Optimized** with compressed CSS and efficient markup

## Setup

### Prerequisites

- Ruby 2.7+ 
- Bundler gem
- Git

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd windsurf-project
```

2. Install dependencies:
```bash
bundle install
```

3. Run the local server:
```bash
bundle exec jekyll serve
```

4. Open your browser to `http://localhost:4000`

## Project Structure

```
windsurf-project/
|-- _config.yml          # Jekyll configuration
|-- _layouts/
|   |-- default.html     # Main layout template
|-- _includes/
|   |-- navigation.html  # Navigation component
|   |-- footer.html      # Footer component
|-- assets/
|   |-- css/
|       |-- style.css    # Main stylesheet
|-- index.md             # Homepage content
|-- Gemfile              # Ruby dependencies
|-- README-JEKYLL.md    # This file
```

## Configuration

Edit `_config.yml` to customize:

- Site title and description
- Author information
- Social media links
- URL and baseurl for deployment

## Deployment

### GitHub Pages

1. Push to your GitHub repository
2. Enable GitHub Pages in repository settings
3. Select source as "GitHub Actions" or "main branch"

### Netlify

1. Connect your Git repository
2. Set build command: `bundle exec jekyll build`
3. Set publish directory: `_site`

## Customization

### Adding New Sections

1. Create new section in `index.md`
2. Add corresponding styles to `assets/css/style.css`

### Modifying Styles

Edit `assets/css/style.css` - uses CSS custom properties for easy theming.

### Changing Content

Update `index.md` with your personal information and content.

## License

© 2026 Mweetwa Mweembo Nketani. All rights reserved.
