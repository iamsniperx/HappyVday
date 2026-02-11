# Valentine Ask Webpage

A standalone, mobile-first valentine ask page that supports personalization via URL parameters.

## Route

- `http://localhost:8000/valentine/`

Example:

```text
/valentine/?to=Madison&from=Alexis&msg=Be%20mine%20forever&img=https%3A%2F%2Fi.imgur.com%2Fabcd1234.jpg
```

## Supported URL Params

- `from` (required)
- `to` (required)
- `msg` (optional)
- `img` (optional direct image URL ending in `.jpg`, `.jpeg`, `.png`, or `.webp`)

If `img` is missing or fails to load, a default cute SVG illustration is shown.

## Local Run

From repo root:

```bash
python3 -m http.server 8000
```

Then open:

- `http://localhost:8000/valentine/`

## Deploy (Static)

This project is static HTML/CSS/JS, so deploy options include:

- **Netlify**: Drag-and-drop the project folder, publish as static site.
- **Vercel**: Import repository and deploy as “Other” static project.
- **GitHub Pages**: Enable Pages for the repo and serve from root branch.

On deploy, share links in the form:

```text
https://your-domain/valentine/?to=...&from=...&msg=...&img=...
```
