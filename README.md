# Resume — Joaquin Cardenas

LaTeX source for my resume, in English and Spanish. The PDFs are rebuilt by GitHub
Actions on every push and committed back to this repository.

| File | What it is |
|---|---|
| `resume-en.tex` | English source. Harvard-style template by Jake Gutierrez (MIT), based on sb2nov/resume. |
| `resume-es.tex` | Spanish source. Same template, same layout — only the language changes. |
| `resume-en.pdf` | Compiled English output, one page, ATS-parseable. |
| `resume-es.pdf` | Compiled Spanish output, one page. |

Both files share the same preamble, margins and type size, so the two CVs look
structurally identical.

## Build locally

MiKTeX (Windows) or TeX Live:

```bash
pdflatex -interaction=nonstopmode resume-en.tex
pdflatex -interaction=nonstopmode resume-es.tex
```

The site **daelfame.github.io** pulls `resume-en.pdf` and `resume-es.pdf` from this
repository at build time, so updating the CV here is enough — the portfolio picks it up
on its next deploy.
