# Venkat Akhil Ankem — Portfolio

Personal portfolio website of **Venkat Akhil Ankem**, Ph.D. candidate in Industrial Engineering (Operations Research) at Polytechnique Montréal / GERAD.

Built with the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme (v1.x). The site is deployed automatically to GitHub Pages on every push to `main` via `.github/workflows/deploy.yml`.

**Live site:** https://venkat-akhil-ankem.github.io/

## Local development

Requires Ruby and Bundler:

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000/.

## Customizing

- `_config.yml` — site title, URL, author details, plugins
- `_pages/about.md` — homepage bio
- `_data/cv.yml` — CV page content (also see `assets/pdf/venkat-ankem-cv.pdf`)
- `_data/socials.yml` — email, GitHub, LinkedIn, Scholar, ORCID links
- `_bibliography/papers.bib` — publications (rendered on the publications page; mark key papers `selected = {true}`)
- `_projects/` — project showcase pages
- `_data/repositories.yml` — GitHub repositories shown on the repositories page
- `_news/` — news/announcement items on the homepage
- `assets/img/prof_pic.jpg` — profile photo
