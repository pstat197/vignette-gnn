# vignette-gnn
Group 3 - Graph Neural Networks

Vignette on using graph neural networks (GNNs) for molecular property prediction, with an example task predicting whether a molecule is permeable to the blood–brain barrier; created as a class project for PSTAT197A (Fall 2025).

---

## Contributors
- Emily Tian (@emilytian0)
- Pratyush Rallapally (@p-rallapally)
- Jasper Luo(@JasperLuo0228)
- Adarsh (@anagar16)
- Nathan Kim (@nakim12)

---

## Vignette Abstract
Graph neural networks (GNNs) are a class of neural networks designed to operate on graph structured data, where observations are represented as nodes connected by edges. This makes them powerful for molecular machine learning, since molecules naturally form graphs. Atoms act as nodes, and chemical bonds act as edges. By leveraging these relational structures, GNNs learn expressive representations that support accurate property prediction.

In this vignette, we demonstrate how to use GNNs for molecular property prediction using the `chemprop` package. As a real world example, we train a GNN to classify whether a small molecule is permeable to the blood brain barrier (BBB), a key consideration in drug development, since compounds must cross the BBB to act on targets in the central nervous system. The tutorial walks through data preparation, model training, prediction, and evaluation using ROC–AUC, providing a clear, introduction for PSTAT197 students learning GNNs.

---

## Repository Contents
The repository is organized as follows to maintain clarity, reproducibility, and ease of navigation:

```
root/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── model_checkpoints/bbbp_checkpoints/
│   └── model_0/
│        ├── checkpoints/
│        ├── trainer_logs/version_0
│        ├── args.json
│        └── config.toml
│
├── scripts/
│   ├── Vignette_Introduction.ipynb
│   ├── vignette_gnn.ipynb
│   └── vignette_gnn_script.ipynb
│
├── vignette_gnn_final.ipynb
├── vignette_gnn_final.html
├── README.md
```

## References
- Distill.pub. *A Gentle Introduction to Graph Neural Networks.* https://distill.pub/2021/gnn-intro/
- Yang, K. et al. *Analyzing Learned Molecular Representations for Property Prediction.* https://pubs.acs.org/doi/10.1021/acs.jcim.9b00237