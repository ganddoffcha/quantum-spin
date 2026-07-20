# Quantum Spin

**Representations of Lie Groups and Lie Algebras: A Mathematical Dissection of Quantum Spin**

Gordon Chan (U2440785A) · Odyssey Research Programme · School of Physical and Mathematical Sciences, NTU

Supervised by Assoc. Prof. François Gay-Balmaz

## Abstract

Introductory quantum mechanics often introduces the concept of spin heuristically. This project investigates the mathematical foundations of quantum mechanical spin — exploring the geometric and algebraic origins of spin in the language of Lie groups, Lie algebras, and their unitary irreducible representations. A central focus is the topological and algebraic relationship between the rotation group SO(3) and its universal double cover SU(2) ≅ S³. By classifying the irreducible representations of SU(2), we present how this abstract algebraic classification naturally gives rise to the physical phenomena of integer and half-integer spin, bridging topology, abstract algebra, and quantum physics.

## Files

| File | Description |
|------|-------------|
| [`gordon-chan-quantum-spin.pdf`](gordon-chan-quantum-spin.pdf) | Full paper with complete proofs (30 pages) |
| [`poster.pdf`](poster.pdf) | A1 poster summary |

## Build

```bash
cd poster && TEXINPUTS=.:../texnow//: latexmk -lualatex poster.tex
cd "Representation Theory of Lie" && TEXINPUTS=.:../texnow//: latexmk -pdf Representations_of_Lie_Groups_*.tex
```

Uses [`leopard.sty`](https://github.com/ganddoffcha/documents/tree/main/texnow) v3 — a custom LaTeX style file with 60+ math macros.

## License

[CC BY 4.0](LICENSE) — you are free to share and adapt with attribution.
