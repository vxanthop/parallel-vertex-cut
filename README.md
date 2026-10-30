# Small Vertex Cut in the PRAM Model

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23817023.svg)](https://doi.org/10.5281/zenodo.23817023)

This repository contains the LaTeX source code and compiled manuscript for **Small Vertex Cut in the PRAM Model**, which formalizes and archives results originally developed as part of my Master's thesis.

📄 **[Read the compiled PDF here](./main.pdf)**

## Overview
The vertex cut problem asks for a minimum set of vertices whose removal disconnects a given graph. It has applications in fault-tolerant network design, parallel computation, and distributed systems. This work studies the problem in the PRAM model. 

Building on the sequential algorithm of Nanongkai et al. for small vertex connectivity and the parallel reachability algorithm of Sidford et al., I present a parallel randomized algorithm for finding a separator of size less than $k$. The algorithm gives a work–depth tradeoff controlled by a parameter $\alpha$. For $k = O(\sqrt{n})$, it achieves $\tilde{O}(mk^2 + m^2/\alpha)$ work and $\max\{n^{1/2+o(1)}, k\alpha\}$ depth with high probability. For constant $k$, I also give a vertex-sampling variant that improves the work in dense regimes.

## Origin and Context
This manuscript cleans up, formalizes, and presents the results originally developed in my Master's thesis at the **National Technical University of Athens (NTUA)**, conducted in collaboration with Yonngang Jiang (Max Planck Institute for Informatics) and supervised by Danupon Nanongkai. 

* 🏛️ **Original Thesis Archive:** [NTUA Artemis Repository](https://artemis.ece.ntua.gr/items/a08524a3-c9af-4fd9-9eca-297381914ef6)
* 📚 **Zenodo Archive Record:** [Zenodo Record](https://zenodo.org/records/23817023)

## Compiling from Source
If you wish to compile the PDF locally from the provided source files, ensure you have a standard LaTeX distribution installed and run:

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

## License

The manuscript and LaTeX source code in this repository are licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](LICENSE). 


