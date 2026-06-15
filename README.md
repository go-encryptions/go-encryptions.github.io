<p align="center"><img src="static/img/logo.svg" alt="go-encryptions" width="120"></p>

# go-encryptions.github.io

Sources for **[go-encryptions.github.io](https://go-encryptions.github.io)** —
the go-encryptions org landing page. Built with [Hugo](https://gohugo.io),
using the same self-contained single-`index.html` template shape as the
sibling [go-compressions](https://github.com/go-compressions/go-compressions.github.io)
landing.

## Layout

```text
.
├── hugo.toml                 Site config + per-repo card params
├── content/
│   └── _index.md             Homepage marker (empty)
├── layouts/
│   └── index.html            Homepage (inline CSS, light/dark, repo grid)
└── static/
    ├── favicon.svg           Org favicon
    └── img/logo.svg          Hero logo (88px)
```

## Build locally

```sh
hugo server -D          # live reload at http://localhost:1313/
hugo --gc --minify      # production build → ./public/
```

## Deploy

`.github/workflows/hugo.yml` builds and deploys on every push to `main`.
Configure GitHub Pages on the repo with **Source = "GitHub Actions"**
(not "Deploy from a branch").
