# mhoangvslev.github.io

Personal academic website of [Minh-Hoang Dang](https://mhoangvslev.github.io), built with [Jekyll](https://jekyllrb.com/) and the [al-folio](https://github.com/alshedivat/al-folio) theme (used as a template, not a fork).

## Structure

| What                                  | Where                      |
| ------------------------------------- | -------------------------- |
| Site settings, name, URL              | `_config.yml`              |
| About page and bio                    | `_pages/about.md`          |
| Social links                          | `_data/socials.yml`        |
| Publications (BibTeX)                 | `_bibliography/papers.bib` |
| CV (education, experience, skills...) | `_data/cv.yml`             |
| Projects                              | `_projects/`               |
| Photo                                 | `assets/img/prof_pic.jpg`  |

## Run locally

```bash
export LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.

## Deployment

Pushes to `main` are built and deployed by the GitHub Actions workflows in `.github/workflows/`. In the repository settings, Pages must use **GitHub Actions** as its source.

## Credits and license

Theme: [al-folio](https://github.com/alshedivat/al-folio) by Maruan Al-Shedivat and contributors, MIT licensed. See `LICENSE`.
