# Single-page HTML resume (gradient)

Print-friendly, responsive CV: gradient header, sectioned skills and experience, and **Print / Save as PDF** in the browser. No build step—open `index.html` locally or host this folder as a static site.

**Template author:** [Arul Cornelious](https://arulcornelious.com) — [GitHub](https://github.com/Arul1998) · [LinkedIn](https://www.linkedin.com/in/arul-cornelious) · [Portfolio](https://arulcornelious.com)

## Preview

Sample wireframe of this layout (gradient header, sections, skills blocks). Open **`preview.png`** in this folder if your Markdown viewer does not show images.

![Preview of the single-page HTML resume layout](./preview.png)

## Quick start

1. Open **`index.html`** in this folder and replace every `{{TOKEN}}` with your content (search for `{{` in your editor).
2. Optional: use **`placeholders.json`** as a checklist (it is not loaded by the page).
3. Preview in a browser, then **Print → Save as PDF** (Chrome or Edge recommended).

## Placeholder reference

| Token | Used for |
|--------|-----------|
| `{{FULL_NAME}}`, `{{HEADLINE}}` | Header |
| `{{LOCATION}}`, `{{PHONE}}`, `{{EMAIL}}` | Contact line |
| `{{LINKEDIN_URL}}`, `{{PORTFOLIO_URL}}`, `{{GITHUB_URL}}` | Links (`https://` URLs) |
| `{{PROFESSIONAL_SUMMARY}}` | Summary (HTML allowed, e.g. `<strong>`) |
| `{{SKILLS_*}}` | Five skill rows: Front-End, Back-End, Mobile, DevOps & Quality, AI/ML |
| `{{PROJECT_N_*}}` | Up to three projects: title, tech line, bullets |
| `{{EDU_N_*}}` | Two education blocks |
| `{{JOB_N_*}}` | Four jobs: title, company, dates, bullets |
| `{{CERT_N_*}}` | Six certification lines |
| `{{LANGUAGES}}`, `{{AVAILABILITY}}`, `{{RELOCATION}}` | Additional information |

## Customizing layout

- **More jobs or projects:** Duplicate a full `.experience-item` or `.project-item` block.
- **Fewer sections:** Remove whole `.section` blocks you do not need.
- **Colors:** In `<style>`, replace `#667eea` and `#764ba2` with your palette.

## Push to GitHub

Create a repository named **`resume-templates`** on your GitHub account, then from the **repository root**:

```bash
git remote add origin https://github.com/Arul1998/resume-templates.git
git branch -M main
git push -u origin main
```

If your GitHub username is different, replace `Arul1998` in the URL.

## Hosting

Works on GitHub Pages, Netlify, Vercel, or any static host. Publish either the **repo root** or **this folder** (`single-page-html`), depending on your provider.
