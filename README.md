# Songs

Source for [sasha.canta.md](https://sasha.canta.md/) — a personal songbook built with [MkDocs](https://www.mkdocs.org/) and the [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) theme, published via GitHub Pages.

## Files in this repo

| Path | Purpose |
| --- | --- |
| `Songs/` | The site content. Each `.md` file is one song page; `Songs/index.md` is the site's home page. |
| `songs-mkdocs.yml` | MkDocs config: site name, theme, markdown extensions, and plugins used to build the site from `Songs/`. |
| `songs-mkdocs-req.txt` | Python packages needed to build the site (`mkdocs`, `mkdocs-material`, and the [`mkdocs-publisher`](https://github.com/litnialex/mkdocs-publisher) plugin, pinned to a fork with an empty-slug fix for non-ASCII filenames). |
| `.github/workflows/gh-pages.yml` | GitHub Actions workflow that builds the site and deploys it to GitHub Pages on every push to `main`. |
| `.gitignore` | Ignores everything by default (`*`); song and config files are tracked because they were force-added. |

### Song front matter

Each song file starts with YAML front matter consumed by the `pub-meta` plugin:

```yaml
---
publish: "true"   # or: draft / hidden
---
```

- `"true"` — page is built and shown in navigation.
- `draft` (the default if omitted) — page is excluded from the build.
- `hidden` — page is built and reachable by URL but left out of navigation (used for `index.md`).

