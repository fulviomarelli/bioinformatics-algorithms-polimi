# Bioinformatics Algorithms - Lecture Notes

LaTeX source code for the "Bioinformatics Algorithms" course lecture notes (Politecnico di Milano, A.A. 2025/2026). Authored by Fulvio Marelli.

## Overview

This repository contains a comprehensive set of lecture notes covering fundamental and advanced algorithms used in bioinformatics. The document is typeset in LaTeX, providing a clean, structured, and highly readable format for complex mathematical, algorithmic, and biological concepts.

## Topics Covered

1. **Foundations**: Molecular Biology and Sequencing
2. **Sequence Alignment**: String Matching, Needleman-Wunsch (Global), Smith-Waterman (Local)
3. **Genome Assembly**: Overlap-Layout-Consensus (OLC) and De Bruijn Graphs
4. **Pattern Matching & Indexing**: Tries, Suffix Trees, Suffix Arrays, Burrows-Wheeler Transform (BWT), and FM Index
5. **Read Mapping**: BWA optimization and Variant Calling
6. **Phylogenetics & MSA**: Evolutionary Trees, Multiple Sequence Alignment, Heuristics, and Stochastic Search
7. **Probabilistic Models**: Hidden Markov Models (HMMs) in Bioinformatics

## Project Structure

- `main.tex`: The root document. Handles preamble, package imports, and doc structure.
- `data/`: Contains individual `.tex` files for each lecture/chapter.
- `imgs/`: Images and figures used throughout the notes.
- `lex_md/`, `matcher/`, `other/`: Additional project assets, scripts, and data.

## Compilation

To compile the final PDF, use `pdflatex`. The project uses the `minted` package for syntax highlighting, which requires the `-shell-escape` flag.

```bash
# Compile the document (run twice to resolve TOC and references)
pdflatex -shell-escape main.tex
pdflatex -shell-escape main.tex
```

### Key Dependencies
- `tcolorbox`: Used for custom theorem/definition boxes.
- `tikz` / `circuitikz`: Used for automata and logic diagrams.
- `hyperref`: Manages document cross-references and internal links.
- `minted`: Syntax highlighting (requires Python and Pygments installed).

## License

Created for academic purposes. Politecnico di Milano.
