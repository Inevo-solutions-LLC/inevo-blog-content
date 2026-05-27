# InEvo Blog Content

This repo holds the markdown source and images for blog posts published on [inevo.ai/blog](https://inevo.ai/blog).

Content is authored through the Sveltia CMS at [inevo.ai/admin](https://inevo.ai/admin/) — writers should not edit files here directly.

## Structure

- `content/blog/*.md` — one markdown file per blog post (frontmatter + body)
- `blog-images/*` — cover images and inline images referenced by posts

## How publishing works

1. A writer creates or edits a post at [inevo.ai/admin](https://inevo.ai/admin/)
2. Sveltia CMS commits the change to this repo's `main` branch
3. A workflow in this repo dispatches an event to the main website repo
4. The main website rebuilds, pulls the latest content from this repo, and deploys to inevo.ai
