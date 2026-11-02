# t-SNE from Scratch

A from-first-principles implementation of t-SNE (t-Distributed Stochastic Neighbor Embedding) in NumPy, benchmarked against `sklearn.manifold.TSNE`.

The notebook derives the high-dimensional Gaussian affinities, the Student-t affinities in the embedding, the KL divergence objective and its gradient, and maps each of them directly onto code:

- `conditional_probabilities`: per-point binary search on $\sigma_i$ to match the target perplexity.
- `joint_probabilities` and `low_dim_affinities`: the symmetric distributions $P$ and $Q$.
- `kl_gradient`: fully vectorised gradient, checked against finite differences.
- `TSNE`: scikit-learn style class with PCA or random initialisation, early exaggeration, momentum and adaptive gains.

It is evaluated on 10-dimensional synthetic clusters (perplexity calibration, convergence, how the embedding evolves) and on the digits dataset, where it is compared with scikit-learn by KL divergence, trustworthiness and run time. A final section shows the effect of perplexity.

All data is generated or loaded with scikit-learn, so no external files are needed.

## Requirements

```
numpy
pandas
matplotlib
scikit-learn>=1.5
```
