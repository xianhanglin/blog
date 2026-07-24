# Xianhang Lin — Blog

Personal tech blog built with [Astro](https://astro.build), deployed on [Vercel](https://vercel.com).

## Local development

```sh
bun install
bun dev
```

Open [http://localhost:4321](http://localhost:4321).

| Command         | Action                                      |
| :-------------- | :------------------------------------------ |
| `bun install`   | Install dependencies                        |
| `bun dev`       | Dev server at `localhost:4321`              |
| `bun build`     | Production build to `./dist/`               |
| `bun preview`   | Preview the production build locally        |

## Deploy to Vercel (Hobby / free)

1. Push this repo to GitHub.
2. Sign in at [vercel.com](https://vercel.com) with GitHub.
3. **Add New Project** → import this repository.
4. Leave the defaults (Vercel detects Astro). Framework preset: **Astro**. Build: `bun run build` or `npm run build`. Output: `dist`.
5. Deploy. You’ll get a URL like `https://your-project.vercel.app`.

After the first deploy, set `site` in `astro.config.mjs` to that URL (needed for canonical links, sitemap, and RSS), then push again.

Every later push to the connected branch redeploys automatically.

## Writing posts

Add Markdown or MDX under `src/content/blog/`. Frontmatter:

```yaml
title: 'Post title'
description: 'Short summary'
pubDate: 'Jul 24 2026'
heroImage: '../../assets/posts/your-image.png' # optional
```

## Credit

Theme based on the [Astro blog starter](https://github.com/withastro/astro/tree/main/examples/blog) / [Bear Blog](https://github.com/HermanMartinus/bearblog/).
