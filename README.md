# Marp Template

A Marp starter deck with a custom theme, bundled sample assets, and examples of backgrounds, two-column layouts, and slide classes.

## Requirements

- Node.js 22 or newer and npm
- Google Chrome, Microsoft Edge, or Mozilla Firefox for PDF export

## Build

Install the pinned dependencies and build both formats:

```bash
npm ci
npm run build
```

Or build only HTML:

```bash
npm run build:html
```

Outputs are written to `dist/`. The HTML export includes the `assets/` directory beside it, so keep the HTML and directory together when sharing or deploying it. PDF conversion uses `--allow-local-files` so local images render. Only run that command on Markdown and themes you trust.

## Customize

Edit `slide-deck.md` and `custom.css`.

To update Marp CLI, install a specific reviewed version and commit both `package.json` and `package-lock.json`:

```bash
npm install --save-dev @marp-team/marp-cli@<version>
```

## GitHub Actions

The workflow builds HTML on pushes and pull requests. It builds PDF on pushes to `main` and manual runs only, because PDF rendering enables local-file access. The uploaded HTML artifact contains both the HTML file and its required assets.

## Credits

Built with [Marp](https://github.com/marp-team/marp).
