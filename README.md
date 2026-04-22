# ruphaa.dev

[![Built with Astro](https://img.shields.io/badge/Astro-1.8-BC52EE?logo=astro&logoColor=white)](https://astro.build)
[![Styled with Tailwind](https://img.shields.io/badge/Tailwind-3.2-06B6D4?logo=tailwindcss&logoColor=white)](https://tailwindcss.com)
[![TypeScript](https://img.shields.io/badge/TypeScript-4.9-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-FED689.svg)](LICENSE)

> 🪴 My personal corner of the internet — a digital garden where I share what I **learn**, what I **build**, and what I **write**.

[🌐 Live Site](https://ruphaa.dev) · [💬 Say Hi](https://twitter.com/ruphaaganesh)

---

## ✨ What's Inside

This site is intentionally simple — a lightweight, fast, and joyful place to collect thoughts and work.

- **🌗 Light / Dark mode** — Toggle your preferred vibe anytime
- **📦 Collapsible Archives** — Old content tucked away neatly, still easy to find
- **📝 Markdown-powered** — All content lives in plain `.md` files via Markdoc
- **📡 RSS Feed** — Subscribe at `/rss.xml`
- **📱 Fully Responsive** — Looks great on every screen size
- **⚡ Blazing Fast** — Statically generated with Astro

---

## 🛠 Tech Stack

| Layer | Tech |
|-------|------|
| **Framework** | [Astro](https://astro.build) — zero-JS by default, islands when needed |
| **Styling** | [Tailwind CSS](https://tailwindcss.com) — with a custom "bubblegum" theme |
| **Content** | [Markdoc](https://markdoc.dev) — Markdown with structure & validation |
| **Type System** | TypeScript |
| **Icons** | Font Awesome |

---

## 🗂️ Content

The site is organized into three curated spaces. Older posts live in **Archives** — click to expand and browse.

| Section | Route | What Goes Here |
|---------|-------|----------------|
| **Write** | `/write` | Blog posts, tutorials, and deep dives |
| **Build** | `/build` | Side projects and things I've shipped |
| **Learn** | `/learn` | Book notes, quick thoughts, and snippets |

---

## 🚀 Getting Started

```bash
# 1. Clone the repo
git clone https://github.com/ruphaa/ruphaa-blogster.git
cd ruphaa-blogster

# 2. Install dependencies
npm install

# 3. Start the dev server
npm run dev

# 4. Open http://localhost:9000
```

### Build for Production

```bash
npm run build
```

The static output lands in the `dist/` folder, ready for Netlify, Vercel, or any static host.

---

## ✏️ Adding Content

Everything lives in the `content/` directory as plain Markdown files with YAML frontmatter.

### Blog Post (`content/write/`)

```markdown
---
external: false
title: "Your Post Title"
date: 2024-06-15
ogImagePath: "/images/blog/your-image.png"
---

Your post content here. Supports images, code blocks, embeds, and more.
```

Set `external: true` and add a `url:` field for posts that live elsewhere.

### Project (`content/projects/`)

```markdown
---
title: "Project Name"
description: "What it does"
date: 2024-06-15
url: https://github.com/ruphaa/your-project
---
```

Projects are always external links — great for linking to GitHub repos, live demos, or case studies.

### Writing / Library Note (`content/library/`)

```markdown
---
external: false
title: "Note Title"
date: 2024-06-15
---

Book notes, quick thoughts, or anything worth remembering.
```

---

## 🏗 Project Structure

```
ruphaa-blogster/
├── content/                 # All Markdown content
│   ├── write/               # Write — blog posts & tutorials
│   ├── projects/            # Build — projects
│   └── library/             # Learn — book notes & snippets
├── public/                  # Static assets (images, fonts, favicons)
│   └── fontawesome/         # Self-hosted icon font
├── src/
│   ├── components/          # Astro UI components (Header, Footer, Nav, etc.)
│   ├── layouts/             # Page layouts & HTML skeleton
│   ├── lib/                 # Helpers, SEO, Markdoc config, content reader
│   ├── pages/               # Astro file-based routing
│   └── styles/              # Global CSS, Tailwind theme, typography
├── astro.config.mjs         # Astro configuration
├── tailwind.config.cjs      # Tailwind + custom color tokens
└── package.json
```

---

## 🎨 Theme

The site uses a playful "bubblegum" color palette with light and dark modes. Colors are defined as CSS custom properties in `src/styles/theme.css` and mapped through `tailwind.config.cjs`.

Toggle the theme with the sun/moon button in the header — your preference is saved in `sessionStorage`.

---

## 🙏 Acknowledgements

This site was originally scaffolded with [**Blogster**](https://github.com/flexdinesh/blogster), a wonderful Astro blog starter by [Dinesh Pandiyan](https://github.com/flexdinesh). I've since reshaped the navigation, added archives, built out the theme toggle, and made it my own — but the solid bones are all Blogster.

---

## 📄 License

MIT © [Ruphaa Ganesan](https://github.com/ruphaa)
