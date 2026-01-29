# AGENTS.md

## Project overview
- This repo is a single LaTeX “living document” for exam notes.
- The source of truth is `ds-main.tex`. The PDF and aux/log files are build artifacts.

## Editing guidelines
- Add content under the existing section/subsection placeholders; avoid restructuring unless asked.
- Reuse the provided tcolorbox environments (`examlikelihood`, `examfavorite`, `pitfall`, `cheatsheet`, `visualbox`) for emphasis.
- Keep new additions concise and exam-focused; prefer bullet lists and short definitions.
- Avoid adding new LaTeX packages unless required; if you must, add them in the “Packages” block near the top.
- Do not manually edit generated files (`*.aux`, `*.log`, `*.out`, `*.toc`, `*.pdf`, `*.synctex.gz`).

## Build / compile
- From repo root: `pdflatex ds-main.tex` (run twice to refresh ToC links).
- Optional: `latexmk -pdf ds-main.tex` if available.

## Assets
- No asset folder currently. If figures/images are needed, create a `figures/` directory and reference it via `\includegraphics`.
