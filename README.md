# causal-networks-cryptocurrency
Repository containing network outputs for "Vector Autoregression in Cryptocurrency Markets: Unraveling Complex Causal Networks" to support reproducibility.


## Contents

This repository provides:

- **T-value matrices**:
  - `tvals_var.csv` — Matrix of $t$-statistics from the VAR model.
  - `tvals_correlation.csv` — Matrix of $t$-statistics from bivariate correlation analysis.
  - `tvals_transfer_entropy.csv` — Matrix of $t$-statistics from transfer entropy analysis.

- **Correlation matrix**:
  - `correlation_matrix.csv` — Full correlation matrix computed across asset returns. Includes node labels. 

- **Adjacency lists (binary networks)**:
  - `VAR_network.adjlist` — Thresholded VAR-based network saved as an adjacency list.
  - `Corr_network.adjlist` — Thresholded correlation-based network saved as an adjacency list.
  - `TE_network.adjlist` — Thresholded transfer entropy-based network saved as an adjacency list.

## Format
- T-value matrices and the correlation matrix are stored as `.csv` plain text files.
- Network structures are provided in `.adjlist` format, listing edges between nodes.
- Nodes correspond to assets indexed consistently across all files.
- Networks are thresholded using a two-tailed $t$-test at a 1% significance level ($t^* = 2.57$).
