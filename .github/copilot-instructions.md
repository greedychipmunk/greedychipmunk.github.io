# GitHub Copilot Instructions

## Project Overview
This is a personal Jekyll-based GitHub Pages website hosted at greedychipmunk.github.io. The site uses Jekyll 4.4.1 with the jekyll-theme-dinky theme to generate static content.

## Tech Stack
- **Static Site Generator**: Jekyll 4.4.1
- **Theme**: jekyll-theme-dinky (v0.2.0)
- **Plugins**: 
  - jekyll-feed (v0.12)
  - jekyll-timeago (v0.13.1)
- **Language**: Ruby
- **Hosting**: GitHub Pages

## Project Structure
- `_posts/`: Blog posts in Markdown format (filename: YYYY-MM-DD-title.markdown)
- `_sass/`: Sass stylesheets for theme customization
- `_config.yml`: Main Jekyll configuration file
- `assets/`: Static assets (CSS, images, etc.)
- `index.markdown`: Homepage content
- `about.markdown`: About page content
- `resume.html`: Resume page
- `fiftytwolearn.html`: Custom page
- `Gemfile`: Ruby dependencies

## Development Commands
- **Install dependencies**: `bundle install`
- **Build site**: `bundle exec jekyll build`
- **Serve locally**: `bundle exec jekyll serve` (available at http://localhost:4000)
- **Clean build artifacts**: `bundle exec jekyll clean`

## Coding Standards

### Jekyll & Markdown
- Follow Jekyll's front matter conventions (YAML between `---` delimiters)
- Blog posts must be named `YYYY-MM-DD-title.markdown` and placed in `_posts/`
- Use Markdown for content pages, HTML only when necessary
- Always include proper front matter (layout, title, permalink, etc.)

### File Naming & Structure
- Markdown files use `.markdown` extension (not `.md`)
- Keep consistent front matter structure across similar page types
- Place theme customizations in `_sass/` directory
- Store static assets in `assets/` directory

### Configuration
- **CRITICAL**: Be extremely careful when modifying `_config.yml` as it affects the entire site
- Always test configuration changes locally before committing
- Preserve existing plugin configurations

### Git & Version Control
- Do NOT commit build artifacts (handled by `.gitignore`):
  - `_site/`
  - `.sass-cache/`
  - `.jekyll-cache/`
  - `.jekyll-metadata`
  - `vendor/`
  - `.bundle/`
  - `Gemfile.lock`

## Best Practices
1. **Test locally**: Always run `bundle exec jekyll serve` to test changes before committing
2. **Validate Markdown**: Ensure all Markdown is properly formatted
3. **Check links**: Verify internal and external links work correctly
4. **Front matter**: Always include required front matter fields
5. **Preserve theme**: Avoid breaking theme functionality when customizing styles
6. **Dependencies**: Only update gems when absolutely necessary; test thoroughly

## Common Tasks

### Adding a New Blog Post
1. Create file in `_posts/` with format `YYYY-MM-DD-title.markdown`
2. Add front matter:
   ```yaml
   ---
   layout: post
   title: "Your Post Title"
   date: YYYY-MM-DD HH:MM:SS +/-TTTT
   categories: [category1, category2]
   ---
   ```
3. Write content in Markdown below front matter
4. Test with `bundle exec jekyll serve`

### Adding a New Page
1. Create `.markdown` file in root directory
2. Add front matter with layout, title, and permalink
3. Write content in Markdown
4. Update navigation if needed

### Customizing Styles
1. Add/modify files in `_sass/` directory
2. Follow existing Sass structure
3. Test across different browsers and screen sizes

## Prohibited Actions
- Never delete or significantly modify `_config.yml` without explicit instructions
- Do not remove or modify `vendor/`, `.bundle/`, or other dependency directories
- Do not commit build artifacts listed in `.gitignore`
- Avoid breaking changes to the theme without thorough testing
- Do not modify core theme files unless creating intentional overrides

## Helpful Resources
- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Jekyll Theme Dinky](https://github.com/pages-themes/dinky)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Markdown Guide](https://www.markdownguide.org/)
