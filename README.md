# resume-templates

[![GitHub stars](https://img.shields.io/github/stars/Arul1998/resume-templates?style=social&logo=github)](https://github.com/Arul1998/resume-templates)
[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-ffdd00?style=flat&logo=buy-me-a-coffee&logoColor=black)](https://www.buymeacoffee.com/arulcornelious)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

Open-source **resume and CV templates** in several formats. Choose a template folder, replace placeholders with your content, then print to PDF or use the files however you prefer.

If this project is helpful, consider starring the repository or supporting via **Buy Me a Coffee** (badges above).

---

## Templates

| Folder | Format | Notes |
|--------|--------|--------|
| [`single-page-html`](./single-page-html/) | HTML (single file) | Gradient header, skills grid, experience blocks, A4-friendly print. No build step. |

Additional layouts are added as **new top-level folders** alongside `single-page-html` (for example: two-column HTML, minimal typography, or other styles).

## Getting started

1. Clone or download this repository.
2. Open the README in the template you want (for example [`single-page-html/README.md`](./single-page-html/README.md)).
3. Edit the template files and follow the placeholder and export instructions for that folder.

## Contributing a new template

Pull requests are welcome. Use this checklist so reviews stay straightforward:

1. **Fork** this repository and create a branch from `main` (for example `add-template-name`).
2. **Add a new root-level folder** with a short `kebab-case` name (for example `minimal-html`). Do not nest new templates inside `single-page-html`; each template is its own directory.
3. **Include** a `README.md` in that folder (how to edit, export or print, dependencies, browser notes), the template source files, and any assets paths documented or self-contained.
4. **License:** contributions should remain compatible with the [MIT License](./LICENSE).
5. **Document** every placeholder or variable users must change; note print settings (paper size, margins) when relevant.
6. **Update** the **Templates** table in this file with one new row: folder name, format, short description.
7. **Open a pull request** describing the layout and how it differs from existing templates. A screenshot in the PR helps reviewers and users.

Unsure about scope? Open an issue to discuss before investing heavy effort.

**Summary:** one template = one root folder + README + self-contained assets + row in the table above.

## Publishing changes (Git)

| Command | Purpose |
|---------|---------|
| `git add …` | Stage files for the next commit. |
| `git commit -m "…"` | Save a snapshot **locally** only. |
| `git push` | Upload commits to GitHub (requires `origin` or another remote). |

Example (use your own clone path):

```powershell
cd path\to\resume-templates
git add -A
git status
git commit -m "Describe your change"
git push origin main
```

No repository yet? Create one on [GitHub](https://github.com/new), then run `git remote add origin <repository-url>` before the first push.

## License

MIT — see [LICENSE](./LICENSE).
