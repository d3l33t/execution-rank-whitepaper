# ExecutionRank Whitepaper

**Verified Multi-Agent Execution via Weighted Attestation and Threshold Acceptance**

This repository contains the LaTeX source for the *ExecutionRank* whitepaper and a GitHub Action that builds a PDF on every push.

## Build locally

### Option A: latexmk
```bash
cd paper
latexmk -pdf -interaction=nonstopmode main.tex
```

### Option B: pdflatex (two passes) + bibtex
```bash
cd paper
pdflatex -interaction=nonstopmode main.tex
bibtex main
pdflatex -interaction=nonstopmode main.tex
pdflatex -interaction=nonstopmode main.tex
```

The output PDF will be `paper/main.pdf` (or in your TeX build dir, depending on your setup).

## License

- **Paper / text / figures:** Creative Commons Attribution 4.0 International (**CC BY 4.0**) — see [`LICENSE`](LICENSE).
- If you later add software code, consider licensing code separately (e.g., Apache-2.0) and documenting that split in the README.

## How to cite

See [`CITATION.cff`](CITATION.cff).
