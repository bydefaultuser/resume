# resume

LaTeX source for Shiva Mishra's professional resume.

## Files

| File | Description |
|------|-------------|
| `main.tex` | LaTeX source — edit this |
| `main.pdf` | Compiled output (committed for convenience) |

## How to Compile

### Option 1 — Local LaTeX (recommended)

```bash
# macOS
brew install mactex

# Ubuntu / Debian
sudo apt-get install texlive-full

# Compile
pdflatex main.tex
```

### Option 2 — Overleaf

1. Create a free account at [overleaf.com](https://www.overleaf.com)
2. New Project → Upload Project → select this folder
3. Click Recompile

### Option 3 — Docker (no local install)

```bash
docker run --rm -v "$(pwd)":/workdir texlive/texlive pdflatex /workdir/main.tex
```

## Customising

All content lives in `main.tex`. The structure is:

- **Header** — name, title, contact links
- **Summary** — 2–3 sentence positioning statement
- **Experience** — `\entry{title}{company}{type}{dates}` + bullet list
- **Technical Skills** — tabular format
- **Open-Source Projects** — linked project entries
- **Education** — `\entry` macro

The accent colour is `#1A56DB` — change `\definecolor{accent}{HTML}{...}` to restyle.

## License

MIT
