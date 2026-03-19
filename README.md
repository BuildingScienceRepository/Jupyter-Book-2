# Building Science Atlas

[![Deploy MyST Site to GitHub Pages](https://github.com/BuildingScienceRepository/Jupyter-Book-2/actions/workflows/deploy.yml/badge.svg)](https://github.com/BuildingScienceRepository/Jupyter-Book-2/actions/workflows/deploy.yml)

Welcome to the Building Science Atlas! This is a collaborative, open-source repository and wiki compiling the current state of sustainability analysis for building science and urban analysis.

## Goals

1.  **Collaborative Knowledge Base:** A place for students, researchers, and professionals to contribute and learn.
2.  **Systems & Complexity Perspective:** Explore topics from simple ballpark estimations to complex simulations (e.g., Energy Balance, Neural Nets, Eddy3D, Urbano).
3.  **Theory & Code:** Combine theoretical explanations with executable workflows and examples.

## How to Contribute

This project is built using [MyST Markdown](https://mystmd.org/) (the engine behind Jupyter Book 2) and deployed via GitHub Actions.

1.  Fork the repository.
2.  Add or edit content in `chapters/` (Markdown files) or `notebooks/` (Jupyter Notebooks).
3.  Submit a Pull Request.

All changes to the `main` branch are automatically built and deployed to GitHub Pages.

## PDF outputs

Every content page in the MyST table of contents defines its own page-level PDF export and download button (`Download This Page (PDF)`) with a unique export ID and output path.

The project configuration in `myst.yml` also defines a `full-book-pdf` export with an explicit `articles` list so the deployed site exposes a single concatenated PDF containing all TOC pages.

The GitHub Pages workflow builds both the site and PDF artifacts automatically on each push to `main`.
