# Projects

This repository serves multiple purposes: it contains the template for your **thesis**, backs-up your any **paper** we en up submitting, and contains an optional **project page** (Markdown or HTML) relevant to your project. The file/folder naming convention used in this repository is important due to several automations. This repository will be linked to an overleaf project where you will do most of the editing.

## Structure

```
my-project/
  paper_<venue>.tex       # paper source (or main_<venue>.tex for multi-venue)
  thesis.tex              # thesis document (master/bachelor/semester project report following DISCO guidelines)
  proposal.tex            # project proposal
  references.bib          # bibliography
  author_kit_<venue>/     # conference style files and templates (DO NOT TOUCH)
  author_kit_thesis/      # thesis-specific style files and templates (DO NOT TOUCH)
  assets/                 # all figures, images, videos, and other media for the tex and md files
  page.md                 # project page content (Markdown or HTML)
  build/                  # compilation output (git-ignored, for local latex compilation)
```

- **`paper.tex`** is the paper source. Use `main_<venue>.tex` when targeting multiple venues or resubmitting. Please read [this guide](https://fberdoz.github.io/teaching/paper-writing-guide/) before writing anything.
- **`thesis.tex`** is the thesis or semester/master project report. Uses style files from `author_kit_thesis/`.
- **`proposal.tex`** is the project proposal, typically written before the main work begins.
- **`*.tex`** other optional tex files, such as `poster.tex`, `slides.tex`, etc. relevant for the project.
- **`references.bib`** is shared across venues; keep one copy at the root. Each bibtex entry should follow [these guidlines](https://fberdoz.github.io/teaching/bibtex-guide/).
- **`author_kit_<venue>/`** holds style files for each target venue.
- **`author_kit_thesis/`** holds thesis-specific style files and templates (e.g., university formatting requirements).
- **`assets/`** holds all media (paper figures, web images, videos). Reference them with relative paths: `assets/figure.pdf`.
- **`page.md`** (or `page.html`) is your project page. Write body content only, no frontmatter. Metadata (title, authors, venue, abstract, etc.) is added automatically by the website template.
- **`build/`** must be git-ignored. This is for compilation artifacts when compiling LaTeX locally.

## `page.md` template
Below is a simple `page.md` template. You can find an example of the final rendering [here](https://fberdoz.github.io/projects/sd-square/). The header (links) and footer (citation) information will be handled automatically, you just have to care about the content.
```markdown
## Overview

Brief description of the project and its contributions.

## Method

![Method overview](assets/method.pdf)

Explain the approach here.

## Results

![Main results](assets/results.pdf)

Summarize the key findings.

## Acknowledgements

This work was supported by ...
```
