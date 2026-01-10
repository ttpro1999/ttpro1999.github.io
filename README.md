# C_ultra - Kernel Engineering Blog

Welcome to the **C_ultra Kernel Engineering Blog** - exploring RTOS, system design, and data structures from first principles.

## About

This is the public blog for the C_ultra project, featuring engineering essays on:
- Single Linked List (SLL)
- Doubly Linked List (DLL) with Intrusive Pattern
- Circular Linked Lists
- Kernel design and architecture
- Real-Time Operating Systems (RTOS)
- Data structure implementation with focus on kernel-level constraints
- ISR latency and deterministic design

## GitHub Pages

This repository hosts static HTML generated from Hugo. Blog content is deployed automatically to GitHub Pages.

### Viewing the Blog

Visit: **https://ttpro1999.github.io**

Or locally, open `articles/` folder and view `.html` files directly.

Once deployed, the blog will be available at: `https://ttpro1999.github.io/embedded_bootcamp`

### Local Development

To run the blog locally:

1. Install Ruby and Bundler
2. Clone this repository
3. Install dependencies:
   ```bash
   bundle install
   ```
4. Run Jekyll locally:
   ```bash
   bundle exec jekyll serve
   ```
5. Open your browser to `http://localhost:4000`

## Structure

- `_config.yml` - Jekyll configuration
- `_posts/` - Blog posts (named with format: YYYY-MM-DD-title.md)
- `index.md` - Homepage
- `about.md` - About page
- `.github/workflows/jekyll.yml` - GitHub Actions workflow for deployment

## Contributing

Feel free to suggest improvements or report issues!

## License

Content is available for educational purposes.
