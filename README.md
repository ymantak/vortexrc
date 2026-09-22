# CRAS Template SCSS Build

This project uses Sass to compile SCSS into the stylesheet used by the HTML pages.

## Output file used by pages

The pages link to:

- `assets/sass/style.css`

So compile from:

- `assets/sass/style.scss`

into:

- `assets/sass/style.css`

## Setup

Run once from the project root:

```bash
npm install
```

## Commands

Build CSS one time:

```bash
npm run css:build
```

Watch SCSS and rebuild automatically on changes:

```bash
npm run css:watch
```

## Typical workflow

1. Edit any partial in `assets/sass/common` or `assets/sass/shortcode`.
2. Keep `npm run css:watch` running while you work.
3. Refresh the browser to see changes.

## Notes

- `assets/sass/style.scss` imports all section partials.
- If you stop watch mode, run `npm run css:build` once before publishing.
