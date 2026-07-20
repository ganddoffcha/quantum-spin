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
| [`gordon-chan-quantum-spin.pdf`](gordon-chan-quantum-spin.pdf) | Full paper (pdflatex) |
| [`poster.pdf`](poster.pdf) | A1 poster (lualatex) |
| [`paper/`](paper/) | Paper LaTeX source |
| [`poster/`](poster/) | Poster LaTeX source |

## Build

```bash
# Paper (pdflatex)
cd paper && TEXINPUTS=.:/path/to/texnow//: latexmk -pdf Representations_of_Lie_Groups_*.tex

# Poster (lualatex)
cd poster && TEXINPUTS=.:/path/to/texnow//: latexmk -lualatex poster.tex

# Or publish everything in one command
./publish
```

Uses [`leopard.sty`](https://github.com/ganddoffcha/documents/tree/main/texnow) v3 — a custom LaTeX style file with 60+ math macros.

## License

[CC BY 4.0](LICENSE) — you are free to share and adapt with attribution.
