# csshah.com

Swapnil Shah's personal site. Built with [Hugo](https://gohugo.io/) using the [hugo-xmin](https://github.com/yihui/hugo-xmin) theme, deployed via Cloudflare Workers Static Assets.

## Local development

```sh
hugo server
```

Open http://127.0.0.1:1313/.

## New post

```sh
hugo new content post/2026-mm-dd-my-post.md
```

Or create the file manually under `content/post/` with frontmatter:

```yaml
---
title: "My post"
date: 2026-05-18
---
```

## Deploy

Pushed commits on `master` are built and deployed automatically by Cloudflare. Local build:

```sh
hugo --minify        # writes to ./public
npx wrangler deploy  # uploads ./public to Cloudflare Workers
```
