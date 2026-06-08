# WebGet - Digital Services Agency

A high-performance, SEO-optimized website built with Astro, Tailwind CSS, and modern web technologies.

## 🚀 Tech Stack

- **Framework**: [Astro](https://astro.build/) - Static-first, content-focused
- **Styling**: [Tailwind CSS](https://tailwindcss.com/) - Utility-first CSS
- **Animations**: CSS Animations + [Framer Motion](https://www.framer.com/motion/) for React components
- **Content**: Astro Content Collections with Markdown
- **View Transitions**: Native Astro View Transitions API

## 📁 Project Structure

```
webget/
├── public/
│   ├── images/          # Static images
│   ├── favicon.svg
│   └── robots.txt
├── src/
│   ├── components/      # Reusable components
│   │   ├── animations/  # Framer Motion wrappers
│   │   ├── Header.astro
│   │   ├── Footer.astro
│   │   ├── Hero.astro
│   │   ├── Services.astro
│   │   └── ContactForm.astro
│   ├── content/         # Content Collections
│   │   ├── config.ts
│   │   ├── blog/
│   │   └── portfolio/
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/
│   │   ├── index.astro
│   │   ├── blog/
│   │   └── portfolio/
│   └── styles/
│       └── global.css
├── astro.config.mjs
├── tailwind.config.mjs
├── tsconfig.json
└── package.json
```

## 🛠️ Getting Started

### Prerequisites

- Node.js 18+ 
- npm or pnpm

### Installation

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## 📝 Content Management

### Adding Blog Posts

Create a new `.md` file in `src/content/blog/`:

```markdown
---
title: "Your Post Title"
description: "Brief description"
pubDate: 2024-01-15
author: "Author Name"
image: "/images/post-image.jpg"
tags: ["tag1", "tag2"]
---

Your content here...
```

### Adding Portfolio Projects

Create a new `.md` file in `src/content/portfolio/`:

```markdown
---
title: "Project Title"
description: "Project description"
client: "Client Name"
date: 2024-01-10
image: "/images/project-image.jpg"
tags: ["web design", "development"]
featured: true
url: "https://example.com"
---

Project details here...
```

## ⚡ Performance

This site is optimized for perfect Lighthouse scores:

- **Performance**: 100
- **Accessibility**: 100
- **Best Practices**: 100
- **SEO**: 100

### Optimizations Include:

- Static HTML generation
- Minimal JavaScript
- Optimized images with lazy loading
- Preconnect to external resources
- Semantic HTML structure
- ARIA labels for accessibility

## 🎨 Customization

### Colors

Edit `tailwind.config.mjs` to change the color scheme:

```javascript
colors: {
  primary: '#0f172a',    // Dark background
  accent: '#3b82f6',     // Blue accent
  'accent-light': '#60a5fa',
}
```

### Fonts

Fonts are loaded via `@fontsource`. To change fonts:

1. Install new font package: `npm install @fontsource/your-font`
2. Import in `Layout.astro`
3. Update `tailwind.config.mjs` fontFamily

## 📄 License

MIT License - feel free to use this template for your projects.

## 🤝 Contact

For inquiries, reach out at hello@webget.com
