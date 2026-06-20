# [sunilbastola.github.io](https://sunilbastola.github.io)

Personal site and blog. Astro, GitHub Pages, CloudFlare DNS.

## Structure

```
src/
  components/        # Header, Footer, PostList, ReadingProgress, TableOfContents
  content/blog/      # Markdown posts (Zod-validated frontmatter)
  layouts/           # BaseLayout, PostLayout
  pages/             # index, blog/index, blog/[...slug]
  styles/global.css  # Design tokens, dark/light themes
```

## Dev

```sh
npm install
npm run dev      # localhost:4321
npm test         # vitest
npm run build    # dist/
```

## Deploy

Push to `main` triggers GitHub Actions build and deploy.
