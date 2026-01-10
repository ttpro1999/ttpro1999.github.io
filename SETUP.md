# GitHub Pages Setup Instructions

This guide will help you enable GitHub Pages for your blog.

## Step 1: Enable GitHub Pages

1. Go to your repository on GitHub: `https://github.com/ttpro1999/embedded_bootcamp`
2. Click on **Settings** (gear icon at the top)
3. In the left sidebar, click on **Pages**
4. Under **Source**, select **GitHub Actions** (recommended) or **Deploy from a branch**

### Option A: GitHub Actions (Recommended)

If you select GitHub Actions:
- The workflow file `.github/workflows/jekyll.yml` is already configured
- Every push to `main` or `master` branch will automatically build and deploy your blog
- You can also manually trigger the workflow from the Actions tab

### Option B: Deploy from a branch

If you prefer to deploy from a branch:
1. Select **Deploy from a branch**
2. Choose the branch (e.g., `main` or `master`)
3. Select the `/ (root)` folder
4. Click **Save**

## Step 2: Wait for Deployment

- If using GitHub Actions, go to the **Actions** tab to monitor the deployment
- The first deployment might take a few minutes
- Once complete, your site will be available at: `https://ttpro1999.github.io/embedded_bootcamp`

## Step 3: Verify Your Blog

Visit `https://ttpro1999.github.io/embedded_bootcamp` to see your blog live!

## Adding New Blog Posts

To add new blog posts:

1. Create a new file in the `_posts/` directory
2. Name it following the format: `YYYY-MM-DD-title-of-post.md`
3. Add front matter at the top:
   ```yaml
   ---
   layout: post
   title: "Your Post Title"
   date: YYYY-MM-DD HH:MM:SS +0000
   categories: category1 category2
   ---
   ```
4. Write your content in Markdown below the front matter
5. Commit and push to GitHub
6. Your post will automatically appear on the blog!

## Customization

### Changing the Theme

Edit `_config.yml` and change the `theme:` line to use a different [GitHub Pages supported theme](https://pages.github.com/themes/).

### Updating Site Information

Edit `_config.yml` to update:
- `title`: Your blog title
- `description`: Your blog description
- `author`: Your name/username
- `url`: Your GitHub Pages URL

### Adding Pages

Create new `.md` files in the root directory with front matter:
```yaml
---
layout: page
title: "Page Title"
permalink: /page-url/
---
```

## Troubleshooting

### Blog not showing up
- Make sure GitHub Pages is enabled in repository settings
- Check the Actions tab for any build errors
- Verify the workflow has permissions to deploy

### Posts not appearing
- Check the date in the post filename and front matter
- Ensure the filename follows the `YYYY-MM-DD-title.md` format
- Posts dated in the future won't appear until that date

### Build errors
- Check the Actions tab for detailed error messages
- Verify all YAML front matter is properly formatted
- Ensure there are no syntax errors in Markdown files

## Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Markdown Guide](https://www.markdownguide.org/)
- [Jekyll Themes](https://jekyllrb.com/docs/themes/)

## Local Development

To run the blog locally:

1. Install Ruby (version 2.7 or higher)
2. Install Bundler: `gem install bundler`
3. Install dependencies: `bundle install`
4. Run Jekyll: `bundle exec jekyll serve`
5. Visit `http://localhost:4000` in your browser

Happy blogging! 🚀
