# Wasserstein K-Center Clustering with Robust Validation

This repository contains the official implementation and manuscript for a Wasserstein K-center and K-median clustering framework designed for distribution-valued data. The project integrates semi-free support barycenters, Wasserstein Fréchet medians (IRLS), and a robust validation metric based on Wasserstein spatial depth (ReD).

## Overview

This work provides a complete algorithmic and theoretical toolkit for clustering probability distributions in Wasserstein space. The framework includes:

1. Semi-free support Wasserstein barycenters for flexible representation of cluster centers.
2. Wasserstein Fréchet medians computed via an iteratively reweighted least squares (IRLS) method.
3. Wasserstein K-median / K-center clustering algorithms with PAM-based warm starts.
4. A depth-based validation metric (ReD) for selecting the number of clusters K.
5. Theoretical results establishing a Pollard-type strong consistency guarantee for Wasserstein K-means under compact-support assumptions.

The complete methodology and experimental analysis are documented in:

    Manuscript.pdf

## Repository Structure

    .
    ├── Manuscript.pdf
    ├── Fixed-support version/
    ├── Semi-Free Support Version/
    ├── README.md
    └── .gitignore

## Features

- Robust clustering of distribution-valued datasets
- Free-support and fixed-support barycenter solvers
- IRLS Wasserstein median computation
- Depth-based validation for determining K
- Demonstrated on synthetic mixtures, MNIST distributions, and AML flow cytometry data

## Usage

To use this repository:

1. Clone the project:
       git clone https://github.com/your-username/your-repo-name.git
       cd your-repo-name

2. Explore either implementation:
       Fixed-support version/
       Semi-Free Support Version/

Both folders contain complete scripts for clustering, validation, and experimental reproduction.

## Dependencies

Typical Python requirements include:

    numpy
    scipy
    matplotlib
    joblib
    POT  (Python Optimal Transport)
    scikit-learn
    pandas


## License

This repository is provided for academic and research purposes.

