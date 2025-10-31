# Jekyll Setup Complete! 🎉

## How to Use

### Writing New Blog Posts

1. Create a new file in `_posts/` directory
2. Use the format: `YYYY-MM-DD-post-title.md`
3. Add frontmatter at the top:

```markdown
---
layout: post
title: "Your Post Title"
date: 2025-01-15
---

Your content here...
```

### Example Post Structure

See `_posts/2025-01-15-example-post.md` for a complete example.

### Testing Locally

To test your site locally before pushing to GitHub:

1. Install Jekyll: `gem install bundler && bundle install`
2. Run locally: `bundle exec jekyll serve`
3. Visit: `http://localhost:4000`

### Deploying

Just push to GitHub! GitHub Pages will automatically:
- Process your Markdown files
- Generate HTML
- Deploy your site

### File Structure

- `_posts/` - Your blog posts (Markdown files)
- `_layouts/` - HTML templates
- `_config.yml` - Jekyll configuration
- `index.md` - Homepage
- `writing.md` - Writing/blog listing page

### Converting from HTML to Markdown

If you have existing HTML posts in `posts/`, you can:
1. Convert them to Markdown
2. Move them to `_posts/` with the correct naming format
3. They'll automatically appear on the writing page!

