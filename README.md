# andrewchang — personal site

A minimal, single-page academic site. No themes, no JavaScript, no external
fonts or packages. GitHub Pages builds it automatically on every push to
`master`; the live site is <https://curlsloth.github.io>.

## Editing

Everything you'll normally touch is plain text:

| What you want to change        | File                        |
| ------------------------------ | --------------------------- |
| Bio, research interests, news  | `index.md`                  |
| Publications                   | `_data/publications.yml`    |
| Name, links, email, photo      | `_config.yml`               |
| Colors, fonts, spacing         | `assets/css/style.css`      |
| Page structure / layout        | `_layouts/default.html`     |

### Add a publication

Open `_data/publications.yml` and copy an existing block into the `journal:` (or
`conference:`) list, keeping entries newest-first:

```yaml
  - title: "Your paper title"
    authors: "Chang, A.; Coauthor, B."   # your name as "Chang, A." is auto-bolded
    venue: "Journal Name"
    year: 2026
    volume: "12"        # optional
    pages: "1–10"       # optional
    doi: "10.xxxx/xxxxx" # optional; becomes the title link
```

## Local preview (optional)

```bash
bundle install
bundle exec jekyll serve
```

Then open <http://localhost:4000>. This is only for previewing — pushing to
GitHub is all that's needed to publish.
