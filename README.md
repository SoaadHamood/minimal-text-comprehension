This project explores the relationship between brain activation patterns and semantic representations of words.
The goal is to learn how neural activity recorded using fMRI can be mapped to semantic word vectors, enabling the prediction of the concept a person is thinking about based on brain signals.

The project demonstrates how distributional word embeddings can be used to decode semantic meaning from neural activation patterns.

Overview

Human brain activity encodes semantic information when we think about concepts such as animals, tools, or places.
This project investigates whether it is possible to recover the semantic concept from brain activation data.

We use:

fMRI activation patterns corresponding to 180 different concepts

pretrained word embeddings representing semantic meaning

machine learning models to decode semantic vectors from neural signals

The trained decoder learns a mapping:

Brain activation (fMRI) → Semantic vector → Concept
Dataset

The dataset contains:

fMRI brain activation patterns recorded for 180 concepts

Each concept is associated with a semantic representation vector

Each sample consists of:

Brain activation vector
+
Semantic embedding vector

The task is to learn a function that maps brain activation to its corresponding semantic representation.

Methodology

The pipeline consists of several steps:

1. Data Representation

Brain activation patterns are represented as high-dimensional vectors corresponding to voxel activations.

Concept meanings are represented using distributional word embeddings.

2. Learning the Decoder

A model is trained to learn the mapping:

fMRI activation → semantic embedding

The decoder attempts to reconstruct the semantic vector associated with a concept based on brain activation patterns.

3. Concept Prediction

Given unseen brain activation data, the system:

Predicts the semantic embedding

Finds the closest concept in the embedding space

This allows the model to infer which concept produced the neural activity.

Visualization

To analyze the structure of the data and the learned representations, dimensionality reduction techniques are applied:

PCA (Principal Component Analysis)

t-SNE

These methods allow visualization of how brain activation patterns cluster according to semantic categories.

Technologies Used

Programming Language:

Python

Libraries:

NumPy

pandas

scikit-learn

matplotlib

seaborn

Techniques:

Word embeddings

Linear decoding models

PCA

t-SNE

Semantic similarity analysis

Example Pipeline
fMRI Brain Activation
        ↓
Feature Representation
        ↓
Decoder Model
        ↓
Predicted Semantic Vector
        ↓
Nearest Concept in Embedding Space
Project Structure
minimal-text-comprehension
│
├── data
│   ├── fmri_data
│   └── semantic_vectors
│
├── notebooks
│   └── unstructured_part_lastv.ipynb
│
└── README.md
Results

The learned decoder demonstrates that semantic representations can be partially recovered from neural activation patterns, showing meaningful alignment between brain activity and distributional word embeddings.

Visualization of the embedding space reveals clusters corresponding to related semantic concepts.

Author

Soaad Hamood
B.Sc. Data and Information Engineering
Technion – Israel Institute of Technology

GitHub:
https://github.com/SoaadHamood
