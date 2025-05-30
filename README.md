# 🧬 ML Frameworks in Spatial Transcriptomics Analysis Methods

This repository summarizes recent machine learning (ML) frameworks applied in **spatial transcriptomics** data analysis. These methods focus on discovering spatial domains, cell types, and embedding representations from high-dimensional single-cell gene expression data.

---

## 🚀 Key ML Frameworks

### 1️⃣ Graph Neural Networks (GNNs)
- **Use case**: Modeling gene expression dependencies between neighboring spots or cells.
- **Example**: 
  - **UTAG**: Combines graph smoothing with clustering.
  - **BANKSY**: Uses azimuthal Gabor filters to project gene expression into an embedding space.

### 2️⃣ Variational Autoencoders (VAEs)
- **Use case**: Learning low-dimensional embeddings that preserve both feature and graph structure.
- **Example**: 
  - **VGAE**: Graph-based VAE (lacks explicit feature reconstruction loss).
  - **BASS**: Incorporates feature reconstruction likelihood directly.

### 3️⃣ Topic Models
- **Use case**: Modeling spatial domains and cell types jointly.
- **Example**: 
  - **SpatialTopic**: Fast and interpretable; uses collapsed Gibbs sampling.

### 4️⃣ Gaussian Mixture Models (GMMs)
- **Use case**: Clustering nodes (spots/cells) by accounting for feature variance across dimensions.
- **Example**:
  - Used in **BASS** to improve clustering performance over KMeans.

---

## 📊 Data Benchmarks

- Annotated **MERFISH mouse hypothalamus** data.
- Simulated data sets.
- **10x Genomics Xenium** breast tissue.
- **NanoString CosMx** NSCLC tissue.

---

## 🔥 Notable Trends

- Models increasingly integrate **spatial information** and **gene expression**.
- Combining **generative models** with **probabilistic clustering** (e.g., GMM) enhances interpretability.
- Growing focus on benchmarking across **real** and **simulated** datasets.

---

## 📚 References

- **BASS**: Models feature likelihood, includes GMM clustering, and adds feature reconstruction.https://github.com/zhengli09/BASS
- **UTAG**: Simple and fast; uses graph smoothing plus clustering.https://github.com/ElementoLab/utag.
- **BANKSY**: Projects expression data with spatial filtering.https://github.com/prabhakarlab/Banksy_py
- **SpatialTopic**: Uses topic modeling with collapsed Gibbs sampling.https://github.com/xiyupeng/SpaTopic/
- **VGAE**: Variational Graph Autoencoder (basic form).github.com/tkipf/gae

---

## ⚙️ Environment

Install recommended packages:
```bash
pip install numpy pandas scikit-learn torch openpyxl
