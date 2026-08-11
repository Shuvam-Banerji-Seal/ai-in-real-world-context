# AI in Real World Context

A 60-minute presentation on **AI in the real world** — the tools, the services,
and the next-token predictors underneath the hype. Two flavours of the same deck:

- **HTML deck** (`index.html`) — the live, pointer-friendly slide deck, served on GitHub Pages.
- **LaTeX Beamer** (`main.tex` + `sections/`) — the same content compiled with `pdflatex`, styled by `sbs_dark_beamer.sty`.

Built by [Shuvam Banerji Seal](https://github.com/Shuvam-Banerji-Seal) —
BS–MS final-year student at IISER Kolkata (Chemistry major, Computer Science
minor), researching Information Retrieval (RAG, BM25, TREC, ECIR'26).

## Features

- **26 slides** — prologue → agenda → tool time → AI landscape → fundamentals →
  knowledge compression → tools you should learn → agentic tools.
- **Pointer-friendly deck** — reveal each point one by one with a click, `→` or
  `Space`; click the left edge to step back.
- **Keyboard shortcuts** — press `?` for the full help overlay, `O` for the
  overview grid, `F` for fullscreen, or type a slide number to jump.
- **Real logos & memes** — Git, GitHub, GitLab, Codeberg, LaTeX, Overleaf,
  Python, Docker, OpenAI, ChatGPT, Anthropic, Gemini, HuggingFace, plus a
  curated set of memes and xkcd comics.
- **Diagrams drawn in-code** — the three circles of knowing, the AI umbrella,
  next-token distribution, services flow, knowledge compression, and the
  agent loop (SVG in the HTML deck, TikZ in the LaTeX deck).
- Dark, high-contrast theme.

## Quick start

### View the HTML deck

Open `index.html` in any browser, or visit the live site:
<https://shuvam-banerji-seal.github.io/ai-in-real-world-context/>

### Read the compiled PDF

A compiled copy of the LaTeX deck is committed to the repo:

- [`main.pdf`](main.pdf) — also served at
  <https://shuvam-banerji-seal.github.io/ai-in-real-world-context/main.pdf>

### Compile the LaTeX deck

Requires a TeX distribution with `pygments` (used by `minted`) and the packages
listed in `sbs_dark_beamer.sty`.

```sh
pdflatex -shell-escape main.tex   # run twice so the table of contents settles
```

The same project is mirrored on Overleaf.

## Repository structure

```
.
├── index.html              # HTML deck (GitHub Pages entry point)
├── main.tex                # LaTeX deck entry point
├── sbs_dark_beamer.sty     # custom dark Beamer theme
├── sections/               # one LaTeX file per group of slides
│   ├── 01_prologue.tex     #   title-question, Real → Current
│   ├── 02_agenda.tex       #   venn diagram, the goal
│   ├── 03_tooltime.tex     #   what kind of tools, are they AI?
│   ├── 04_ailandscape.tex  #   umbrella, next-token, lens, axis, alignment
│   ├── 05_fundamentals.tex #   services, about me, storage, all text
│   ├── 06_knowledge.tex    #   compression, distribution, too much math
│   ├── 07_tools.tex        #   git, latex, do it yourself?
│   └── 08_agents.tex       #   agentic tools
└── assets/
    ├── img/                # logos, memes, xkcd comics (used by both decks)
    └── xkcd_*.json         # xkcd metadata
```

## Presenting

- **HTML**: press `F` to go fullscreen, `?` for shortcuts, `O` for the slide grid.
- **LaTeX**: `\pause` reveals points step by step; section pages auto-insert between parts.

## License

[MIT](LICENSE) © Shuvam Banerji Seal
