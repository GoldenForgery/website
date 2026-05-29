---
name: new-post
description: Scaffold a new Hugo post under content/posts/ with the project's TOML frontmatter. Use when the user asks to create a post, blog entry, or article. Pass the desired slug (kebab-case) as the argument.
---

# new-post

Scaffold a new Hugo post and open it for editing.

## Steps

1. Take the slug from `$ARGUMENTS`. If empty, ask the user for one. Normalize to kebab-case (lowercase, hyphens between words, no extension).
2. Run `hugo new content/posts/<slug>.md` from the project root. This uses `archetypes/default.md`, which sets `draft = true`, `date`, and a titlecased `title` derived from the slug.
3. Read the generated file and show its current frontmatter to the user.
4. Ask the user for the post title (if it should differ from the auto-titlecased one) and any tags/categories. Update the frontmatter accordingly — keep it TOML (`+++` delimiters), do not switch to YAML.
5. Leave `draft = true` so it doesn't ship by accident; remind the user to flip it to `false` and update `date` when ready to publish.
6. Tell the user how to preview it: `hugo server -D` (the `-D` flag is required to render drafts).

## Notes

- Posts live under `content/posts/`. Other content types (e.g., standalone pages) go directly under `content/`.
- Don't edit `archetypes/default.md` to change a single post's frontmatter — that file is the template for *all* new posts.
