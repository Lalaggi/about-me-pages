# about-me-pages

A static HTML/CSS About Me page showcasing my GitLab projects and tools, hosted on Cloudflare Pages.

**Source:** [gitlab.com/Lalaggi/about-me-pages](https://gitlab.com/Lalaggi/about-me-pages)

**Live:** [lalaggi.xyz](https://lalaggi.xyz) · [about.lalaggi.xyz](https://about.lalaggi.xyz)

## Features

- **Intro** - name, pronouns, and short bio
- **Projects grid** - auto-generated cards for all GitLab projects (from a single `projects` array in `index.html`)
- **Static & fast** - no build step, just HTML + CSS, deployed to Cloudflare Pages

## Structure

```
index.html      # page content + project list (edit projects array here)
assets/
  style.css     # Material 3 Expressive dark theme (purple seed)
```

To add or update a project, edit the `projects` array in `index.html`:

```js
{ name: "my-project", url: "https://gitlab.com/Lalaggi/my-project", desc: "One-line description." }
```

## Development

Open `index.html` directly in a browser, or serve locally:

```bash
python -m http.server 8000
# then visit http://localhost:8000
```

No dependencies or build tools required.

## Deployment

Hosted on **Cloudflare Pages** (connected to the `main` branch). Any push to `main` auto-deploys to both:

- https://lalaggi.xyz
- https://about.lalaggi.xyz

## Reporting Issues

https://gitlab.com/Lalaggi/about-me-pages/-/issues

## License

GPL-3.0 - see [LICENSE](LICENSE).
