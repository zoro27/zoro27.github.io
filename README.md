# Le Zhou — Personal Academic Website

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-live-brightgreen)](https://zoro27.github.io)
[![Jekyll](https://img.shields.io/badge/Jekyll-CC0000?logo=jekyll)](https://jekyllrb.com/)
[![Theme](https://img.shields.io/badge/theme-Minimal%20Mistakes-blue)](https://github.com/mmistakes/minimal-mistakes)

My personal academic website built with **Jekyll** and the **Minimal Mistakes** theme, hosted on **GitHub Pages**.

## 📂 Structure

```
├── _config.yml          # Site configuration
├── index.md             # Homepage (bio, news, recent pubs)
├── _pages/
│   ├── about.md         # About page
│   ├── blog.md          # Blog listing
│   ├── cv.md            # Curriculum Vitae
│   └── publications.md  # Publications listing
├── _posts/              # Blog posts
├── _publications/       # Individual publication entries
├── _data/
│   └── navigation.yml   # Site navigation
└── assets/
    ├── css/main.scss    # Custom styles
    ├── docs/            # PDF files (CV, slides, posters)
    └── images/          # Images (avatar, header, etc.)
```

## 🚀 Quick Start

```bash
# Install Jekyll and dependencies
gem install bundler jekyll

# Run locally
bundle exec jekyll serve

# Visit http://localhost:4000
```

## ✏️ Customization Checklist

1. **Update `_config.yml`** — your name, email, social links, university
2. **Add your photo** — place `bio-photo.jpg` in `assets/images/`
3. **Add your CV PDF** — place `cv.pdf` in `assets/docs/`
4. **Update publications** — edit files in `_publications/`
5. **Write blog posts** — add `.md` files to `_posts/`
6. **Customize colors** — edit `assets/css/main.scss`

## 📝 Publishing

Push to the `main` branch — GitHub Pages builds and deploys automatically.
