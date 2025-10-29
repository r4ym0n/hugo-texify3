# TeXify3

> A LaTeX-style hugo theme with the gruvbox color scheme for personal blogging

[![Hugo](https://img.shields.io/badge/hugo-0.115.1-blue.svg)](https://gohugo.io)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Hugo](https://github.com/michaelneuper/hugo-texify3/actions/workflows/hugo.yml/badge.svg)](https://github.com/michaelneuper/hugo-texify3/actions/workflows/hugo.yml)

![texify-light](https://github.com/michaelneuper/hugo-texify3/assets/73108749/8b006060-939f-4f11-b597-8ff1861fce90)
![texify-dark](https://github.com/michaelneuper/hugo-texify3/assets/73108749/77d34466-037c-4402-94e3-019d5b2122e5)

## Features

- Any comment engine (giscus, remark42, hyvor, etc.)
- [Mermaid](https://mermaid.js.org) support
- Built-in site search with [Fuse.js](https://fusejs.io/) - fast, fuzzy search across all content
- Buymeacoffee widget
- Auto numbered subtitles
- [Disqus](https://disqus.com/) & Google Analytics
- Render math equations with [KaTeX](https://katex.org/)
- [PostCSS](https://postcss.org/) to make writing CSS easier
- Dark mode toggle
- Citations

Visit the [demo site](https://michaelneuper.github.io/hugo-texify3/).


![Lighthouse report](https://github.com/michaelneuper/hugo-texify3/assets/73108749/2bd66f9d-0c28-4ea5-acbc-d53e9078a2cd)

View full lighthouse report [here](https://pagespeed.web.dev/analysis/https-michaelneuper-github-io-hugo-texify3/c740roolxm?form_factor=desktop)

## Usage

```bash
git submodule add https://github.com/michaelneuper/hugo-texify3.git themes/hugo-texify3
```

Visit the [wiki](https://github.com/michaelneuper/hugo-texify3/wiki) for more information on how to install and configure.

See [`hugo.toml`](https://github.com/weastur/hugo-texify2/blob/master/hugo.toml)
for an example configuration.

### Search Configuration

The theme includes built-in search functionality powered by Fuse.js. To enable search:

1. Create a search page (e.g., `content/search.md`):
```markdown
---
title: "Search"
layout: "search"
---
```

2. Add search output to your site config:
```yaml
outputs:
  home:
    - HTML
    - RSS
    - JSON  # Required for search index
```

3. (Optional) Customize Fuse.js search options in your config:
```yaml
params:
  fuseOpts:
    isCaseSensitive: false
    includeScore: false
    shouldSort: true
    threshold: 0.4
    distance: 100
    ignoreLocation: true
    keys:
      - title
      - permalink
      - summary
      - content
```

The search page will automatically index all your content and provide fast, fuzzy search with keyboard navigation support.

## Acknowledgement

The following software inspires the design of this theme:

- <https://github.com/weastur/hugo-texify2>
- <https://github.com/vincentdoerig/latex-css>
- <https://github.com/7ma7X/HugoTeX>
- <https://theme.typora.io/theme/Academic/>
- <https://github.com/queensferryme/hugo-theme-texify>
- <https://sharingbuttons.io>

## Support

If you want to support the development or say thanks, become a GitHub Sponsor or

<a href="https://www.buymeacoffee.com/michaelneuper" target="_blank">
<img src="https://cdn.buymeacoffee.com/buttons/default-orange.png"
    alt="Buy Me A Coffee"
    height="41"
    width="174">
</a>
