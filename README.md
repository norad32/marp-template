# Marp Template

Simple Marp template with a custom theme based on uncover, background image, two-column layout, and example slides.

## Quick start

```bash
sudo pacman -S npm firefox
```

Render the deck:

```bash
npx @marp-team/marp-cli@latest slide-deck.md --theme ./custom.css
```

Export to PDF:
```bash
npx @marp-team/marp-cli@latest slide-deck.md --theme ./custom.css --allow-local-files -o slide-deck.pdf
```

## Credits

Built with [Marp](https://github.com/marp-team/marp).
