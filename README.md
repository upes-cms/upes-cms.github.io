# UPES-CMS website - Version 1

Deployable Jekyll site adapted from the structure and conventions of `sbryngelson/academic-website-template`.

## Edit content

- Each faculty member has exactly one primary data file in `_data/faculty/`.
- Add current and previous students in `_data/students.yml`.
- Edit research text in `_pages/research.md`.

## Preview locally

```bash
bundle install
bundle exec jekyll serve
```

Open `http://localhost:4000`.

## Deploy on GitHub Pages

1. Create a GitHub repository and upload this package.
2. In Settings > Pages, select **GitHub Actions** as the source.
3. Push to the `main` or `source` branch. The included workflow builds and deploys automatically.

For a project repository such as `upes-cms`, set `baseurl: "/upes-cms"` in `_config.yml`. For an organization/user Pages repository, leave `baseurl` empty.

## Notes

- Software, Teaching, and Blog are intentionally absent from the navigation and package.
- Initials are used as accessible placeholders until portraits are supplied.
- Version 1 content was prepared from the supplied CV PDFs. The source PDFs are not bundled because they contain phone numbers and other personal biodata; only public-facing academic information was retained.
