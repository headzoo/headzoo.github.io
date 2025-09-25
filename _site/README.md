# Jekyll site for headzoo.github.io

This was generated automatically from your ripped static site.

## What was done
- Common header & footer were detected and moved into `_layouts/default.html`
- Page bodies were inserted as `{{ content }}` with `layout: default`
- Disqus embeds (div#disqus_thread and scripts referencing disqus.com) were removed
- Non-HTML assets were copied with original paths
- A minimal `_config.yml` with `jekyll-seo-tag` plugin stub was added

## How to run locally
```bash
gem install bundler jekyll jekyll-seo-tag
jekyll serve
```
Then open http://127.0.0.1:4000

## Deploy to GitHub Pages
- Push this directory to your `headzoo.github.io` repo
- In Settings → Pages, choose "Deploy from a branch", branch `main`, folder `/ (root)`
- (Optional) Enable "Enforce HTTPS"

## Notes
- If some pages still include bits of header/footer, tweak `_layouts/default.html`:
  - You can move parts into `_includes/` and reference with `{% include %}` if you prefer
- If titles look wrong, edit each page's front matter `title:`
- If your site used client-side routes (SPA), each route now has a static file counterpart.
