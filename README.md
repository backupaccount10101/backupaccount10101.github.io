# Security Notes

Source for a security research blog: vulnerability writeups, exploitation mechanics, and defensive engineering notes. Built with Astro, deployed to GitHub Pages.

## Structure

- `src/content/blog/` — posts, in Markdown
- `src/pages/` — routes (home, blog index, about, RSS feed)
- `src/components/` — shared layout components (header, footer, head)
- `astro.config.mjs` — site configuration

## Development

```
npm install
npm run dev
```

Runs at `http://localhost:4321`.

## Build

```
npm run build      # output to ./dist
npm run preview    # preview the production build locally
```

## Deployment

Pushing to `master` triggers `.github/workflows/deploy.yml`, which builds the site and publishes it to GitHub Pages.

## Adding a post

Add a Markdown file to `src/content/blog/` with `title`, `description`, and `pubDate` frontmatter.
