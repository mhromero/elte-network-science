# ELTE Network Science Coursework

Participants: María Romero Huertas and Javier Martín Fuentes

This repository is a portfolio of Network Science coursework. It combines weekly laboratory exercises with a final project that studies character relationships across the Harry Potter books.

## Overview

The [final project](final_project/) investigates whether the social structure that emerges from character appearances in the Harry Potter books can be described with established network-science models. It constructs weighted, undirected character co-occurrence networks for each book and for the full series, using repeated appearances within a three-paragraph sliding window as a proxy for interaction strength.

The workflow cleans and standardizes character names, including aliases and alternative references, then matches those names against the book texts. The resulting networks are examined through centrality and structural measures, community detection, robustness simulations, and their evolution over the series. The project also compares the observed network with generative models, including Barabási–Albert, Bianconi–Barabási, and Double Preferential Attachment models.

The accompanying [final report](final_project/docs/report.pdf) documents the methodology, analysis, results, and cited data sources; a [presentation](final_project/docs/presentation.pdf) is also included.

## Tech Stack

The notebooks use Python and Jupyter, principally with pandas, NetworkX, NumPy, Matplotlib, Seaborn, SciPy, scikit-learn, and tqdm. Some exercises and analyses additionally use Beautiful Soup, Requests, python-louvain, CDlib, Dash, Plotly, Graphviz/PyGraphviz, and Cytoscape session files.

## Coursework Contents and Structure

The [labs/](labs/) directory contains the weekly exercises, while [final_project/](final_project/) contains the larger character-network study.

- **Lab 1 — Cytoscape basics:** creates and explores networks with Cytoscape.
- **Lab 2 — Zachary Karate Club:** examines the Karate Club social network and its properties.
- **Lab 3 — Ego networks and social-media communities:** loads and analyzes a Facebook ego network, then prepares results for Cytoscape.
- **Lab 4 — Graphviz:** creates directed graphs and compares Graphviz layouts.
- **Lab 5 — Random networks:** explores Erdős–Rényi graphs, connectivity, clustering, path lengths, and degree distributions.
- **Lab 6 — Network growth:** implements and evaluates the Barabási–Albert model against a collaboration network.
- **Lab 8 — Fitness-based growth:** implements the Bianconi–Barabási model and investigates fitness-dependent degree distributions.
- **Lab 9 — Degree correlations:** measures and manipulates assortativity in networks.
- **Lab 10 — Network robustness:** studies percolation, attack tolerance, cascading failures, and robust-network design.
- **Lab 11 — Community detection:** compares hierarchical clustering, modularity optimization, overlapping communities, and community characterization.

## Getting Started

### Requirements

The work is provided as completed Jupyter notebooks and includes their saved outputs. Notebook metadata records Python 3.11 and 3.12 environments, but the repository does not include a pinned environment or dependency lockfile. Interactive use therefore requires a compatible Python and Jupyter installation, together with the libraries listed above; Graphviz/PyGraphviz and Cytoscape are needed only for notebook cells and session files that use them.

### Installation

No verified clean-room installation procedure is provided, because the coursework has no managed dependency specification. Install the required tools in an isolated environment appropriate for the notebook you intend to inspect.

### Running

Open an individual `.ipynb` file in Jupyter to inspect its saved work or run cells interactively. The repository is presented as archived coursework, so a complete from-scratch rerun is not guaranteed.

## Results

The final project provides programmatically generated network figures in [results/figures](final_project/results/figures/) and explains the analysis in the [final report](final_project/docs/report.pdf).

## Academic Context

This repository preserves Network Science coursework. The final project was completed by María Romero Huertas and Javier Martín Fuentes, as identified in the final report.
