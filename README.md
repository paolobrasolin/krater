# krater

<img align="right" width="192px" alt="Terracotta calyx-krater, ca. 460–450 B.C. Source: https://www.metmuseum.org/art/collection/search/247966" src="https://github.com/paolobrasolin/krater/raw/main/krater.png">

This is a template to start building math-rich websites effortlessly.

Ancient Greeks placed large vessels named _kraters_ at the center of the room during a symposium.
An elected _symposiarch_ would oversee the event by deciding the dilution of the wine in the krater and timing refills.
Meanwhile, other _symposyasts_ drank, talked, and enjoyed any pleasure the evening offered.

I hope this affords you to reproduce that, with ideas instead of wine.

## Getting started

1. Click [`Use this template`][krater-generate-url] here or at the top of this page.
2. Pick a name for your new repo and create it.
3. Wait for the first build to become green; you can observe its status at `> Actions > Publish`.
4. Enable GitHub Pages on branch `gh-pages` and folder `/`; you can reach the configuration panel at `> Settings > Pages`.

That's it! Your website is now visible at `https://<USER_NAME>.github.io/<REPO_NAME>/`

[krater-generate-url]: https://github.com/paolobrasolin/krater/generate

## Usage

This is a [Jekyll][jekyll-url] setup, so its excellent documentation fully applies.

Schematically, this is what `krater` gives you:

- A [KaTeX][katex-url] setup composed of:
  - a custom page header in `custom-head.html`
  - a default configuration at `katex` in `_config.yml`
- An [AnTeX][antex-url] setup composed of:
  - the [`jekyll-antex`][jekyll-antex-url] gem in `Gemfile`
  - a default configuration at `antex` in `_config.yml`
- A tweak to the `kramdown` configuration in `_config.yml` to let the previous components do their job.
- A [GitHub Action][gha-url] workflow which compiles and publishes your website on [GitHub Pages][ghp-url] everytime something is pushed to the `main` branch.

As long as you keep these pieces in place the math rendering machinery will work.

Let's review some common tasks now.

[jekyll-url]: https://jekyllrb.com/
[katex-url]: https://katex.org/
[antex-url]: https://github.com/paolobrasolin/antex/
[jekyll-antex-url]: https://github.com/paolobrasolin/jekyll-antex/
[gha-url]: https://github.com/features/actions
[ghp-url]: https://pages.github.com/

### Running on your machine

### Configuring CI

### Kickstarting a blog

### Kickstarting a course

### Kickstarting a book

### Plugins customization

It also installs [all Jekyll plugins available in GitHub Pages][ghp-jekyll-plugins-url] with the `github-pages` gem in `Gemfile`.
This will help you if you're used to the standard features of GitHub Pages.
You can add any other [Jekyll plugins][jekyll-plugins-url] you need.

[ghp-jekyll-plugins-url]: https://pages.github.com/versions/
[jekyll-plugins-url]: https://jekyllrb.com/docs/plugins/

### Theme customization

The default theme is [`minima`][minima-url] but you can easily change that as long as you ensure `custom-head.html` still gets included.

[minima-url]: https://github.com/jekyll/minima
