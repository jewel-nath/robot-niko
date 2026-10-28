# Technical report

**Robot Niko: A Life-Size 3D-Printed Humanoid Assistant on a Raspberry Pi —
System Design and Build.** Version 1.1, October 2026.

By Jewel Nath, Shanjit Mondol, Tousif Bin Parves, Md Mohiuddin Khan Mahin and
Anik Chakraborty (Quanta Robotics).

[Read the PDF](robot-niko-report.pdf) (15 pages, one column). On Zenodo:
[doi:10.5281/zenodo.23700587](https://doi.org/10.5281/zenodo.23700587), which
always points to the latest version.

It describes Niko's mechanical build, electronics, software, motion, voice and
vision, the behaviours recorded on video in December 2022, and the next steps.
Every number in it comes from this repository's code and configuration.

Every diagram is also in [docs/diagrams/](../diagrams/README.md) as its own PDF
and PNG, for reuse.

## Files

| Path | What it is |
|---|---|
| `robot-niko-report.tex` | The report |
| `style.tex` | The page layout: one column, 11 pt, coloured headings and summary boxes |
| `figure-style.tex` | Fonts, the colour palette and the TikZ styles every figure shares |
| `references.bib` | The references; every DOI was checked at doi.org |
| `figures/` | One file per diagram (`figNN-*.tex`, TikZ) or plot (`plotNN-*.tex`, pgfplots), each naming the code it was drawn from |
| `make-diagrams.py` | Builds each figure as its own cropped PDF in `docs/diagrams/` |
| `robot-niko-report.pdf` | The built report |

The photos come from [docs/media/](../media/). The report and its diagrams
are under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/); the code
keeps its MIT licence.

## Build it

With [Tectonic](https://tectonic-typesetting.github.io), which fetches the
LaTeX packages and the TeX Gyre fonts it needs on the first run:

```bash
cd docs/report
tectonic -X compile robot-niko-report.tex
python make-diagrams.py
```

The style uses `fontspec`, so another TeX distribution needs XeLaTeX or
LuaLaTeX (`latexmk -xelatex robot-niko-report.tex`).
