# Resume — Joaquin Cardenas

LaTeX source for my resume. The PDF is rebuilt by GitHub Actions on every push and
committed back to this repository.

| File | What it is |
|---|---|
| `resume.tex` | Source. Harvard-style template by Jake Gutierrez (MIT), based on sb2nov/resume. |
| `resume.pdf` | Compiled output, one page, ATS-parseable. |

## Build locally

MiKTeX (Windows) or TeX Live:

```bash
pdflatex -interaction=nonstopmode resume.tex
```

The site **daelfame.github.io** pulls `resume.pdf` from this repository at build time,
so updating the CV here is enough — the portfolio picks it up on its next deploy.
