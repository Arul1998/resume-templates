# resume-templates

A growing collection of **resume and CV templates** in different structures and styles. Pick a folder, customize the content, and export to PDF or host as a static page.

**Repository:** [github.com/Arul1998/resume-templates](https://github.com/Arul1998/resume-templates)

**Author:** [Arul Cornelious](https://arulcornelious.com)  
**Profiles:** [GitHub](https://github.com/Arul1998) · [LinkedIn](https://www.linkedin.com/in/arul-cornelious) · [Portfolio](https://arulcornelious.com) · [Email](mailto:arulcornelious@gmail.com)

---

### If you find this useful

- **Star the repo** on GitHub — it helps others discover these templates and shows support for the project. Click **Star** at the top of [the repository page](https://github.com/Arul1998/resume-templates).
- **Buy me a coffee** — [Buy Me a Coffee](https://www.buymeacoffee.com/arulcornelious) if you would like to say thanks.

---

## Templates

| Folder | Format | Notes |
|--------|--------|--------|
| [`single-page-html`](./single-page-html/) | HTML (single file) | Gradient header, skills grid, experience, print-friendly A4. No build step. |

New layouts are added as **separate top-level folders** next to `single-page-html` (for example: two-column HTML, minimal, LaTeX export, another visual style).

### Preview (why not an iframe?)

GitHub **does not allow** `<iframe>` (or most raw HTML) in README files; those tags are removed when the page is rendered. To show how a template looks, use one or more of these instead:

| Approach | Works on GitHub? |
|------------|------------------|
| **Live link** | Yes — open the hosted page in a new tab. |
| **Screenshot** | Yes — commit a PNG/WebP and embed with `![alt](./path/to/image.png)`. |
| **PNG screenshot** | Yes — best compatibility; commit a `preview.png` and embed it. |
| **Vector wireframe** | Yes — optional SVG ([`preview.svg`](./single-page-html/preview.svg)). |
| **iframe** | **No** — stripped for security. |

**Live preview (single-page HTML)** — works once [GitHub Pages](#github-pages) is configured and deployed:  
[Open the template in your browser](https://Arul1998.github.io/resume-templates/single-page-html/) (replace `Arul1998` with your username if you forked the repo). If the link 404s or looks wrong, follow the steps below — this repo includes a [`.nojekyll`](./.nojekyll) file so placeholder syntax like `{{FULL_NAME}}` is not broken by Jekyll.

Stylized layout reference (sample wireframe — not your real data; [open `preview.png` locally](./single-page-html/preview.png) if the image does not load):

[![Stylized preview of the single-page HTML resume — click to open the live GitHub Pages version](./single-page-html/preview.png)](https://Arul1998.github.io/resume-templates/single-page-html/)

## Using this repository

1. Clone or download the repo.
2. Open the README inside the template folder you want (e.g. [`single-page-html/README.md`](./single-page-html/README.md)).
3. Follow that template’s instructions for placeholders and PDF export.

## GitHub Pages

### Enable Pages (once per repository)

1. Open the repo on GitHub → **Settings** → **Pages** (under “Code and automation”).
2. Under **Build and deployment** → **Source**, choose **Deploy from a branch**.
3. **Branch:** `main`, folder **`/ (root)`** → **Save**.
4. Wait 1–3 minutes. The site URL appears at the top of the Pages settings (and in green on the **Actions** tab when the deploy finishes).

### Live URL

With the default setup, the single-page template is at:

`https://Arul1998.github.io/resume-templates/single-page-html/`

Use your own GitHub username in place of `Arul1998` if you forked the repo.

### Why the live preview can fail (and how this repo fixes it)

| Issue | What to do |
|--------|------------|
| **404 Not Found** | Pages is not enabled yet, or the deploy is still running. Confirm the URL in **Settings → Pages** and wait a few minutes after saving. |
| **Blank page or build error** | GitHub Pages runs **Jekyll** by default. Jekyll treats `{{ ... }}` in HTML as **Liquid** templates, which breaks `index.html`’s resume placeholders. This repository includes an empty **`.nojekyll`** file at the [repo root](./.nojekyll) so files are served as plain static HTML. Commit and push `.nojekyll`, then redeploy (push any commit or re-run Pages). |
| **Wrong account** | Project Pages URLs are always `https://<owner>.github.io/<repo>/...`. Forks use *your* username, not the original author’s. |

After pushing changes, open the live link in an **incognito/private** window or hard-refresh (**Ctrl+F5**) to avoid a cached 404.

## Adding a new resume template (for contributors)

Contributions are welcome. Follow this structure so maintainers can review your work and users can find your template easily.

### 1. Fork and branch

- Fork [this repository](https://github.com/Arul1998/resume-templates).
- Create a branch from `main` with a clear name, e.g. `add-minimal-html-template`.

### 2. Add a new top-level folder

- Use a **short, descriptive folder name** in `kebab-case` (e.g. `minimal-html`, `two-column-latex`, `print-a4-markdown`).
- **Do not** nest your template inside `single-page-html` — each template is its **own** directory at the repo root.

### 3. What to include in that folder

| Item | Purpose |
|------|--------|
| **`README.md`** | How to fill in content, export to PDF or print, any dependencies, and browser or tool requirements. |
| **Template files** | Source files users edit (HTML, CSS, Markdown, etc.). Prefer **no mandatory build step** unless you document it clearly. |
| **Assets** | Images, fonts, or CSS kept **inside the same folder** (or documented paths) so the template is self-contained or easy to clone. |
| **License** | Your contribution should be compatible with this repo’s [MIT License](./LICENSE). |

### 4. Document placeholders and customization

- Explain every placeholder or variable users must replace (see [`single-page-html`](./single-page-html/) for an example).
- Mention print settings (e.g. A4, margins) if relevant.

### 5. Register the template in the root README

- Add a **new row** to the **Templates** table in this file with the folder name, format, and a one-line description.

### 6. Open a pull request

- Describe what your template offers and how it differs from existing ones.
- Optional: add a screenshot in the PR description so people can preview the layout.

Pull requests that match the above are much easier to merge. If you are unsure, open an issue first to discuss the idea.

## Contributing (short version)

- One template = **one root-level folder** + **README** + **self-contained assets**.
- Update the **Templates** table in this README when you add something new.
- Keep the project approachable: clear docs, minimal friction for people who only want to download and edit.

## Publish to GitHub (maintainer)

This folder is a Git repo on branch `main`. To create **`resume-templates`** on GitHub and push in one step (after a one-time login):

```powershell
cd C:\Users\kutty\resume-templates
gh auth login
gh repo create resume-templates --public --source=. --remote=origin --push
```

If you already created an **empty** repository named `resume-templates` under [github.com/Arul1998](https://github.com/Arul1998), use:

```powershell
git push -u origin main
```

## License

MIT — see [LICENSE](./LICENSE).
