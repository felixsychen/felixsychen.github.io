# Academic homepage

This repository is a small Jekyll site inspired by [Jon Barron's academic homepage](https://jonbarron.info/). Its layout is rebuilt for easy editing; it does not include his photos, papers, or project assets.

The published page is at <https://felixsychen.github.io/>. GitHub Pages should build from the `main` branch and the repository root.

## Edit the content

Open [`_data/content.yml`](_data/content.yml) on GitHub, click the pencil icon, edit the fields, and commit. Empty sections are hidden automatically. To add a publication, replace `publications: []` with a list like this:

```yaml
publications:
  - title: "Paper title"
    authors: "First Author, Second Author"
    venue: "Conference or status"
    year: "2026"
    summary: "A short description of the work."
    image: "images/paper-image.jpg"
    highlighted: false
    links:
      - label: "Paper"
        url: "https://example.com/paper"
      - label: "Code"
        url: "https://github.com/example/repository"
```

Add a portrait at `images/profile.jpg` and enter `images/profile.jpg` in `profile.photo`. Add a CV at `files/CV.pdf` and enter `files/CV.pdf` in `profile.cv`. Paths to local files have no leading slash so Jekyll can resolve them at the site root.

The main layout is in `index.html`, and the styling is in `stylesheet.css`. Jekyll reads `_data/content.yml` during each GitHub Pages build. Do not add `.nojekyll`.
