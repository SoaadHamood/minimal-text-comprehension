# Semantic Decoding of Brain Activation Using Word Embeddings

This project explores the relationship between **brain activation patterns and semantic representations of words**.  
Using fMRI data and pretrained word embeddings, we train a model that attempts to **decode the semantic concept a person is thinking about based on brain activity**.

The project demonstrates how techniques from **Natural Language Processing (NLP)** can be applied to **computational neuroscience** to analyze semantic representations in the brain.

---

# Project Overview

Humans represent concepts in the brain in complex ways.  
In this project we attempt to decode these representations by mapping **fMRI activation patterns to semantic word vectors**.

The goal is to determine whether **semantic information encoded in brain activity aligns with distributional representations of language learned from text corpora**.

---

# Methodology

The project follows several main steps:

1. **Data Preparation**

The dataset contains:

- fMRI activation patterns recorded while participants think about different concepts
- A set of **180 semantic concepts**

Each concept is associated with:

- a **brain activation pattern**
- a **semantic representation**

---

2. **Semantic Representation**

Each concept is represented using **distributional word embeddings**, which encode semantic meaning as vectors in a high-dimensional space.

These embeddings allow us to represent semantic similarity between concepts.

---

3. **Mapping Brain Activity to Semantics**

A decoding model is trained to learn a mapping:


fMRI activation → semantic embedding


The model attempts to predict the **semantic vector corresponding to the concept represented by the observed brain activity**.

---

4. **Dimensionality Reduction**

To analyze and visualize the structure of the data, dimensionality reduction techniques are applied:

- **PCA (Principal Component Analysis)**
- **t-SNE**

These methods allow us to explore how brain activation patterns cluster according to semantic relationships.

---

# Visualization

Dimensionality reduction techniques help reveal patterns in the data.

Example goals of visualization:

- Identify clusters of related concepts
- Observe semantic structure in brain activation
- Compare semantic and neural representations

---

# Technologies Used

### Programming Language
- Python

### Libraries

- NumPy  
- Pandas  
- scikit-learn  
- matplotlib  
- seaborn  

### Techniques

- Word embeddings
- Semantic vector representations
- Dimensionality reduction (PCA, t-SNE)
- Decoding models

---

# Repository Structure


minimal-text-comprehension
│
├── unstructured_part_lastv.ipynb # Main analysis notebook
├── data/ # Brain activation and concept data
├── utils/ # Helper functions
│
└── README.md


---

# Example Workflow


Brain Activation Data
↓
Preprocessing
↓
Semantic Word Embeddings
↓
Decoding Model
↓
Predicted Semantic Representation
↓
Dimensionality Reduction (PCA / t-SNE)
↓
Visualization of Semantic Structure


---

# Research Motivation

Understanding how semantic concepts are represented in the brain is an important problem in:

- Cognitive science
- Neuroscience
- Natural language processing

By combining **neural data with language embeddings**, this project explores whether **distributional semantic representations align with neural representations of meaning**.

---

# Author

**Soaad Hamood**  
B.Sc. Data and Information Engineering  
Technion – Israel Institute of Technology

GitHub:  
https://github.com/SoaadHamood
