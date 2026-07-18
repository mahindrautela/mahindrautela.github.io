# Mahindra S. Rautela — academic website

A lightweight Jekyll site hosted by GitHub Pages. The homepage uses Liquid templates, YAML data, SCSS, and a small vanilla JavaScript file; no client framework or database is required. Existing biography, research, publication, talk, and sitemap routes remain available.

## Run locally

Install Ruby and Bundler, then run:

```sh
bundle install
bundle exec jekyll serve
```

The site is available at `http://localhost:4000`. A production build uses `bundle exec jekyll build`.

## Update content

- News: add a newest-first item to `_data/news.yml`. `date` and `text` are required; `url` and `link_label` are optional.
- Homepage publications: add structured entries to `_data/publications.yml`. The complete bibliography remains in `_pages/publications.md`.
- Biography, research, and talks: edit the matching Markdown file in `_pages/`.
- Profile photograph: replace `images/aps_pic.jpg` while retaining a roughly square crop and sensible file size.
- CV: replace `files/MahindraSRautela_CV_O1.pdf` without changing its filename, or update links in `_pages/about.md` and `_pages/bio.md`.

## Design and architecture

`_layouts/home.html` provides the accessible single-page shell, `_pages/about.md` provides homepage content, `_sass/_modern.scss` controls colors, type, spacing, and responsive behavior, and `assets/js/site.js` handles the mobile menu and publication filters. Dedicated archive pages continue to use the compatible AcademicPages layouts.

The repository is a GitHub user site. GitHub Pages builds Jekyll from the `master` branch; there is no custom deployment workflow in this repository.
