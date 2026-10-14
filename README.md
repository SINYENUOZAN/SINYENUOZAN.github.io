# LI's Personal Site

This repository contains a GitHub Pages site built with Jekyll and the Minimal Mistakes theme.

## Local preview

```bash
git checkout feature/minimal-mistakes

docker run --rm -it \
  -v "$PWD":/srv/jekyll \
  -p 4000:4000 \
  jekyll/jekyll:4 \
  jekyll serve --watch
```

Then open http://localhost:4000

## Deploy to GitHub Pages

In the repository settings:
1. Go to Settings -> Pages
2. Set Source to Branch: feature/minimal-mistakes
3. Save and wait for GitHub to build the site

## Notes

- The current site uses preview.jpg as a temporary placeholder.
- Replace the placeholder content with your actual project images and text.
