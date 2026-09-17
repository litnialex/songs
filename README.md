# Songs

Source for a personal songbook site built with [MkDocs](https://www.mkdocs.org/) and the [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) theme, published via GitHub Pages.

## Files in this repo

| Path                             | Purpose                                                                                                                                                                                                                      |
| -------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `Songs/`                         | The site content. Each `.md` file is one song page; `Songs/index.md` is the site's home page.                                                                                                                                |
| `songs-mkdocs.yml`               | MkDocs config: site name, theme, markdown extensions, and plugins used to build the site from `Songs/`.                                                                                                                      |
| `.github/workflows/gh-pages.yml` | GitHub Actions workflow that builds the site and deploys it to GitHub Pages on every push to `main`.                                                                                                                         |
| `.gitignore`                     | Ignores everything by default (`*`); song and config files are tracked because they were force-added.                                                                                                                        |

