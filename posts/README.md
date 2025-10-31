# Blog Setup Guide

## MDX vs MD: Which Should You Use?

### Current Setup (Static HTML)
Your site is currently a simple static HTML site hosted on GitHub Pages. This means:

- **MDX requires a build step**: MDX files need to be compiled to HTML/JS, which requires a build tool like Next.js, Astro, or a custom script
- **MD files can work with static site generators**: Tools like Jekyll (natively supported by GitHub Pages) can process `.md` files

### Recommendations

#### Option 1: Use `.md` files with Jekyll (Easiest for GitHub Pages)
Jekyll is natively supported by GitHub Pages and can process Markdown files automatically:

1. Create a `_config.yml` file
2. Place `.md` files in a `_posts` directory
3. Jekyll will automatically compile them to HTML

**Pros:**
- No build step needed (GitHub Pages handles it)
- Easy to write and maintain
- Syntax highlighting, code blocks work out of the box

**Cons:**
- No React components in your posts
- Less flexible than MDX

#### Option 2: Use MDX with a Build System
If you want to use React components in your blog posts:

1. **Next.js** - Full React framework, great for blogs
2. **Astro** - Fast, content-focused, can use MDX
3. **Custom build script** - Use `@mdx-js/mdx` to compile MDX to HTML

**Pros:**
- Can use React components in posts
- More interactive posts possible
- Modern developer experience

**Cons:**
- Requires a build step
- More complex setup
- May need to deploy differently (or use GitHub Actions)

#### Option 3: Use `.md` files with a simple markdown parser
For now, you can use plain `.md` files and convert them manually or with a simple script:

1. Write posts in `.md` format
2. Use a markdown-to-HTML converter (like `marked` or `markdown-it`)
3. Generate HTML files

### My Recommendation

Since you're already on GitHub Pages, I'd suggest **starting with `.md` files and Jekyll**. It's the simplest path and works perfectly for most blog posts. You can always migrate to MDX later if you need React components in your posts.

### Next Steps

1. If using Jekyll:
   - Create `_config.yml`
   - Create `_posts/` directory
   - Add `.md` files with frontmatter

2. If using MDX:
   - Set up a build system (Next.js/Astro recommended)
   - Create a build script
   - Set up GitHub Actions to build and deploy

3. For now (simple approach):
   - Write posts in `.md` format
   - Manually convert to HTML or use a simple script
   - Place HTML files in `posts/` directory

## Example Blog Post Structure

Create posts in `posts/` directory with this structure:

```
posts/
  my-first-post.html (or .md if using Jekyll)
  another-post.html
```

Each post should link from `writing.html`.

