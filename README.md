# Quantum Spin

**Representations of Lie Groups and Lie Algebras: A Mathematical Dissection of Quantum Spin**

Chan Lok Hin Gordon (U2440785A) · Odyssey Research Programme
School of Physical and Mathematical Sciences, NTU

Supervised by Assoc. Prof. François Gay-Balmaz

## Abstract

Introductory quantum mechanics often introduces the concept of spin heuristically. This project investigates the mathematical foundations of quantum mechanical spin — exploring the geometric and algebraic origins of spin in the language of Lie groups, Lie algebras, and their unitary irreducible representations. A central focus is the topological and algebraic relationship between the rotation group SO(3) and its universal double cover SU(2) ≅ S³. By classifying the irreducible representations of SU(2), we present how this abstract algebraic classification naturally gives rise to the physical phenomena of integer and half-integer spin, bridging topology, abstract algebra, and quantum physics.

## Files

| File | Description |
|------|-------------|
| [`gordon-chan-quantum-spin.pdf`](gordon-chan-quantum-spin.pdf) | Full paper (pdflatex, ~30 pages) |
| [`poster.pdf`](poster.pdf) | A1 conference poster (lualatex) |
| [`slides.pdf`](slides.pdf) | Presentation slides (pdflatex) |
| [`paper/`](paper/) | Paper LaTeX source + [`leopard.sty`](paper/leopard.sty) |
| [`poster/`](poster/) | Poster LaTeX source + [`leopard.sty`](poster/leopard.sty) |
| [`slides/`](slides/) | Slides LaTeX source + [`leopard.sty`](slides/leopard.sty) |

## Build

### Prerequisites

A TeX distribution with `pdflatex`, `lualatex`, and `latexmk`:

- **TeX Live** (Linux): `sudo apt install texlive-full` or `texlive` + `latexmk`
- **MiKTeX** (Windows): [miktex.org](https://miktex.org)
- **MacTeX** (macOS): [tug.org/mactex](https://tug.org/mactex)

The repository is self-contained — `leopard.sty` is bundled in each source directory. No external dependencies.

### Compile everything

```bash
# Paper (pdflatex) → out/paper.pdf
cd paper && latexmk -pdf paper.tex

# Poster (lualatex) → out/poster.pdf
cd poster && latexmk -lualatex poster.tex

# Slides (pdflatex) → out/slides.pdf
cd slides && latexmk -pdf slides.tex
```

Each `latexmk` run produces the PDF in an `out/` subdirectory. Run twice if cross-references or table of contents need updating.

### Publish (author only)

```bash
./publish
```

Compiles all three, copies PDFs to repo root, commits, and pushes to GitHub.

## Style file

[`leopard.sty`](paper/leopard.sty) v3 — a custom LaTeX style file with 60+ math macros, theorem environments, and typographic presets. Bundled in each source directory; no separate install needed.

## License

[CC BY 4.0](LICENSE) — you are free to share and adapt with attribution.
