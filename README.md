# Nikassh Bala
*AI Systems for Genetic Analysis, Space Life Sciences & Multiscale Systems Engineering*

[![Research Domain](https://img.shields.io/badge/Research-Computational%20Biology%20%26%20Space%20Omics-10529F?style=for-the-badge&logo=dna&logoColor=white)](#)
[![Stack](https://img.shields.io/badge/Stack-PyTorch%20%7C%20PyG%20%7C%20SciPy%20%7C%20WNTR-orange?style=for-the-badge)](#)
[![Data](https://img.shields.io/badge/Data-NASA%20GeneLab%20%7C%20ChEMBL%20%7C%20CTD-red?style=for-the-badge)](#)

---

## 🔬 Executive Summary & Research Profile

I engineer computational biology systems, deep graph learning pipelines, and multiscale dynamical solvers to solve complex challenges in **Space Life Sciences**, **Epidemic Modeling**, and **Environmental Systems Engineering**. 

My core focus spans:
1. **Graph Neural Networks (GNNs) for Drug Discovery**: Link prediction on heterogeneous knowledge graphs integrating transcriptomics (NASA GeneLab) with bioactivity databases (ChEMBL, CTD) to identify drug candidates for microgravity-induced physiological stress.
2. **Multiscale Compartmental ODE Solvers**: Coupling within-host intra-cellular viral kinetics with population-level macro-epidemiology to capture non-linear disease dynamics and behavioral feedbacks.
3. **Reactive Transport & Water Quality Engineering**: EPANET-MSX multi-species biofilm dynamics and Global Sensitivity Analysis (Sobol/eFAST) for opportunistic pathogen persistence.

---

## 🌟 Featured Research Repositories

<div align="center">

| Repository | Research Domain | Key Methodologies |
| :--- | :--- | :--- |
| 🚀 [`gnn-drug-repurposing-spaceflight-atrophy`](https://github.com/Nikassh/gnn-drug-repurposing-spaceflight-atrophy) | Space Life Sciences & Bio-AI | Heterogeneous GraphSAGE, NASA GeneLab DEG Consensus, Ensembl Orthologs |
| 🦠 [`Coupled-Epidemic-ODE-Solver`](https://github.com/Nikassh/Coupled-Epidemic-ODE-Solver) | Multiscale Mathematical Biology | Stiff ODEs (Radau), Next-Gen Matrix $R_0$, 134-State SEPIAQRV |
| 💧 [`legionella-biofilm-msx-model`](https://github.com/Nikassh/legionella-biofilm-msx-model) | Environmental Systems Engineering | WNTR / EPANET-MSX, Biofilm Detachment, Sobol Global Sensitivity |

</div>

---

## 🧮 Theoretical & Mathematical Foundations

### 1. Heterogeneous Graph Convolution (Spaceflight Therapeutic Discovery)
Node representation updates across relation types $r \in \mathcal{R}$ connecting Gene, Drug, and Ortholog entities:

$$\mathbf{h}_{v}^{(k)} = \sigma \left( \mathbf{W}_{\text{self}}^{(k)} \mathbf{h}_{v}^{(k-1)} + \sum_{r \in \mathcal{R}} \sum_{u \in \mathcal{N}_r(v)} \frac{1}{|\mathcal{N}_r(v)|} \mathbf{W}_{r}^{(k)} \mathbf{h}_{u}^{(k-1)} \right)$$

### 2. Intra-Host to Macro-Population Transmission Coupling
Coupling within-host viral load $V(\tau)$ to the force of infection $\lambda(t)$ via Hill kinetics:

$$\beta(V) = \beta_{\text{max}} \cdot \frac{V^n}{\text{EC}_{50}^n + V^n}, \quad \lambda(t) = \beta(V) \cdot \frac{\sum (I_{\text{symptom}} + \epsilon A)}{N}$$

---

## 🛠️ Technical Capabilities

- **Deep Learning & Graph Mining**: PyTorch, PyTorch Geometric (PyG), HeteroData, NetworkX, DeepSNAP
- **Scientific Computing & ODEs**: SciPy (`solve_ivp`), NumPy, SymPy, Matplotlib, Seaborn
- **Bioinformatics & Systems Biology**: DESeq2 / Limma differential expression, Ensembl REST API, ChEMBL API, CTD API
- **Environmental Hydraulics**: WNTR, EPANET-MSX, SALib (Sobol / eFAST Global Sensitivity Analysis)
- **Software Standards**: Modular Python packaging (`src/`), PyTest, Docker, GitHub Actions (CI/CD), LaTeX, BibTeX

---

## 📜 Citation & Academic Metadata

If you reference or build upon any of these computational frameworks in your research, please use the citation metadata provided in each repository's `CITATION.cff`.

```bibtex
@misc{bala2026computational,
  author       = {Bala, Nikassh},
  title        = {Computational Biology, Space Life Sciences, and Multiscale Dynamical Solvers},
  publisher    = {GitHub},
  year         = {2026},
  url          = {https://github.com/Nikassh}
}
```
