# AI Agent Instructions for Blog Codebase

This is a Jekyll-based blog using the Hydejack theme. Here's what you need to know to work effectively with this codebase:

## Project Structure

- `_posts/` - Blog posts in Markdown format with YAML front matter
- `_data/` - Data files (including resume.markdown)
- `assets/` - Static assets including images
- `_config.yml` - Main Jekyll configuration

## Key Workflows

### Local Development
```bash
bundle install     # Install dependencies
bundle exec jekyll serve  # Run development server
```

### Content Creation

1. Blog Posts
   - Create files in `_posts/` following format: `YYYY-MM-DD-title.markdown`
   - Required front matter:
     ```yaml
     ---
     layout: post
     title: "Post Title"
     date: YYYY-MM-DD HH:MM:SS -0700
     categories: category1 category2
     ---
     ```

2. Images
   - Store in `assets/images/` or `assets/img/`
   - Reference in posts using: `![alt text](/assets/images/filename.ext)`

## Configuration

- Site settings are in `_config.yml`
- Key settings:
  - `title`, `email`, `description`
  - `baseurl` and `url` for deployment
  - Theme configuration (Hydejack)

## Jekyll-Specific Patterns

1. Liquid Templates
   - Use `{% %}` for logic
   - Use `{{ }}` for output
   - Example: `{% highlight ruby %}...{% endhighlight %}`

2. Code Snippets
   - Use fenced code blocks with language
   - Or use Jekyll's highlight tags for more features

## Theme Details

- Using Hydejack theme (`jekyll-theme-hydejack`)
- Theme customization should be done through Jekyll's override system
- Custom styles can be added in `assets/` directory

## Common Tasks

1. Adding a new post
2. Updating site configuration
3. Managing static assets
4. Modifying layout templates

For detailed Jekyll documentation, refer to https://jekyllrb.com/docs/