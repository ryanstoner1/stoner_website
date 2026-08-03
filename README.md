# stoner_website

Personal academic site and blog for Ryan K. Stoner, built with
[Hugo](https://gohugo.io/) and the [Blowfish](https://blowfish.page/) theme.

**Live at:** https://ryanstoner1.github.io/stoner_website/

## Local development

Hugo **extended** is required (Blowfish compiles SCSS):

```bash
brew install hugo          # macOS
hugo version               # must say "+extended"
```

Clone with the theme submodule, then serve with drafts visible:

```bash
git clone --recurse-submodules https://github.com/ryanstoner1/stoner_website.git
cd stoner_website
hugo server -D
```

The site is then at http://localhost:1313/stoner_website/ — note the subpath.

If you already cloned without `--recurse-submodules`:

```bash
git submodule update --init --recursive
```

## Adding a blog post

```bash
hugo new blog/my-post-slug/index.md
```

Then edit `content/blog/my-post-slug/index.md`. Set `draft: false` when it's ready to
publish. Images for a post go in that same folder next to `index.md`.

## Layout

```
config/_default/     site config (hugo, params, menus, languages)
content/
  _index.md          homepage bio
  research/          research overview
  publications/      papers, theses, abstracts
  blog/              posts, one folder each
  cv/                curriculum vitae
assets/img/          profile photo and other images
themes/blowfish/     theme (git submodule — do not edit)
```

## Deployment

Every push to `master` triggers `.github/workflows/hugo.yaml`, which builds the site and
publishes it to GitHub Pages. No manual step is needed.

To customize the theme, override files in the top-level `layouts/` or `assets/`
directories rather than editing `themes/blowfish/` — that way theme updates
(`git submodule update --remote`) won't clobber your changes.
