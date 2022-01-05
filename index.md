---
layout: page
katex:
  macros:
    "\\MyLocalMacro": "\\LaTeX"
antex:
  preamble: >-
    \usepackage{amsmath,amsfonts}
    \usepackage{commutative-diagrams}
---

**Welcome to `krater`!**

This is a template for the static website generator [Jekyll][jekyll-url].

Its purpose is setting up all the plumbing needed by a modern math-intensive website:

- client side rendering of ordinary LaTeX with [KaTeX][katex-url]
- server side rendering of **arbitrarily complex** LaTeX with [AnTeX][antex-url] via [`jekyll-antex`][jekyll-antex-url]
- a nice automatic deploy running on [GitHub Actions][gha-url] to host the website on [GitHub Pages][ghp-url].

You can get going in no time!
All details are in the [readme][readme-url].

[jekyll-url]: https://jekyllrb.com/
[katex-url]: https://katex.org/
[antex-url]: https://github.com/paolobrasolin/antex/
[jekyll-antex-url]: https://github.com/paolobrasolin/jekyll-antex/
[gha-url]: https://github.com/features/actions
[ghp-url]: https://pages.github.com/
[readme-url]: https://github.com/paolobrasolin/krater#readme

The remainder of this page is a demo.

A pretty formula:

$$ F([n]) = \coprod*{i=1}^n F([1]) = \coprod*{i=1}^n X = [n] \otimes X $$

A pretty diagram:

{% tex classes: [antex, display] %}
\begin{codi}
\obj{ A & B \\ C & D \\ };
\mor A -> B -> D;
\mor A -> C -> D;
\end{codi}
{% endtex %}
