# Spencer Lab website

A minimal Jekyll site for the Spencer Lab, styled with Stanford's
official brand colors (Cardinal Red, Cool Gray, Black, white) plus
Palo Alto Green as the accent.

## Editing content (no HTML needed for routine updates)

| To change...           | Edit this file              |
|-------------------------|------------------------------|
| Lab name, nav links, footer/contact info | `_config.yml` |
| Landing page headline & intro text | `index.html` (top section only) |
| Research focus areas    | `_data/research.yml` |
| Lab news items          | `_data/news.yml` |
| People / roster         | `_data/people.yml` |
| Colors, fonts, spacing  | `assets/css/style.css` (top of file has all color/font variables) |
| Person photos           | drop image in `assets/images/people/`, reference it in `_data/people.yml` |

Each `_data/*.yml` file is a simple list — copy an existing block,
paste it, and edit the text to add a new entry. No need to touch any
HTML file for these.

## Preview locally (optional but recommended)

You'll need Ruby installed. Then, from this folder:

```bash
gem install bundler jekyll
jekyll serve
```

Open `http://localhost:4000/spencer_lab/` in your browser. It rebuilds
automatically while `jekyll serve` is running — just save a file and
refresh.

## Publish to GitHub Pages

1. Push this folder's contents to `https://github.com/gargollo/spencer_lab`
   (main branch, root of repo).
2. On GitHub: go to the repo → **Settings** → **Pages**.
3. Under "Build and deployment", set **Source** to "Deploy from a branch",
   branch `main`, folder `/ (root)`. Save.
4. Wait a minute or two, then your site is live at:
   `https://gargollo.github.io/spencer_lab/`

Because `_config.yml` already has `baseurl: "/spencer_lab"` set to
match the repo name, all internal links and asset paths will resolve
correctly once it's live — you don't need to change anything else for
deployment to work.

## Placeholder content

Every page currently has a dashed placeholder-note box and generic
text/photos. Once real content is ready, remove the placeholder-note
`<div>` blocks and fill in the real copy — everything is set up so
that's a content swap, not a redesign.
